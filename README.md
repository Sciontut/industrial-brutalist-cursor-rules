# industrial-brutalist-cursor-rules

A Cursor rule for industrial / brutalist / tactical-telemetry design. Drop the `.cursor/` directory into any project and the rule becomes available to Cursor's agent.

## What's here

```
.cursor/rules/
  industrial-brutalist-ui.mdc
```

## Activation

The rule uses `alwaysApply: false` with a `description`, so Cursor's agent loads it when your prompt signals **industrial / brutalist / tactical-telemetry** work — and stays out of unrelated tasks. To force it always-on, set `alwaysApply: true`; to scope by file type, add a `globs:` list.

## Source

Converted for Cursor from the `brutalist-skill` (frontmatter name `industrial-brutalist-ui`) in [hamzafarooq/claude-code-starter](https://github.com/hamzafarooq/claude-code-starter/tree/main/.claude/skills/brutalist-skill). Design prose preserved verbatim.
