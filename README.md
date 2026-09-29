# Business Planner

**Business Planner is a free, open-source bundle of six Claude skills that plans, validates and stress-tests physical or offline businesses.** It interrogates your idea instead of writing it up, and every engagement ends in a GO, NO-GO, PIVOT or PILOT decision.

MIT licensed. Works for a solo side-business, a single shop, an MSME, or a funded startup.

```
/plugin marketplace add diligent-dilettante/business-planner
/plugin install business-planner
```

## What it does

Most AI tools act as a scribe: you describe an idea, they produce a polished plan. This one acts as the advisor who kills the idea in ten minutes so you don't spend six months on it.

It opens with five blunt questions. Does anyone want this. Can one unit make money. Can you reach the buyer. Is there a rule that ends it on day one. Would it matter to you if it worked. An idea that dies there cost you ten minutes.

What survives gets interviewed section by section. Unit economics cannot be skipped. Every number carries a tag: `sourced`, `founder-supplied`, or `estimate`. Override a warning and it records your reason and moves on. Correct a fact and it takes your word, because you know your market and it does not.

Then the plan gets rehearsed against a synthetic customer panel and a competitor wargame, and turned into documents you can actually run: a strategy doc, a 90-day operating plan, and an investment card.

## Who it is for

Physical and offline businesses at any scale. Solo operators, shops, MSMEs, D2C brands, retail, food, services, manufacturing, funded startups.

Ambition is set by you, not assumed. The skill calibrates to Livelihood, Growth or Venture, and applies the same standard of rigour to each with different scope. Any business returning more than your cost of capital, including your own time, is a real business. A solo operator clearing a good living is succeeding.

## The six skills

| Skill | Role | What it does |
|---|---|---|
| **business-planner** | Controller | Interview-driven plan builder with two tracks: **A: New Business** (idea to validation to strategy to launch) and **B: Scale / Grow** (an existing business expanding). Grills section by section with web research, named frameworks and bias checks before locking anything. Orchestrates the five sub-skills. |
| **founder-fit** | Sub-skill | Profiles whoever is actually executing: conviction, domain expertise, willingness to learn, skills, network. Maps each plan area to **run confidently / de-risk / get help**, with the trade-offs stated. |
| **market-sim** | Sub-skill | The customer stack. Rehearses the plan against a synthetic panel for any customer type: B2C, B2B buying committees, B2G tenders, B2B2C channel plus end-consumer. Objections, willingness to pay, segment and role splits. Sits at the bottom of the evidence ladder, so output is capped, ranked hypotheses, each paired with a real test. |
| **competition-sim** | Sub-skill | An adjudicated wargame with the customer as referee rather than 1-v-1 combat. Drafts competitor profiles that you correct *before* any simulation runs, then plays your moves against threshold-triggered reactions. Indifference is the base case. Outputs are tells to watch, never predictions. |
| **strategy-ops** | Sub-skill | Turns the surviving plan into run-documents: a **Strategy Doc** (Rumelt kernel, scenarios, tripwires), an **Operating Plan** (90-day OKR-lite cadence), and an **Investment Card** (money and time in, payback, NPV at your real discount rate, IRR by scenario, drawdown, reversibility) that makes any two ideas comparable. |
| **whisper** | Background watcher | A quiet senior advisor in surveillance mode across the whole flow. Watches for documented success and failure patterns, book mechanisms matching your moment, cross-section biases and sniff-test failures. Speaks in two labelled sentences under a soft budget, holds mandatory precedent checkpoints at the competition and GTM locks, and takes auditor or red-team roles inside the sims. Silence is its default, and "nothing fits" is an honest answer. |

## How it thinks

**Grill, research, framework and bias check, lock.** No section closes on vibes.

**It ends in a decision, not a document.** Every engagement resolves to GO / NO-GO / PIVOT / PILOT, plus the single riskiest assumption and one cheap dated next step. Planning that never decides is procrastination.

**Skeptical on irreversible bets, biased to action on reversible ones.** For 0-to-1 founders, over-planning kills as surely as under-planning. Sim depth scales to what is about to be spent, findings are capped, and every finding arrives with a move attached.

**Frameworks by name.** Zero to One, Lean Startup, Jobs to Be Done, The Mom Test, Dunford positioning, Seven Powers, Bullseye, $100M Offers, Profit First, cost of capital, E-Myth. Cited so you learn the lens rather than just the answer.

**Bias engine.** Planning fallacy, sunk cost, confirmation, survivorship, anchoring, narrative. Plus two the literature tends to miss: *scale bias*, assuming venture-scale is the only valid outcome, and *lifestyle dismissal*, under-planning a small business because it seems small.

**Evidence ladder.** Simulation sits under stated interest, which sits under interviews, which sit under smoke tests and pre-orders. Sims generate hypotheses. Real customers settle them, and the skill says so every time it runs one.

**Stories, in a testable template.** Customer, founder and stakeholder stories captured as *As a… when… I want… so that… and I'd…*, each tagged `assumed` / `sim-tested` / `evidence`. Your hard DOs and DON'Ts get captured up front as binding guardrails. A physical business fails on three surfaces: the customer won't buy, the founder can't execute, or a supplier, landlord, funder or regulator breaks the chain. Each gets a story the plan is accountable to.

**Precedent, including the failures.** Draws on how physical businesses actually succeeded and failed in India and comparable economies, always separating the transferable lesson from luck and context.

**India-aware.** For India-based plans it cuts the market thirty ways (economic class India1/2/3, city tier, generation, digital and channel behaviour, values, category behaviour) to force a precise beachhead instead of "all of India". Each city tier is treated as its own microcosm, so you pick a city rather than a tier. South India is treated as a distinct bloc: highest per-capita consumption, vernacular-first across Tamil, Telugu, Kannada and Malayalam, strong regional retail champions. Every age is treated as a market, from millennials at peak earnings to the under-served silver economy to values-gated Gen Z. It also carries the margin traps that kill Indian physical businesses: GST 2.0, inverted-duty ITC, working capital. Tuned for 0-to-1 businesses targeting roughly ₹8 to 17 crore.

**MSME and Venture both get a real path.** Livelihood founders get concise, jargon-light output and a setup on-ramp (Udyam, GST, FSSAI). Venture founders get a fast-pass plus fundraising sequence, dilution maths, VC criteria and the strategic-acquirer exit landscape. Capital sources are mapped for each: Mudra, CGTMSE, gold loan and TReDS on one side, angel to seed to Series A on the other. The upward scale challenge ("this could be Venture, here is what it costs") is offered, never pushed.

## Install

**Claude Code (plugin):**

```
/plugin marketplace add diligent-dilettante/business-planner
/plugin install business-planner
```

**Claude Desktop or Claude.ai:** upload the skill folders under **Settings → Capabilities → Skills**, or add them to a Project's knowledge. Each skill's description stays under the 1024-character limit.

**Any other agent that supports skills:**

```bash
git clone https://github.com/diligent-dilettante/business-planner.git
cp -r business-planner/plugins/business-planner/skills/* .agents/skills/
```

## Usage

Describe what you're doing. The controller picks the track and pulls in sub-skills as it needs them.

> *"I want to start a furniture brand selling online. Is it worth it?"*
> Planner on Track A, founder-fit once the bet locks, market-sim to rehearse price and positioning.

> *"My bakery does well locally. Should I add a second product line?"*
> Planner on Track B.

> *"We want to export to the UAE."*
> Planner plus the domestic-to-international conversion.

> *"What does Hooked actually tell me to do for my subscription box?"*
> whisper.

You can also call a sub-skill directly: *"assess my founder-market fit for X"*, *"rehearse this offer against my target market"*, or *"how did a business like mine actually get built?"*

## FAQ

### Is it free?

Yes. MIT licensed and open source. No account or API key beyond the Claude access you already have.

### How is this different from asking Claude or ChatGPT for a business plan?

A plain chat defaults to agreeable and will produce an optimistic plan for any idea you hand it. This runs the kill screen first, makes unit economics and financials non-skippable, tags the provenance of every number, applies named frameworks and bias checks before locking each section, and refuses to end without a decision.

### Does it work outside India?

Yes. The method is country-neutral: kill screen, unit economics, evidence ladder, framework and bias checks, simulations. The India reference files covering GST, Udyam, MSME capital sources and city-tier segmentation load only when the plan is India-based.

### Does it only work for startups?

No. It was built for physical businesses of any ambition, and it explicitly checks for *scale bias*. A shop clearing a lakh a month is a good business, and the skill will tell you so rather than pushing you to raise.

### What does it actually produce?

A business plan document, a Strategy Doc with scenarios and tripwires, a 90-day Operating Plan, and an Investment Card showing money and time in, payback, NPV at your real discount rate, IRR by scenario, drawdown and reversibility. The Investment Card is what lets you compare two unrelated ideas. Every engagement also resolves to a decision, the riskiest assumption, and one cheap dated next step.

### Can I use it on a business I already run?

Yes, that is Track B. It handles expansion, a second product line, a new geography, or a channel shift.

### How long does an engagement take?

The kill screen is ten minutes. A full plan with simulations and run-documents is a few sessions, and depth scales to how much money is about to move.

## Repository layout

Canonical skill source lives under `plugins/business-planner/skills/`. Earlier duplicate copies at the repo root and under `/skills/` have been removed. Do not add skill files anywhere else.

```
.
├── .claude-plugin/
│   └── marketplace.json
├── marketplace.json
├── plugins/
│   └── business-planner/
│       ├── .claude-plugin/
│       │   └── plugin.json
│       └── skills/
│           ├── business-planner/          # controller
│           │   ├── SKILL.md
│           │   └── references/
│           │       ├── frameworks.md
│           │       ├── business-plan-template.md
│           │       ├── financial-model-spec.md
│           │       ├── domestic-to-international.md
│           │       ├── india-market-context.md
│           │       ├── india-segmentation.md        # 30 market cuts
│           │       ├── india-regional-tiers.md      # tier microcosms, South India, Vizag
│           │       ├── india-consumption-by-age.md  # how each generation buys
│           │       ├── india-capital-landscape.md   # MSME schemes, VC stages
│           │       ├── venture-track.md             # raise, dilution, exit
│           │       ├── msme-setup.md                # Udyam / GST / FSSAI on-ramp
│           │       ├── correction-log.md
│           │       ├── handoff-template.md
│           │       └── stories.md
│           ├── founder-fit/
│           │   └── SKILL.md
│           ├── market-sim/                # B2C / B2B / B2G / B2B2C
│           │   └── SKILL.md
│           ├── competition-sim/           # adjudicated wargame
│           │   └── SKILL.md
│           ├── strategy-ops/              # strategy doc, operating plan, investment card
│           │   ├── SKILL.md
│           │   └── references/
│           │       └── strategy-ops-templates.md
│           └── whisper/
│               ├── SKILL.md
│               └── references/
│                   ├── case-library.md
│                   └── book-library.md
├── README.md
└── LICENSE
```

## Related open-source skills

market-sim is a lightweight rehearsal built into planning. For heavier standalone market simulation:

- **crowdcast**, `github.com/TheQmaks/crowdcast`, multi-agent social simulation with zero dependencies.
- **claude-persona**, `github.com/takechanman1228/claude-persona`, structured persona panels informed by Microsoft's TinyTroupe.

Method credit for the simulation approach goes to Stanford's Generative Agents (Park et al., 2023) and Social Simulacra. This bundle borrows the method rather than the code, and stays honest about where simulation sits on the evidence ladder.

## License

MIT. Use it, fork it, adapt it.
