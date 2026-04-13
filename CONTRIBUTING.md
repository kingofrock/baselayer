# Contributing

This is a curated, opinionated substrate — not a crowdsourced
collection. Contributions are welcome; scope boundaries are tight
on purpose.

## What belongs here

- **Refinements to published content** — typo fixes, clearer
  phrasing, corrections, additional examples
- **Proposals for new skills/rules/standards** via issue first,
  code second
- **Cross-platform adaptations** — if a skill assumes Claude
  Code and you've made it work with another agent framework,
  open an issue and let's talk about how to generalize

## What doesn't

- Generic agent-framework plumbing (this isn't a framework;
  it's methodology)
- Opinion-based style changes without rationale
- Content that assumes the reader has access to private
  companion material (this repo must stand alone)

## Proposing a new skill/rule/standard

Open an issue before writing. Include:

- **What it does** (one sentence)
- **When it fires** (the moment in a workflow where it
  triggers)
- **What it replaces or augments** (if something adjacent
  already exists)
- **Evidence it earns its keep** — concrete incidents or
  workflows where this would have helped

Proposals without a specific problem getting solved are
usually not a fit — the bar for adding to the foundation is
"this has earned its place in my real work for months" not
"this seems like a good idea."

## Pull requests

- One logical change per PR
- Include a short explanation in the description of what
  shifted and why
- Keep the existing voice — direct, specific, no marketing
  hedge
- If you're modifying a skill/rule/standard, update the
  [CHANGELOG](CHANGELOG.md) with a dated entry

## Issue templates

For now, issues are free-form. Templates will land when the
volume warrants them.

## Provenance note

Published content here is curated from baselayer-private, a
companion repo not open to external contributions. Accepted
public contributions do not flow back into the private side —
direction is one-way. By contributing, you're contributing to
this public repo only, not to any private work.
