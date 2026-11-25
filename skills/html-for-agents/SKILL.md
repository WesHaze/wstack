---
name: html-for-agents
license: MIT
description: >
  Use when working on public webpages.
  Aims to harden agentic page visits information extraction.
---

# Conveying the same information to agents as we do human readers
1. What does the page tell humans both explicitly and implicitly with visual cues?
2. Create a list of sampling questions based on the html with correct answers, cover some edge cases.
3. Hand a smaller model with a lower level of reasoning the html through a local server and questions, record wrong answers.
4. Iterate on the html
  1. Does the answer show what went wrong and thus imply the solution?
  2. Should and can we avoid altering the human user experience?