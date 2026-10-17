---
description: "Use when creating or editing GitHub Copilot custom agents or agent skills in this repository. Covers scope, frontmatter, discoverability, validation, and sharing."
applyTo: "com.github.copilot/agents/**, skills/**"
---

# Customization Authoring

- Choose the smallest primitive that fits: use a custom agent for a focused
  persona or delegated role, and a skill for an on-demand repeatable workflow.
- Keep each agent's role and boundaries clear. Include a specific,
  keyword-rich `description`; grant only the tools the role needs when tools
  must be restricted.
- Give every skill a directory containing `SKILL.md`. The skill's lowercase,
  hyphenated `name` must match its directory, and its description must explain
  when to load it.
- Put reusable procedures in skills. When an agent relies on a skill in this
  repository, explicitly name and link it from the agent body, and tell the
  agent when to follow it. Do not duplicate the skill's instructions in the
  agent.
- Keep guidance version-aware and grounded in the target project's files.
  Avoid imposing framework migrations, dependencies, or conventions without a
  clear need.
- Before sharing a change, check frontmatter delimiters and YAML syntax, verify
  skill names match their folders, and review relative links and referenced
  assets.
