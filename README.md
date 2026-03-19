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

## Installation / Einbindung in GitHub Copilot CLI

### Voraussetzungen

- GitHub Copilot CLI ist installiert
- Du bist in Copilot CLI eingeloggt (`/login`)

### Plugin installieren

1. Copilot CLI starten:
   - `copilot`
2. Plugin-Manager öffnen:
   - `/plugin`
3. Plugin aus Git-Repository hinzufügen:
   - Repository: `https://github.com/silvio-l/amboss-copilot-plugin`
4. Plugin aktivieren (falls nicht automatisch aktiv):
   - Im `/plugin`-Dialog auf **enabled** setzen

### Agent aktivieren

1. Agent-Auswahl öffnen:
   - `/agent`
2. `amboss:amboss` auswählen
3. Optional prüfen:
   - Neue Anfrage stellen und im Header prüfen, dass Amboss aktiv ist

### Alternative: Lokale Entwicklungsversion verwenden

Wenn du lokal an Amboss entwickelst, kannst du den lokalen Ordner statt der Git-URL einbinden:

- Plugin-Ordner:  
  `C:\Users\<dein-user>\.copilot\installed-plugins\_direct\silvio-l--amboss`

Danach im `/plugin`-Manager aktivieren und über `/agent` auswählen.

## Notes

- Language and workflow are optimized for German-speaking development teams.
- Review model fallback behavior is configured in `agents/amboss.agent.md`.
