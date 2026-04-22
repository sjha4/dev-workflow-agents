# Development Workflow Agents

A collection of skills, commands, agent definitions, and automation tools for Claude Code.

## Structure

```
dev-workflow-agents/
├── skills/          # Custom Claude Code skills (slash commands)
├── agents/          # Custom agent definitions and configurations
├── mcp-servers/     # Model Context Protocol server configurations
├── hooks/           # Pre/post execution hooks for Claude Code
├── templates/       # Reusable templates for common tasks
└── scripts/         # Automation scripts and utilities
```

## Quick Start

### Installing Skills

Copy skill files from `skills/` to `~/.claude/skills/` or reference them in your Claude Code settings.

### Using Agent Definitions

Agent definitions in `agents/` can be referenced in your projects or added to your Claude Code configuration.

### Setting Up MCP Servers

Follow the instructions in `mcp-servers/README.md` to configure MCP servers in your Claude Code settings.

### Using Hooks

Copy hook scripts from `hooks/` and configure them in `~/.claude/settings.json`.

## Contributing

When adding new items:
1. Place them in the appropriate directory
2. Include clear documentation
3. Add examples where applicable
4. Update the relevant README

## License

See LICENSE file for details.
