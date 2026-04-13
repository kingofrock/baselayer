# standards

Reference documents. The "how we do things here" layer — design
principles, architectural posture, engineering conventions, process
definitions.

## Published so far

None yet. Standards will land here as they're de-internalized from
baselayer-private.

## What standards look like

A standard is a longer-form markdown document that defines a
single topic in depth. Unlike rules (short, situational) or
skills (procedural), standards are reference material that
agents and operators consult when they need authoritative
guidance.

Examples of topics that might become public standards over time:

- Branching strategy
- Testing posture (what gets tested, how, why)
- Graceful exit (what an agent does when it hits an interruption)
- Engineering principles (the shape of good code in this context)

## What makes something a standard vs a rule

**Standards** are reference. Read when you need the full
treatment of a topic. Usually 200-400 lines.

**Rules** (see [rules/](../rules/)) are terse behavioral
guidance loaded automatically.

Standard → "here's everything about how we handle X"  
Rule → "don't do the thing that breaks X"
