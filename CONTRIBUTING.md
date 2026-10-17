# Contributing

Contributions that improve the usefulness, accuracy, accessibility, or
maintainability of these Copilot customizations are welcome.

## Before you start

- For a substantial change, open an issue first to discuss its purpose and
  scope.
- Keep each agent focused on a clear role and each skill focused on a
  repeatable, on-demand workflow.
- Avoid duplicating instructions across an agent and a skill; put reusable
  procedures in the skill and have the agent refer to it.

## Prepare a change

1. Edit the relevant agent under `com.github.copilot/agents/` or skill under
   `skills/`.
2. Check frontmatter delimiters and YAML syntax. For skills, confirm the
   `name` matches the containing directory.
3. Check descriptions for clear task triggers, and review any relative links
   or referenced assets.
4. Keep guidance accurate for the target framework and version. Avoid
   prescribing migrations, dependencies, or conventions without a clear
   reason.
5. If practical, try the customization in a GitHub Copilot workspace and
   describe what you verified in the pull request.

There is no automated validation suite yet. Validate `plugin.json` as JSON and
check that the skill and agent paths referenced by the package exist. Do not
claim automated checks passed unless a check was actually run.

## Pull requests

- Keep a pull request focused and explain the user problem it solves.
- Include the affected agent or skill and summarize meaningful behavior
  changes.
- Note manual or automated validation performed, or explain why validation
  was not practical.
- Update the README when repository usage or distribution guidance changes.

By submitting a contribution, you confirm that you have the right to submit
it. Contributions are distributed under the repository's MIT License, subject
to its terms.
