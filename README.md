# baselayer

Methodology substrate for agent-driven software development.

A growing collection of skills, rules, standards, and agent
definitions that make AI coding agents less frantic and more
deliberate — pulled from real work on real systems, curated for
re-use.

## What this is

Four kinds of content, each addressing a different layer of how
an agent behaves during a software development task:

- **Skills** — invocable workflows the agent runs on request or
  at named moments. E.g., a pause-and-think gate before a
  non-trivial change.
- **Rules** *(coming)* — contextual guidance the agent loads
  automatically. No invocation required; they shape behavior in
  the background.
- **Standards** *(coming)* — reference documents the agent and
  operator share. The "how we do things here" layer.
- **Agents** *(coming)* — role definitions for specialized work
  (reviewer, architect, builder, etc.) used in multi-step or
  multi-agent setups.

Each category lives in its own directory with a README explaining
the concept and what's published so far.

## What's here today

- **[skills/temperance](skills/temperance/SKILL.md)** — a
  pause-and-think gate that asks two questions every other
  governance mechanism misses: *Am I building the right thing?*
  and *Am I building it the right way?* Fires before non-trivial
  work.

## What's coming

More skills will land incrementally as they're proven in real use
and sanded down for public consumption. The four top-level
directories (`skills/`, `rules/`, `standards/`, `agents/`)
already exist to signal the shape — their READMEs describe what
each layer does and what's queued.

No roadmap commitments, no release calendar. When a piece of the
substrate has earned its keep privately and is genuinely
re-usable, it lands here.

## How to use

Designed primarily for use with
[Claude Code](https://claude.com/claude-code), but the content is
plain markdown and nothing is platform-locked.

### With Claude Code

Clone this repo, then symlink the skill into your project:

```bash
git clone https://github.com/kingofrock/baselayer.git ~/src/baselayer
ln -s ~/src/baselayer/skills/temperance ~/my-project/.claude/skills/temperance
```

Claude Code auto-discovers skills under `.claude/skills/`; once
symlinked, you can invoke `/temperance` in any session in that
project.

### Without Claude Code

The SKILL.md files are structured markdown with a frontmatter
block. They read naturally as documentation — pull the checklist,
the invocation cues, the decision format, and adapt.

### Cherry-picking

Nothing in this repo requires the rest of it. Each skill, each
rule, each standard is a standalone piece you can lift into your
own workflow. If you want the full methodology, read multiple
pieces and compose them; the pieces are designed to compose but
work alone.

## Relationship to baselayer-private

This repo is a curated, de-internalized subset of a private
companion repo (baselayer-private) where these ideas get worked
out against real projects. The private side contains
project-specific context, session records, and work-in-progress
that isn't generally useful.

Direction is one-way: private → public. Nothing from this public
repo flows back into the private one automatically. When
something here gains traction and earns a place in the
foundation, it's because it proved itself first in private.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Short version: issues and
discussion are welcome; PRs are welcome on the content that's
already published. Proposals for new skills/rules/standards
should open an issue first so we can talk about fit before you
write anything.

## License

MIT. See [LICENSE](LICENSE).

## Who's behind this

Built by **Sanjay Pandey** —
[GitHub](https://github.com/kingofrock) ·
[LinkedIn](https://www.linkedin.com/in/sunjaypandey/)

Curated from real work on real projects.
