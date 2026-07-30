---
name: competition-sim
description: Simulates how competitors, incumbents, and channels respond to a business plan's moves — as a multi-round wargame where the CUSTOMER PANEL is the referee, not the analyst. Drafts competitor profiles (founder reviews and corrects them BEFORE any simulation), then plays the plan's key moves across up to three rounds of move and counter-move, reallocating the market-sim panel by segment at each round and costing every move on both sides. Models indifference as the base case — most incumbents don't notice a small entrant for a long time. Use when pressure-testing a plan against competition, asking "what will the incumbent do when I launch / cut price / take their shelf space," identifying which moves trigger retaliation and which fly under the radar, or preparing counter-moves. Sub-skill of business-planner. Requires market-sim to have run first. Outputs capped, ranked findings each paired with a real-world tell to watch — hypotheses to monitor, never predictions.
---

# competition-sim

Plays a business plan's moves against the competitors who might respond, across up to three rounds — as **business, not war**. Competitors don't win by defeating you; they win by satisfying customers better. Combat framing produces macho nonsense; customer framing produces insight. (Method descends from adjudicated business wargaming — cf. IQTLabs Snow Globe's open-source umpire pattern — with that classic critique baked in.)

**The customer panel decides who wins each round — not the analyst.**

**Anti-paralysis:** depth scales to stakes — ask *"what are you about to spend?"* A week-2 instinct gets a light pass (opening move, one round); full three-round games are for when real money is about to be committed. Fear of instant retaliation paralyzes founders over a threat that rarely materializes at 0→1 scale.

## Prerequisites

**Do not run this before market-sim.** The panel from market-sim is the adjudication mechanism here. Without it you are substituting analyst judgement for customer behaviour, which is the exact failure this skill exists to prevent.

If market-sim has not run, say so and run it first.

---

## Step 1 — Draft competitor profiles

Cover four categories. Most plans forget at least two.

| Category | Examples |
|---|---|
| **Direct** | Same product, same customer |
| **Adjacent** | Different product, same occasion or budget |
| **Channel** | Distributors, platforms, landlords — anyone between you and the customer |
| **Do nothing** | The customer's current habit. Usually the strongest competitor and the most overlooked |

For each, state:

```
NAME · CATEGORY · GROUNDED or GUESSED

Position today       — what they sell, to whom, at what price
Capital position     — can they fund a response? Evidence, not assumption
Reaction threshold   — the specific, observable thing that would make them act
Expected timeline    — months until they could plausibly respond
Their likely move    — one sentence
Cost to them of that move — margin, cash, capex, attention, brand
```

**Ground every profile you can.** A competitor whose real prices you have observed is worth five you have imagined. Tag each `GROUNDED` or `GUESSED` and say what the grounding is.

**Indifference is the base case.** Most incumbents do not notice a small entrant for a long time, and many never respond at all. A profile that has everyone reacting is wrong. If a competitor has no plausible reaction threshold, say so and move on — that is a finding.

---

## Step 2 — GATE: founder corrects the profiles

**Show the profiles. Do not simulate until the founder has corrected them or explicitly accepted them.**

The founder knows things you cannot infer: who is actually well-capitalised, who is distracted, who has tried and failed before, who is related to whom. This is the single highest-value input in the skill.

Ask directly:

> "Where am I wrong about these? You know these operators and I don't."

If asked to skip this gate: state what it protects, then ask for explicit confirmation. Do not skip silently.

---

## Step 3 — Run the wargame

Three rounds maximum. Beyond three, uncertainty exceeds insight.

### ROUND 0 — Baseline

Allocate the market-sim panel across the founder and every existing alternative. Who is with whom today, and why.

```
| Actor (from market-sim) | Currently with | Why |
```

This is the board before anyone moves.

### ROUND 1 — The founder's opening move

State the move (launch, price, position, channel).

**Reallocate the panel by segment.** For each actor: do they move, and what specifically made them move or stay?

```
| Actor | Before | After | Reason |
```

**Then check triggers.** Does this move cross any competitor's stated reaction threshold — taking X% of a micro-market, appearing on their key shelf/platform, poaching a named account, undercutting a hero SKU? Name which competitor, and which threshold.

If nothing triggers, say so plainly and stop. **A move that provokes no response is a finding, not a failure** — it means you have room to operate.

### ROUND 2 — Competitor response

Only for competitors whose threshold was crossed.

```
Who responds        — and why this one and not the others
Their move          — specific
THEIR cost          — margin, cash, capex, attention, brand equity
Can they afford it? — reference their capital position from Step 1
```

**Reallocate the panel again, by segment.**

**Then generate the founder's counter-options.** Each one costed:

```
| Counter-option | What it costs | Funded from | What it forecloses |
```

**A response with no cost is not a response.** If every option looks free, the costing is wrong.

### ROUND 3 — The founder's counter

Pick the counter, or present two and let the founder choose.

Reallocate the panel a final time. State the net position.

Then: **their likely follow-up, and whether the game stabilises or escalates.** An escalating game with a better-capitalised opponent is a losing game — say so.

### BRANCH POINTS

Flag every place the path could plausibly diverge, each with **the observable tell** that distinguishes which branch you are in.

```
| Branch point | Path A | Path B | The tell that tells you which |
```

---

## Three hard requirements

**1. Panel continuity.** Adjudication uses the market-sim panel — the same actors, reallocating. If an actor is not in that panel, it cannot referee here. Introducing new actors mid-wargame is the analyst putting a thumb on the scale.

**2. Segment-level reallocation.** Never report a blended "you lose 25–35% of volume." State **which segments moved and why.**

> A price-led entrant takes price-sensitive triers and leaves committed regulars.
> A brand-led entrant takes status-motivated buyers and leaves the community-attached.
>
> **These are different threats requiring different counters. A blended percentage hides the decision.**

**3. Every move is costed, both sides.** Margin, cash, capex, management attention, brand equity. A simulation where responses are free will always recommend responding — which is how founders end up in price wars they cannot fund.

---

## Output

Cap at **five findings, ranked.** More than five and none get acted on.

Each finding:

```
FINDING          — one sentence
WHICH SEGMENT    — who moves, not how many
CONFIDENCE       — grounded / partly grounded / speculative
THE TELL         — the observable signal that this is actually happening
IF IT HAPPENS    — the pre-committed response, and what it costs
```

**Close with the heat map: moves that provoke nothing vs moves that poke the bear.** The quiet moves matter as much as the threatening ones — they are where the founder can act freely, and founders systematically overestimate how much attention they attract. This often reshapes sequencing: **win quiet niches first.**

**Feed back into the planner:** reactions → A3 (positioning), heat map → A7 (GTM sequencing), and every tell → strategy-ops as a tripwire monitor.

---

## Standing rules

**This is a hypothesis generator, not a forecast.** Every output is a thing to watch for, paired with a tell. Never present a simulated response as a prediction.

**Indifference is the base case.** Rebut it with evidence, not with imagination.

**The customer decides.** Not who has the better product, the better story, or the better plan — who the panel actually chooses, and why.

**Do not let the founder's plan win by default.** If the panel would move to a competitor, say so. A wargame the founder always wins has been run wrong.

**A competitor is not a monolith.** A lazy franchisee of an aggressive brand behaves lazily. Profile the local reality, not the head-office reputation.

**If a projected reaction contradicts the founder's confirmed local knowledge, the founder's knowledge wins** and the model's claim is retagged (see the Correction Log).

**This sim ranks below even customer simulation on the evidence ladder** — competitor intent is less observable than customer preference. Tells and monitors are the honest output, not forecasts.

**Never simulate beyond three rounds or short-term horizons** — long-range competitive arcs hallucinate (documented LLM-wargaming failure mode); hand them to strategy-ops scenarios and tripwires.

**Never recommend matching a price cut without costing it.** Matching is the most commonly recommended and most commonly fatal response. If it is the right answer, show the margin arithmetic that makes it so.
