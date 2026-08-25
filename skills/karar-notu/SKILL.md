---
name: "karar-notu"
description: "Bir karar için yapılandırılmış karar notu üretir — seçenekler, ödünleşimler, kriterler, tavsiye ve geri dönüş planı. \"Karar vermem lazım\", \"A mı B mi\", \"hangisini seçmeliyim\", \"artı eksi çıkar\", \"karar notu yaz\" dendiğinde kullan. Also triggers on \"I need to decide\", \"A or B\", \"which one should I pick\", \"help me weigh these options\", \"write me a decision memo\". Kararın dayandığı dış veriyi sıfırdan toplamak için kullanma; onun için deep-research kullan."
---

# Decision memo

The aim is not to **make** the decision. It is to make the right decision
visible on its own.

## 1. Frame the decision — the step that matters most
- **What is the real question?** Under most "A or B" questions sits a badly
  framed one. "Which CRM should we buy" may actually be "what is broken in our
  sales process".
- By when? What does delay cost?
- **Is it reversible?** Reversible decisions get made fast; long analysis on them
  is waste. Say so explicitly.
- Who is affected, and who has to approve?

Do not move on to options until these are settled.

## 2. Set the criteria BEFORE the options
Three to five criteria, weighted. Writing criteria after seeing the options is
fitting the test to the answer you already want. Do not break the order.

## 3. Lay out the options
- At least three. If two are already being discussed, you find the third.
- **"Do nothing" is always an option** — evaluate it every time.
- For each: what it requires (money, time, people), what it gains, what the risk
  is, how hard it is to undo.

## 4. Weigh them honestly
Write each option in its **strongest form** — do not weaken one so it is easy to
beat. Mark what you do not know. Ask "what information would reverse this
decision?" and write that down.

## 5. Write it

```markdown
# Decision: <one sentence>
**Status:** draft | decided
**Date:** | **Owner:** | **Reversible:** | **Deadline:**

## Context  (why now? 3-5 sentences)

## Criteria
| # | Criterion | Weight | Why it matters |

## Options
### A) <name>
What it means: | Pros: | Cons: | Cost: | Risk:
### B) ...
### C) Do nothing

## Comparison
| Criterion | A | B | C |

## Recommendation
**<option>** — because <the 1-2 reasons that actually decide it>.

## What would change this recommendation
## What we do not know
## Fallback plan  (what we do if it turns out wrong, and the signal that tells us)
## Next steps
- [ ] who / what / when
```

If it runs long, write it to a file (`decisions/YYYY-MM-DD-<topic>.md`) and put
the summary in the conversation.

## Rules
- **Do not dodge the recommendation.** "It depends" is useless. Give your
  recommendation and show your reasoning; the user is free to reject it.
- Do not write with more certainty than the evidence carries.
- On a financial or legal decision: give information, do not make the decision,
  and note where professional advice is required.
