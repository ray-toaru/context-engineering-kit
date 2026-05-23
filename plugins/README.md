# Context Engineering Kit Plugins

This directory contains hand-crafted plugins focused on improving agent result quality. Each plugin can include Claude Code metadata in `.claude-plugin/plugin.json` and Codex metadata in `.codex-plugin/plugin.json`.

## Plugin Structure

Each plugin should follow this structure:

```
plugin-name/
├── .claude-plugin/      # Claude Code manifest
├── .codex-plugin/      # Codex manifest
├── README.md           # Plugin documentation
├── commands/           # Slash commands (optional)
└── skills/            # Skills definitions (optional)
```

## Codex Plugin Manifest (.codex-plugin/plugin.json)

```json
{
  "name": "plugin-name",
  "version": "1.0.0",
  "description": "Brief description of what the plugin does",
  "author": {
    "name": "Your Name"
  },
  "skills": "./skills/",
  "interface": {
    "displayName": "Plugin Name",
    "shortDescription": "Short user-facing description",
    "longDescription": "Longer description for plugin details",
    "developerName": "Your Name",
    "category": "Coding",
    "capabilities": ["Read", "Write"],
    "defaultPrompt": ["Use this plugin for the current task"],
    "screenshots": []
  }
}
```

The repo-local Codex marketplace lives at `.agents/plugins/marketplace.json` and points to each plugin under `./plugins/<plugin-name>`.

## Getting Started

See [CONTRIBUTING.md](../CONTRIBUTING.md) for guidelines on creating plugins.
