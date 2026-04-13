# rules

Contextual guidance loaded automatically. Rules shape agent
behavior without being explicitly invoked — the agent reads them
as background context when relevant work begins.

## Published so far

None yet. Rules will land here as they're de-internalized from
baselayer-private.

## What rules look like

A rule is a short markdown file with:

- **Frontmatter** specifying when it loads (globs, triggers, or
  "always")
- **The rule itself** — direct prose, often with bulleted dos
  and don'ts
- **Why the rule exists** — usually a specific incident or
  pattern that justified codifying it

Rules are deliberately short. If a rule starts to feel like a
standard (reference content, decision records, detailed
procedures), it probably belongs in [standards/](../standards/)
instead.

## What makes something a rule vs a skill

**Rules** are contextual. Loaded silently when relevant files
are open. Don't have an invocation.

**Skills** (see [skills/](../skills/)) are invoked on request
or at named moments.

Rule → "don't do X when editing Y"  
Skill → "when I say `/foo`, do these steps"
