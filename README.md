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

**What is actually built** is the Done section of [BACKLOG.md](BACKLOG.md).
Everything under Queue is planned and does not exist yet. The daily loop builds
one item a day; the table above is the intended shape, not the current state.

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

## Planned contents

Nothing here is built yet. This table is the intended shape, and the daily loop
fills it in one item at a time.

| # | Skill | What it does |
| --- | --- | --- |
| 001 | [frame-the-question](skills/frame-the-question) | Establish what is actually being asked before anything is analysed. |
| 002 | [hypothesis-tree](skills/hypothesis-tree) | Break a question into claims that could each turn out false, ranked by how much the answer moves if they do. |
| 003 | [evidence-plan](skills/evidence-plan) | For each claim, what would settle it, where that evidence lives, and what to do when it does not exist — which is the common case and the one most plans skip. |
| 004 | [market-entry-assessment](skills/market-entry-assessment) | Size, structure, competitive response and the cost of being wrong, with the entry decision expressed as what would have to be true. |
| 005 | [competitive-response](skills/competitive-response) | Model what the incumbent does next, since a strategy that assumes no response is a plan for a market with one participant. |
| 006 | [recommendation-memo](skills/recommendation-memo) | Write the recommendation so the reasoning is auditable: the claim, the evidence, the strongest case against, and what would change the answer. |
| 007 | [workshop-design](skills/workshop-design) | Design a session that produces a decision rather than a shared document, including what to do when the decision-maker is not in the room. |
| 008 | [stakeholder-map](skills/stakeholder-map) | Who has to agree, who can block, what each one is optimising for, and which of those are in genuine conflict. |
| 009 | [pre-mortem](skills/pre-mortem) | Assume the recommendation was taken and failed. |

## Licence

MIT. See [LICENSE](LICENSE).
