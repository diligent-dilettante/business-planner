---
name: market-sim
description: >
  Rehearses a business plan against a synthetic customer panel — for ANY customer type: B2C
  (consumers), B2B (buying committees), B2G (government/tenders), B2B2C (distributor/platform +
  end consumer), or mixed. Each mode has its own actor model, buying logic, and objection
  patterns. Turns plan claims into testable "customer stories," runs them past the co-defined
  panel, and returns reactions, objections, willingness-to-pay, and segment splits — always as
  hypotheses at the BOTTOM of the evidence ladder, never proof of demand. Use when pressure-testing
  a product, offer, price, or positioning before spending, when the buyer is a business,
  government, or channel rather than a consumer, or to decide what to validate with real
  customers. Sub-skill of business-planner. Anti-paralysis by design: findings are capped,
  ranked, and each pairs with a cheap next move. Real customers (pre-orders, deposits, pilots,
  signed POs) settle everything.
---

# Market-Sim (Customer Stack)

Rehearse a plan against a **simulated customer panel — whatever kind of customer that is.** A "customer" may be a person, a purchasing committee, a government department, or a distributor with their own end-consumer. Each buys differently. This skill picks the right actor model, runs the plan's claims past it, and reports what held and what broke.

## The one rule that governs everything

**Simulation sits at the BOTTOM of the evidence ladder.** It generates hypotheses, surfaces objections, and stress-tests messaging cheaply. It is never validation.

```
Evidence ladder (weakest → strongest)
  1. Simulation / synthetic panel      ← this skill
  2. Stated interest ("sounds great")
  3. Structured interviews (Mom Test)
  4. Smoke test / fake door / pilot RFQ
  5. Pre-orders / deposits / signed POs / tender wins  ← "credit cards are the truth"
```

Every finding names **the real test one rung up** to run next. Never output a go/no-go from simulation alone.

## Anti-paralysis rules (always on)

A founder early in the journey has instinct and momentum; a wall of objections kills both. So:
- **Depth scales to stakes.** Ask: *"what are you about to spend?"* Week-2 instinct check → light pass (top 3 objections, one segment split). About to sign a lease / order inventory / raise → full pass. Never run the gauntlet on a sketch.
- **Max 3 "fix before spending" findings** surfaced; the rest go to an appendix, ranked.
- **Every finding pairs with a cheap move** that resolves it ("price resistance at ₹500 in segment B → 10-person WTP test this week"). Output is a to-do list, not a verdict.
- **Founder conviction is data, not bias.** Where a sim finding contradicts real domain instinct (per founder-fit), tag it "tension to test" — don't declare the founder wrong.
- Frame everything forward: scenarios and objections are *rehearsal for the future*, not homework before they're allowed to start.

## Step 1 — Identify the customer type(s)

| Mode | Who decides | Buying logic | Key dynamics |
|---|---|---|---|
| **B2C** | An individual/household | Need + emotion + price + trust | Discovery channel, WTP, repeat habit, social proof |
| **B2B** | A committee | ROI + risk + politics | Champion, economic buyer, end user, procurement, blocker — each needs a different story; long cycles; switching costs; "nobody got fired for buying the incumbent" |
| **B2G** | A department + rules | Compliance + price + relationship | Tender/L1 dynamics, GeM portal (India), spec-writing influence, payment delays (model 90–180 days), audit safety |
| **B2B2C** | Two customers | Channel margin AND end-demand | The distributor/retailer/platform needs margin + velocity + low hassle; the end consumer needs the product; their needs conflict — margin stacking, shelf-space logic, who owns the customer |

Mixed models are common (D2C + distributor + institutional) — run the relevant modes separately; don't average them.

## Step 2 — Build the panel (co-defined, written down)

Per mode: 2–5 named actor types, rough weighting, declared variation (price sensitivity, risk appetite, urgency, incumbency loyalty), and each actor's hot buttons and dealbreakers. For B2B/B2G, name the *roles in the deal* (champion, CFO, procurement officer, store owner), not just firmographics. Ground with anything real (existing customers, competitor reviews, tender archives, distributor conversations); mark `grounded` vs `guessed` — guessed panels are weaker evidence. **Grounding floor (hard requirement): at least one actor must be grounded in observed data — real prices, a real venue, a real conversation. If none is available, say so and ask for one before running; an entirely invented panel is the analyst's imagination with extra steps.** India plans: use the India1/2/3 and regional lenses from the planner's references.

## Step 3 — Customer stories

Pull existing stories from the Stories Ledger (`assumed` status) or draft new ones in the strict template — for any actor:
> *As a [actor], when [trigger], I want [job], so that [outcome], and I'd [observable action: buy at ₹X / issue a PO / list the SKU / bid / renew / walk].*

For B2B, write one story per committee role. For B2B2C, write both sides. 5–15 stories covering the load-bearing claims (demand, price, switching, repeat, channel adoption).

## Step 4 — Run and report

Actors react in character with memory across stories; represent declared variation (uniform answers = shallow panel warning). Adjudicate B2B/B2G deals as a *committee outcome*, not one persona's vote. Report:
- **Reaction per story** (accept / reject / conditional, by actor/segment) · **objections** (the gold) · **WTP / margin-required signal** · **segment & role splits** · **messaging that landed** · **confidence flags** (grounded vs guessed)
- **→ Top 3 fixes, each with its cheap real-world test** (mandatory), appendix for the rest.
- Upgrade run stories to `sim-tested` in the Ledger — never to `evidence`.

## Guardrails
- Synthetic reactions are convincing, not accurate; convincingness is the trap. Ungrounded panels reflect stereotypes.
- Worst at genuinely novel products and at predicting actual spend; best at objection discovery and message comparison.
- If sim and real customers disagree, real customers win. Always.

## Heavier standalone tools (credit + pointer)
For larger dedicated persona simulation: **crowdcast** (github.com/TheQmaks/crowdcast), **claude-persona** (github.com/takechanman1228/claude-persona; informed by Microsoft TinyTroupe). Method credit: Stanford Generative Agents (Park et al., 2023) & Social Simulacra. This skill borrows the method, keeps the evidence-ladder honesty, and extends it to B2B/B2G/B2B2C actor models.
