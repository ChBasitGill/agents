# Angular Frontend Agent Plugin

An Agent Plugins 1.0 package for Angular frontend work. It includes an
on-demand Angular skill and a GitHub Copilot-specific frontend agent.

## Included

- `skills/angular-frontend/SKILL.md` — version-aware Angular implementation
  and review workflow.
- `com.github.copilot/agents/angular-frontend.agent.md` — Angular frontend
  agent that links to and follows the skill.
- `.github/instructions/customization-authoring.instructions.md` — repository
  guidance for creating and maintaining customizations.

## Install in VS Code

This repository is an [Agent Plugins 1.0](https://code.visualstudio.com/docs/agent-customization/agent-plugins)
package, not a VS Code extension. In a VS Code version that supports Agent
Plugins and the experimental [Customization Marketplace](https://code.visualstudio.com/docs/agent-customization/overview#_discover-marketplace-customizations-experimental):

1. Enable `chat.plugins.enabled` and
   `chat.customizations.marketplace.enabled` in Settings.
2. Open **Chat: Open Customizations**, then select **Discover**.
3. Search the GitHub Feed for `angular-frontend`, or use another configured
   plugin marketplace source if the repository is not listed there.
4. Review the source and plugin contents before installing.

Marketplace discovery is experimental and availability can vary by VS Code
version and configured source. See the
[Agent Plugins guide](https://code.visualstudio.com/docs/agent-customization/agent-plugins)
for plugin setup and local development details.

Repository: [github.com/ChBasitGill/agents](https://github.com/ChBasitGill/agents)

## Develop and contribute

Read [CONTRIBUTING.md](./CONTRIBUTING.md) before proposing changes. Agent
Plugins components are kept in the documented plugin layout: skills under
`skills/` and Copilot-specific agents under `com.github.copilot/agents/`.
Authoring guidance lives in `.github/instructions/`.

## License

This project uses the MIT License; see [LICENSE](./LICENSE).

## Marketplace note

The VS Code Customization Marketplace is distinct from the VS Code Extension
Marketplace. Publishing an Agent Plugin does not require a VS Code extension
publisher account or an extension manifest. A public repository and valid
plugin package are prerequisites, but marketplace discovery or indexing is
not guaranteed.
