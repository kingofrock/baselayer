# agents

Role definitions for specialized work. Agents are named
personas with scoped responsibilities — reviewer, architect,
builder, etc. — used in multi-step or multi-agent workflows.

## Published so far

None yet. Agent definitions will land here as they're
de-internalized from baselayer-private.

## What agents look like

An agent definition is a markdown file that establishes:

- **Role** — what this agent is responsible for
- **Capability ceiling** — what it can and cannot do
- **Inputs** — what it expects to receive when invoked
- **Outputs** — what it produces
- **Escalation rules** — when it should kick back to a
  human or another agent
- **Luminaries** *(where applicable)* — the thinkers whose
  principles the agent operates through

## What makes something an agent vs a skill

**Agents** are long-lived personas with scope. They maintain
a point of view across multiple tasks.

**Skills** (see [skills/](../skills/)) are procedures. Any
agent can invoke any skill.

Agent → "the reviewer, with reviewer judgment"  
Skill → "the verify procedure, run by whoever"

Agents are most useful in multi-agent setups where different
specialists handle different parts of a workflow — separation
of concerns across roles rather than across procedures.
