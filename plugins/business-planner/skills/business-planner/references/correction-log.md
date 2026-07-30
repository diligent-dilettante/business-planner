# Correction Log

**Records where the ANALYST was factually wrong and the founder corrected it.**

Distinct from the Override Log, which records the founder overriding a *warning* — a judgement call where both parties see the same facts and weigh them differently.

This log records something else: the analyst had a **fact** wrong, and the founder knew better.

---

## Why this exists

Every challenge mechanism in this skill points one way — the analyst interrogates the founder's assumptions. There is no path for the reverse.

That is backwards for an entire class of input. On local facts — prices, supply, regulation, customer behaviour, anything observable on the ground in their own market — **the founder knows and the analyst infers.** Inference loses.

Worse, analyst errors are often **silent**. A misread unit, a cost treated as a loss when it is a gain, a take-up rate borrowed from the wrong reference market. None of these surface through challenging the founder's assumptions, because they are not the founder's assumptions. They sit in the model unexamined until someone with ground knowledge happens to look at the right number.

---

## The log

| Date | What the analyst had | Founder's correction | Basis of their knowledge | Impact on the model |
|---|---|---|---|---|
| 2026-07-30 | Repo lacks `competition-sim` and `strategy-ops`; content triplicated across three paths | Both skills present on `main` at v3.0.0. Reviewer cloned default HEAD, not `main` | Repo owner has direct access to `main` | Invalidated Branch 2's premise and part of Branch 1's. Review's behavioural critique stands; its repo-state claims do not |
| 2026-07-30 | Commit 2762e4b landed on `main` under message *"v3.1.0: engagement-review fixes + correction merge (correct tree)"* — the tree it carried was v2.9.3 | Stale local zip; the intended v3.1.0 tree was never inside the archive that got expanded on the founder's machine | Founder verified via API at head SHA and via the recursive git tree | Superseded by 8c23836 ("verified tree"). The correction log's own push history now demonstrates its lesson: verify the tree, not the commit message |

**Fill the fourth column honestly.** "They operate in this market" is weaker evidence than "they have a screenshot of the competitor's booking page." Both are better than analyst inference, but knowing which you have matters when the correction is later questioned.

---

## Behavioural rules for the controller

**When the founder corrects a factual input:**

1. **Do not defend the prior figure.** The instinct to explain where the number came from is a waste of the founder's time and signals that corrections are unwelcome.
2. **Restate the correction and quantify its effect.** "That moves Year-3 EBITDA from X to Y" — so the founder can see whether their correction mattered.
3. **Check what it invalidates downstream.** A corrected unit price may break a break-even calculation three sections earlier. Trace it.
4. **Log it here.**

**Ask directly, every few sections:**

> "Is anything I've assumed obviously wrong to you? You know this market and I don't."

This is the highest-yield question in the flow. Founders will not volunteer corrections to an analyst who seems confident — they assume the number came from somewhere. Asking gives permission.

**Watch for the correction that arrives as an aside.** Founders frequently correct a major input in passing, inside a sentence about something else. "Oh, that price is per half-hour by the way" is a 50% error in the competitive benchmark delivered as a footnote. Catch these; they rarely get repeated.

---

## What belongs here vs the Override Log

| | Correction Log | Override Log |
|---|---|---|
| **What happened** | The analyst had a fact wrong | The analyst raised a warning, the founder proceeded anyway |
| **Who was right** | The founder | Unresolved — it is a judgement |
| **Example** | "That rate is per session, not per hour" | "I know the window is 12–18 months. Going independent anyway" |
| **What it changes** | The model | Nothing in the model — it records accepted risk |

If a correction turns out to be a judgement in disguise — the founder asserting a number they hope is true rather than one they know — it belongs in the Override Log instead, tagged as an assumption the founder owns.
