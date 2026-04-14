# Contributing to KIBORU

Thanks for wanting to contribute! Here's how.

## Adding a New Agent

1. Create a folder under `agents/your-agent-name/`
2. Add a `SOUL.md` using the template below
3. Submit a pull request

### SOUL.md Template

```markdown
# [NAME] — [Role] Agent

## Identity
[Describe the agent's personality and character]

## Role
[What does this agent specialize in?]

## Capabilities
[List what it can do]

## Output Format
[How should it format responses?]

## Rules
[Any constraints or guidelines]

## Communication Style
[Tone, length, format preferences]

## Routing
[When to pass tasks to other agents]
```

## Submitting an Agent Pack

An agent pack is a collection of 3-6 agents focused on a specific niche.

1. Create a folder: `packs/your-pack-name/`
2. Add a `pack.md` describing the pack
3. Add each agent's `SOUL.md` inside the folder
4. Submit a pull request

## Guidelines

- Keep SOUL.md files clear and specific
- Test your agent before submitting
- One agent per pull request
- English only for agent instructions (for consistency)
