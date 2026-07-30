# Financial model spec

**The minimum viable financial model for a physical business.** Build this by default. Do not wait to be asked for any of it.

Section A4 mandates that unit economics cannot be skipped. This file defines what that means in practice.

---

## 1. Three statements that tie

| Statement | Requirement |
|---|---|
| **P&L** | Monthly for 36 months, rolled to annual |
| **Balance sheet** | At each year end |
| **Cash flow** | Indirect method, split operating / investing / financing |

**Two check rows, both reading zero:**

- Balance sheet: `total equity and liabilities − total assets = 0`
- Cash flow: `closing cash − balance sheet cash = 0`

A model without tie checks is a spreadsheet of hopes. The checks are what make it auditable by a bank, an accountant, or a buyer.

---

## 2. Local accounting classification

Use the classification the founder's accountant, banker and registrar will recognise.

**India:** Schedule III (Companies Act 2013) for P&L and balance sheet; AS-3 / Ind AS 7 for cash flow.

That means P&L lines read: Revenue from operations · Other income · Cost of materials consumed · Employee benefits expense · Finance costs · Depreciation and amortisation · Other expenses.

Not: "revenue, COGS, opex." A model in generic startup format has to be rebuilt before anyone official can use it.

---

## 3. Local number formatting

**India:** lakh/crore comma placement. `₹1,72,50,000` — never `₹17,250,000`.

This is not cosmetic. A model in Western formatting signals the analyst does not know the market, and it makes every number harder for the founder to sanity-check against figures they hold in their head.

Apply the same principle in any market: use the convention the reader reads in.

---

## 4. Dashboard tab

**First tab. The founder should never need to open another one to answer "what if."**

- 10–15 headline drivers, editable, visually distinct (one fill colour, used only for inputs)
- Results adjacent — NPV, IRR, capital, EBITDA by year, break-even, cash trough
- A verdict cell that reads plainly: `VIABLE` / `CASH TIGHT` / `AT RISK` / `DESTROYS VALUE`

**Wire it properly.** The dashboard cells should *be* the inputs, with the assumptions tab referencing them — not a mirror the founder edits in one place and reads in another.

---

## 5. Scenario toggles

- Base / downside / upside, driving the demand and cost assumptions
- Plus a toggle for every binary strategy choice the plan contains — make vs buy, lease vs own, with or without a grant, one route vs another

**A binary choice that cannot be toggled has not been modelled, it has been assumed.**

---

## 6. Break-even, decomposed

A single break-even number is the least useful form of a genuinely useful metric.

**Decompose two ways:**

**By phase** — break-even falls as revenue streams come online, often while costs are rising. That curve is the de-risking story and it is invisible in a single figure.

**By stream** — which revenue lines scale with volume, and which cover fixed cost regardless. The second kind lower break-even without needing a single extra customer, which changes what the founder should launch first.

```
| Phase | Streams live | Fixed cost covered | Break-even | Actual | Margin |
```

---

## 7. Contribution and marginal analysis

- Contribution per unit, built up from revenue and variable cost line by line
- **MC as a percentage of MR** — this single ratio governs the entire discounting policy

Where marginal cost is a small fraction of marginal revenue, unsold capacity is permanently lost inventory and the correct discount floor is far lower than instinct suggests. Where it is high, discounting destroys the business.

**State the discount floor explicitly**, and the distinction between discounting *capacity* (correct) and discounting *the brand* (not).

---

## 8. Sensitivity

A grid on **the two drivers that actually move the answer** — usually volume and price, but derive it rather than assuming.

Not a list of one-way sensitivities. The interaction is where the insight is.

---

## 9. Source tag on every input

Three tags, no fourth:

| Tag | Meaning |
|---|---|
| `sourced` | With a citation |
| `founder-supplied` | From the founder's own knowledge |
| `estimate` | Explicitly flagged as the analyst's guess |

A column on the assumptions tab. **If a number would materially move the answer and cannot be sourced, say so in the same breath as using it.**

---

## 10. Financing, if there is debt

- Loan schedule with moratorium handling
- Interest and principal split
- **DSCR by year** — banks will ask, and the covenant floor is typically 1.25–1.50x
- Debt/EBITDA and interest coverage

---

## 11. Returns

- NPV at the founder's **real** cost of capital — their actual alternative use of the money, not a textbook rate
- IRR, and **equity IRR separately** where there is debt
- **NPV excluding terminal value.** This is the honest floor: what the business earns from operations alone. The gap between the two NPVs is what the founder is betting on
- Payback, simple and discounted
- Profitability index

---

## 12. Terminal value — match it to the asset

| Situation | Treatment |
|---|---|
| Owned premises, saleable going concern | EBITDA multiple, stated conservatively |
| **Leased land, movable assets** | **Salvage of movable assets + refundable deposits. Not a multiple** |
| Founder-dependent operation | Discount heavily, or set to zero and say why |

**Never apply both a short horizon and a salvage-only terminal.** That double-counts the conservatism. If the residual is only scrap, the honest test is cash flows across the full holding period.

---

## Things that are usually missing and usually matter

Check each explicitly rather than assuming they are immaterial:

- **Seasonality** — most physical businesses have it
- **Maintenance and replacement capex** — the wear item is rarely the obvious one
- **Platform or channel commission** — often 5–20%, frequently modelled at gateway rates instead
- **Spectators, companions, non-buying visitors** — they buy things
- **Staff scaling with volume** — flat staffing from month one is never how anyone operates
- **Pre-opening carrying cost** — rent and overhead before revenue
- **Founder time** — usually uncosted, and it changes every comparison against a passive alternative

---

## Anti-patterns

**Do not** hand-write a figure into a document that also exists in the model. It will drift. The model is the single source of truth; documents reference it.

**Do not** present a single confident number for a pre-revenue business. Three scenarios with driving assumptions shown, always.

**Do not** let the model flatter the plan by omission. A missing cost is an error in the founder's favour, which is the more dangerous direction.
