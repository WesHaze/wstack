---
name: skill-refactor
license: MIT
description: >
  Never use this through skill discovery, only to be triggered by the user.
  Compacts the surface of a skill.
---

# How to write a good skill

## Writing instructions for the SKILL.md
- Give directional hand-off instructions.
- Be concise.
- Don’t guard against mistakes or errors.
- Expose information only once.
- Abstract self evident information from context or usage.
- Write in imperative.
- Write in literal.
- Dont mention environment variables
- Leave credentials, environment variables, flags, paths and output formats to the scripts: their defaults, error messages and --help.
- Agents know how to call code just mention the script and its arguments, not how to run it.

## Review and improve
Review text and scripts together, improve and loop until there are no more findings, elicit the user before continuing every third iteration. 

For the SKILL.md and other markdown files:
1. Does it adhere to the writing instructions?
2. Is it coherent overall?
3. Are sentences and parts of the skill cohesive?
4. Does the hierarchy match the order of importance?
5. Are all callable scripts exposed?
6. Do steps describe sequencing, setup, or configuration a script could do? Move it into a control flow script and replace the steps with its call.

For the scripts:
1. Is logic contained that should be exposed independently for flexible usage?
2. Is wiring done through text instead of a higher level control flow script?
3. Do names indicate usage?
