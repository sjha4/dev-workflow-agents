# Skills

Custom skills (slash commands) for Claude Code.

## What are Skills?

Skills are custom commands that extend Claude Code's capabilities. They're invoked with a slash command like `/myskill` and can accept arguments.

## Structure

Each skill should be a separate file with the `.md` format:

```markdown
---
name: skill-name
description: Brief description of what the skill does
---

# Instructions for Claude

Your skill implementation here...
```

## Installation

1. Copy skill files to `~/.claude/skills/`
2. Or reference them in your project's `.claude/settings.json`:

```json
{
  "skills": [
    "path/to/skill.md"
  ]
}
```

## Creating New Skills

1. Create a new `.md` file
2. Add frontmatter with `name` and `description`
3. Write clear instructions for Claude
4. Test with `/skill-name` in Claude Code

## Examples

See the files in this directory for examples of useful skills.
