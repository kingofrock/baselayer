# skills

Invocable workflows. Skills are things the agent *does* on request
or at named moments — a structured procedure with clear triggers,
inputs, and outputs.

Invoked by name (e.g., `/temperance`) in Claude Code, or adapted
as prompts/instructions in other agent frameworks.

## Published so far

| Skill | Purpose | Fires |
|-------|---------|-------|
| [temperance](temperance/SKILL.md) | Pause-and-think gate before non-trivial work | Before building |

## Installing

Each skill is self-contained under its own directory with a
`SKILL.md`. To use with Claude Code, symlink into your project:

```bash
ln -s /path/to/baselayer/skills/temperance .claude/skills/temperance
```

Claude Code auto-discovers skills under `.claude/skills/`. No
other wiring required.

## Anatomy of a skill

Each `SKILL.md` has:

- **Frontmatter** — name, description, whether it's
  user-invocable, whether the model can invoke it automatically
- **When to invoke** — the triggers that should fire the skill
- **Procedure** — the structured steps
- **Output format** (where applicable) — what the skill produces

## What makes something a skill vs a rule

**Skills** are explicitly invoked. The agent (or you) says "run
this now." They produce structured output.

**Rules** (see [rules/](../rules/)) load contextually in the
background. The agent reads them but doesn't "run" them.

A useful heuristic: if you'd put a slash command in front of it
(`/foo`), it's a skill. If it's "the way things are done here,"
it's a rule or standard.
