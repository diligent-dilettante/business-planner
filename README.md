# Business Planner

> **Canonical source is `plugins/business-planner/skills/`. Do not edit skill files elsewhere — earlier duplicate copies at the repo root and `/skills/` have been removed.**

Six orchestrated Claude skills for building and growing **physical / offline businesses** — at any scale of ambition, from a solo side-business to a local shop to a funded startup.

Grill-first, not a scribe. It interrogates the idea, applies proven business frameworks by name, checks for the cognitive biases that kill businesses, profiles the founder actually executing, rehearses the plan against a simulated market, and forces out a plan that survives contact with reality.

**Ambition-neutral by design.** Any business that returns more than your cost of capital — including your own time — is a real business. A solo operator clearing a good living is succeeding just as much as a venture-scale startup. The skill calibrates its rigor to *your* definition of a win, never to a default assumption of scale.

## The four skills

| Skill | Role | What it does |
|---|---|---|
| **business-planner** | Controller | Interview-driven plan builder. Two tracks — **A: New Business** (idea → validation → strategy → launch) and **B: Scale / Grow** (existing business expanding). Section-by-section grilling with web research, named frameworks, and bias checks before locking each section. Runs the five-phase plan → test → run flow and orchestrates the five sub-skills. |
| **founder-fit** | Sub-skill | Profiles the founder(s) — conviction, domain expertise, willingness to learn, hard/soft skills, network — and maps each plan area to **run confidently / de-risk / get help**, with the trade-offs made explicit. Supportive but honest. |
| **market-sim** | Sub-skill | The **customer stack**: rehearses the plan against a synthetic panel for ANY customer type — B2C, B2B buying committees, B2G tenders, B2B2C channel + end-consumer. Objections, WTP, segment/role splits. Bottom of the evidence ladder — capped, ranked hypotheses each paired with a real test. |
| **competition-sim** | Sub-skill | Adjudicated **business wargame** (customer as referee, not 1-vs-1 combat): drafts competitor profiles the founder corrects *before* any simulation, then plays the plan's moves against threshold-triggered reactions. Indifference modelled as the base case; outputs are tells to watch, never predictions. |
| **strategy-ops** | Sub-skill | Turns the surviving plan into run-documents: **Strategy Doc** (Rumelt kernel + scenarios + tripwires), **Operating Plan** (90-day OKR-lite cadence), and an **Investment Card** (money/time in, payback, NPV at the founder's real discount rate, IRR by scenario, drawdown, reversibility) that makes any two ideas comparable. Time = scenarios + tripwires, never long-range prediction. |
| **whisper** | Background watcher | case-library + book-advisor merged: a quiet senior advisor in surveillance mode across the whole flow. Watches for documented success/failure patterns, book mechanisms matching the founder's moment, cross-section biases, single-direction sizing, and sniff-test failures — speaks in two labeled sentences under a soft budget, holds mandatory precedent checkpoints at the competition and GTM locks, and takes auditor/red-team roles inside the sims. Silence is its default; "nothing fits" is an honest answer. |

## How it thinks

- **Grill → Research → Framework + Bias check → Lock.** No section closes on vibes.
- **Ends in a decision, not a document.** Every engagement resolves to GO / NO-GO / PIVOT / PILOT, the single riskiest assumption, and one cheap dated next step. Planning that never decides is procrastination.
- **Fast kill-screen first.** Four blunt questions (demand / economics / reach / showstopper) can kill a bad idea in ten minutes before months are sunk — and resequence the plan to attack the biggest risk first.
- **Holds both skepticism and action.** Skeptical on irreversible bets; biased to action on reversible ones. For 0→1 founders, over-planning kills as surely as under-planning.
- **Frameworks by name.** Zero to One, Lean Startup, JTBD, The Mom Test, Dunford positioning, Seven Powers, Bullseye/Traction, $100M Offers, Profit First, cost-of-capital, E-Myth, and more — cited so you learn the lens, not just the answer.
- **Bias engine.** Planning fallacy, sunk cost, confirmation, survivorship, anchoring, narrative, plus **scale bias** (assuming venture-scale is the only valid outcome) and **lifestyle dismissal** (underplanning a small business).
- **Founder-shaped.** The plan flexes to who's running it — lean into strengths, de-risk gaps, buy what you can't do in time.
- **Evidence ladder.** Simulation < stated interest < interviews < smoke test < pre-orders/POs. Sims generate hypotheses; real customers settle them.
- **Plan → test → run flow with human gates.** The founder reviews the plan before any simulation, and corrects the competitor profiles before the wargame. Then: customer-stack sim → competition sim → max-3 findings each (paired with cheap real tests) → 2–3 iteration loops → Strategy Doc + Operating Plan + Investment Card.
- **Anti-paralysis by design.** Sim depth scales to what's about to be spent; findings are capped and every one comes with a move; founder conviction is treated as data. Scenarios are rehearsal for the future — not homework before you're allowed to start.
- **Story-driven.** Captures **customer, founder, and stakeholder stories** in a strict testable template (*As a… when… I want… so that… and I'd…*), each tagged `assumed` / `sim-tested` / `evidence`. The founder's hard DOs and DON'Ts are captured up front as binding guardrails. A physical business fails on three surfaces — customer won't buy, founder can't execute, or a stakeholder (supplier/landlord/funder/regulator) breaks the chain — so each gets a story the plan is accountable to.
- **Learns from precedent, not just theory.** Draws on how physical businesses actually succeeded and failed in India and comparable economies — always separating the transferable lesson from luck and context, and always including the failures, so precedent informs without becoming survivorship bias.
- **Serves both ends — MSME to Venture.** Calibration sets length and jargon, not reading level (every founder reads English fine): livelihood founders get concise, jargon-light output and a real setup on-ramp (Udyam, GST, FSSAI); venture founders get a fast-pass plus fundraising sequence, dilution math, VC criteria, and the strategic-acquirer exit landscape. It maps India's actual capital sources for each (Mudra/CGTMSE/gold-loan/TReDS vs angel→seed→A) and offers the upward scale challenge ("this could be Venture — here's the cost") without pushing.
- **Feels like a partner, not a form.** Gives a hot-take before the interview, prints a progress header each turn, recalls session state, handles re-entry when a locked section reopens, and contributes a benchmark or comp in every exchange — not just questions.
- **India-aware, MBB-grade.** For India-based plans it cuts the market 30 ways (economic class India1/2/3, city-tier, generation, digital/channel behaviour, values, category behaviour) to spot opportunity and force a precise beachhead instead of "all of India." It treats **each city tier as its own microcosm** (metro saturation and ghost-malls vs Tier-2's better economics and rising spend — pick a specific city, not a tier), and **South India as a distinct bloc** (highest per-capita consumption, vernacular-first across Tamil/Telugu/Kannada/Malayalam, strong regional retail champions). It treats **every age as a market** — millennials (peak earners now), Gen X and seniors (high-income, under-served silver economy), and Gen Z (social-first, phygital, values-gated). Plus current sector tailwinds and the margin traps that kill Indian physical businesses (GST 2.0, inverted-duty ITC, working capital). Tuned for 0→1 businesses targeting ~₹8–17 crore ($1–2M).
- **Ambition calibration first.** Livelihood / Growth / Venture — sets how deep to go. Same bar for a sound plan; different scope.
- **One-way-door discipline.** Reversible decisions → move fast. Irreversible + costly → slow down, pilot small.

## Usage

Just describe what you're doing — the controller triggers and pulls in the sub-skills automatically:

> *"I want to start a furniture brand selling online. Is it worth it?"* → planner (Track A) → founder-fit after the bet locks → market-sim to rehearse price/positioning

> *"My bakery does well locally — should I add a second product line?"* → planner (Track B)

> *"We want to export to the UAE."* → planner + domestic→international conversion

> *"What does Hooked actually tell me to do for my subscription box?"* → **whisper**

You can also call a sub-skill directly: *"assess my founder-market fit for X"*, *"rehearse this offer against my target market"*, or *"how did a business like mine actually get built?"*

## Related open-source skills

market-sim is a lightweight rehearsal built into planning. For heavier standalone market simulation, these community skills do it well:
- **crowdcast** — `github.com/TheQmaks/crowdcast` — multi-agent social simulation, zero dependencies.
- **claude-persona** — `github.com/takechanman1228/claude-persona` — structured persona panels (informed by Microsoft's TinyTroupe).

Method credit for the simulation approach: Stanford's Generative Agents (Park et al., 2023) and Social Simulacra. This bundle borrows the method, not the code, and keeps it honest about its place on the evidence ladder.

## Install

**Claude Code (plugin):**
```
/plugin marketplace add diligent-dilettante/business-planner
/plugin install business-planner
```

**Claude.ai / Claude Desktop:** upload the skill folders under **Settings → Capabilities → Skills**, or add them to a Project's knowledge. Each skill's description stays under the 1024-character limit.

**Manual (any agent that supports skills):**
```
git clone https://github.com/diligent-dilettante/business-planner.git
cp -r business-planner/business-planner .agents/skills/
cp -r business-planner/founder-fit .agents/skills/
cp -r business-planner/market-sim .agents/skills/
cp -r business-planner/plugins/business-planner/skills/whisper .agents/skills/
```

## Structure

```
.
├── .claude-plugin/
│   └── plugin.json
├── business-planner/          # controller
│   ├── SKILL.md
│   └── references/
│       ├── frameworks.md
│       ├── business-plan-template.md
│       ├── domestic-to-international.md
│       ├── india-market-context.md
│       ├── india-segmentation.md          # 30 MBB-style market cuts
│       ├── india-regional-tiers.md        # tier microcosms + South India + Vizag deep-dive
│       ├── india-consumption-by-age.md    # how each generation buys
│       ├── india-capital-landscape.md     # MSME schemes + VC funding stages
│       ├── venture-track.md               # Venture-profile only: raise, dilution, exit
│       ├── msme-setup.md                  # Udyam / GST / FSSAI first-week on-ramp
│       └── stories.md
├── founder-fit/
│   └── SKILL.md
├── market-sim/                    # customer stack: B2C / B2B / B2G / B2B2C
│   └── SKILL.md
├── competition-sim/               # adjudicated business wargame
│   └── SKILL.md
├── strategy-ops/                  # strategy doc + operating plan + investment card
│   ├── SKILL.md
│   └── references/
│       └── strategy-ops-templates.md
├── whisper/
│   ├── SKILL.md
│   └── references/
│       ├── case-library.md
│       └── book-library.md
├── README.md
└── LICENSE
```

## License

MIT. Use it, fork it, adapt it.
