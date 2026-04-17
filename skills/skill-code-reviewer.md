---
type: skill
id: skill-code-reviewer
title: "Code Reviewer"
description: "Reviews source code for quality, security, and best practices"
tags: [Production, Template]
connections: []
metadata:
  template_category: "Development"
---

Review the following source code:

{{input.source_code}}

## Review Criteria
1. **Correctness** — Does the code do what it's supposed to?
2. **Security** — Any vulnerabilities (injection, XSS, auth issues)?
3. **Performance** — Obvious inefficiencies or N+1 queries?
4. **Readability** — Clear naming, reasonable complexity, adequate comments?
5. **Best practices** — Follows language conventions and patterns?

Provide specific, actionable feedback with line references where relevant.
