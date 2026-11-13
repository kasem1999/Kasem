# Mem Skill für Claude AI und Claude Code

Dieses Repository bündelt die offiziellen Beispiel-Skills von Anthropic und das Gedächtnis-Plugin **claude-mem**.

هذا المستودع يجمع السكيلز النموذجية الرسمية من Anthropic مع إضافة الذاكرة **claude-mem**.

## Inhalt / المحتوى

### 1. Example Skills (`.claude/skills/`)

Aus [anthropics/skills](https://github.com/anthropics/skills) — werden in Claude Code automatisch geladen, sobald dieses Repository geöffnet wird.

| Skill | Zweck |
|---|---|
| `algorithmic-art` | Generative Kunst mit p5.js |
| `brand-guidelines` | Anthropic-Markenfarben und Typografie |
| `canvas-design` | Visuelle Designs als PNG/PDF |
| `doc-coauthoring` | Strukturierter Workflow für Dokumente |
| `frontend-design` | Hochwertige Frontend-Oberflächen |
| `internal-comms` | Interne Kommunikation |
| `mcp-builder` | MCP-Server erstellen |
| `skill-creator` | Eigene Skills erstellen und testen |
| `slack-gif-creator` | Animierte GIFs für Slack |
| `theme-factory` | Themes für Artefakte |
| `web-artifacts-builder` | Komplexe HTML-Artefakte (React, Tailwind) |
| `webapp-testing` | Web-Apps mit Playwright testen |

### 2. claude-mem (`.claude/settings.json`)

[claude-mem](https://github.com/thedotmack/claude-mem) ist ein dauerhaftes Gedächtnis für Claude Code: Die nächste Sitzung beginnt dort, wo die letzte aufgehört hat.

Der Marketplace `thedotmack` ist in `.claude/settings.json` registriert und das Plugin aktiviert. Beim ersten Öffnen fragt Claude Code, ob dem Marketplace vertraut werden soll. Manuelle Installation:

```
/plugin marketplace add thedotmack/claude-mem
/plugin install claude-mem
```

Oder: `npx claude-mem install`

## Verwendung / الاستخدام

- **Claude Code:** Repository klonen und `claude` im Ordner starten — die Skills stehen sofort bereit.
- **Claude AI (claude.ai):** Einen Skill-Ordner aus `.claude/skills/` als ZIP packen und unter *Einstellungen → Funktionen → Skills* hochladen. claude-mem funktioniert nur in Claude Code.

## Lizenzen

Jeder Skill enthält seine eigene `LICENSE.txt`; siehe auch `.claude/skills/THIRD_PARTY_NOTICES.md`. claude-mem steht unter der Apache-2.0-Lizenz und wird hier nur referenziert, nicht mitgeliefert.
