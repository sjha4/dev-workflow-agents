# Hooks

Shell hooks for Claude Code automation and workflows.

## What are Hooks?

Hooks are shell commands that execute automatically in response to events like tool calls or user actions.

## Available Hook Types

- `user-prompt-submit-hook`: Runs when user submits a prompt
- `tool-call-hook`: Runs when specific tools are called
- `assistant-response-hook`: Runs after Claude responds

## Configuration

Hooks are configured in `~/.claude/settings.json`:

```json
{
  "hooks": {
    "user-prompt-submit-hook": "echo 'User submitted: $PROMPT'",
    "tool-call-hook": {
      "Bash": "echo 'Running bash command: $COMMAND'"
    }
  }
}
```

## Environment Variables

Hooks have access to:
- `$PROMPT`: User's prompt text
- `$COMMAND`: Tool command being executed
- `$TOOL`: Tool name being called
- `$CWD`: Current working directory

## Creating New Hooks

1. Identify the event to trigger on
2. Write the shell command
3. Test thoroughly (hooks can block Claude if they fail)
4. Document the hook's purpose and variables
5. Add to settings.json

## Examples

See the files in this directory for examples of useful hooks.

## Best Practices

- Keep hooks fast and non-blocking
- Handle errors gracefully
- Use absolute paths
- Test before deploying
- Document expected behavior
