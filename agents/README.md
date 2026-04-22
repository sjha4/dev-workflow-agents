# Agent Definitions

Custom agent definitions and configurations for specialized workflows.

## What are Agents?

Agents are specialized Claude instances that can be spawned for specific tasks. They can have:
- Custom system prompts
- Specific tool access
- Dedicated model configurations
- Isolated contexts

## Structure

Agent definitions should include:
- Agent type configuration
- Available tools
- System instructions
- Use case documentation

## Configuration

Agents can be configured in `.claude/settings.json`:

```json
{
  "agents": {
    "my-custom-agent": {
      "description": "Agent description",
      "model": "sonnet",
      "tools": ["Read", "Write", "Bash"],
      "prompt": "Custom system prompt..."
    }
  }
}
```

## Creating New Agents

1. Define the agent's purpose and capabilities
2. Specify required tools
3. Write clear system instructions
4. Document when to use the agent
5. Test with various scenarios

## Examples

See the files in this directory for examples of specialized agents.
