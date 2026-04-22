# MCP Servers

Model Context Protocol server configurations and integrations.

## What is MCP?

MCP (Model Context Protocol) allows Claude Code to connect to external data sources and tools through standardized servers.

## Structure

Each MCP server configuration should include:
- Server setup instructions
- Configuration examples
- Available tools/resources
- Usage documentation

## Configuration

MCP servers are configured in `~/.claude/settings.json`:

```json
{
  "mcpServers": {
    "server-name": {
      "command": "node",
      "args": ["/path/to/server/build/index.js"],
      "env": {
        "API_KEY": "your-key"
      }
    }
  }
}
```

## Available Servers

Document your MCP servers here:

- **server-name**: Brief description
  - Tools: List of tools provided
  - Resources: List of resources provided
  - Setup: Link to setup instructions

## Creating New Server Configs

1. Document server installation steps
2. Provide configuration examples
3. List available tools and resources
4. Include usage examples
5. Note any dependencies or API keys needed

## Resources

- [MCP Documentation](https://modelcontextprotocol.io/)
- [MCP Servers Repository](https://github.com/modelcontextprotocol/servers)
