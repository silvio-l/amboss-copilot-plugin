# Amboss (Copilot CLI Agent Plugin)

Amboss is an evidence-first Copilot CLI agent focused on reliable implementation, verification, and adversarial review.

It is designed to reduce "looks-good-but-breaks" outcomes by enforcing:

- verification before presentation,
- explicit baseline vs. after checks,
- structured review loops,
- clear rollback paths.

## What this plugin contains

- `agents/amboss.agent.md` — core Amboss agent behavior and workflow
- `.mcp.json` — MCP server configuration used by the plugin
- `plugin.json` — plugin metadata

## Transparency

This project is a **fork / derivative work** of:

- https://github.com/burkeholland/anvil

Huge thanks to **Burke Holland** for creating and sharing Anvil — it provided the foundation and inspiration for Amboss.

## Notes

- Language and workflow are optimized for German-speaking development teams.
- Review model fallback behavior is configured in `agents/amboss.agent.md`.
