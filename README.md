# strategy-agent

Agents and skills for management and strategy consulting work.

Strategy work fails at the framing far more often than at the
analysis. The question arrives already answered — "which market should we enter"
when the real question is whether to enter one at all — and everything
downstream is competent work on the wrong problem.

This repository holds the agents and skills for the parts that are genuinely
repeatable: framing the question so it can come out either way, breaking it into
claims that could be false, building the evidence to test them, and writing the
recommendation so that the reasoning survives contact with someone who
disagrees.

## What this is not

It is not a framework collection. A framework is a way of
organising an argument you already have, not a way of finding one, and a skill
that applies one uninvited is doing harm.

It does not make the decision. It makes the basis for the decision legible.

It is not a substitute for knowing the industry.

## How to use this

These are skills for Claude, not a command-line tool. There is nothing to
install and nothing to import — you describe the work and the matching skill
fires on its own.

**In Claude Code or Cowork**, once the skills are on your machine:

```bash
bash ~/Desktop/agent/_setup/sync-skills.sh
```

That clones every agent repository and links its `skills/` into `~/.claude/skills`,
so they are available in every session and every folder. Re-run it whenever the
daily loop ships something new — it pulls rather than re-clones.

Then simply ask. Each skill's `description` frontmatter is written to match how
the request actually gets phrased, in English or Turkish, so you do not name the
skill and generally should not have to think about which one applies.

**If nothing fires**, that is a defect in the skill rather than in how you
asked. The description was written for the wrong phrasing. Say what you asked
and what you expected, and it gets fixed — that feedback is more valuable than
working around it.

**What is actually built** is listed under Contents below and in the Done
section of [BACKLOG.md](BACKLOG.md). Everything under Queue is planned and does
not exist yet.

## Layout

```
agents/
  <name>.md           one specialist, its brief and its boundaries
skills/
  <name>/
    SKILL.md          the instruction, with triggering description frontmatter
    scripts/          only where deterministic code beats instruction
examples/
  <name>/             worked example on real input, with the output committed
```

## Roadmap

See [BACKLOG.md](BACKLOG.md). The first unchecked item is the one being built.

## Contents

| Skill | What it does |
| --- | --- |
| [karar-notu](skills/karar-notu) | Turn a decision into a written note: options, trade-offs, criteria, recommendation and the way back. |
| [offer-design](skills/offer-design) | Design or repair the thing being sold — value framing, guarantee, structure — before the copy that sells it. |

These arrived already written and in daily use, rather than being built against the queue below — which is why most carry no item number. Some have Turkish bodies: they were written in the language they are used in, and translating them is a queue item rather than a blocker.

Everything still under Queue in [BACKLOG.md](BACKLOG.md) does not exist
yet. The daily loop builds one item a day.
## Licence

MIT. See [LICENSE](LICENSE).
