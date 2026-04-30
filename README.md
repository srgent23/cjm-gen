# CX Business Case Builder
**OG&E | Customer Journey Management**

A single-file web app that drafts structured CX business cases from raw signals using the Anthropic API.

---

## What It Does

You pick a journey, paste a signal or pain point, select your audience, and hit Generate. The app drafts a formatted business case in OG&E voice — opportunity-rich framing, phased actions, KPIs, risks, and a clean ask.

---

## The Four Journeys

| Journey | Code | CJM |
|---|---|---|
| Billing & Payments | BPMTS | U |
| Outages | OUT | E |
| Start Stop Transfer | SST | — |
| Programs & Services | P&S | E |

Each journey pre-loads its own data sources and pain point vocabulary into the AI prompt.

---

## The Three Audiences

- **KB** — Opportunity-rich framing, clear ask, speed to execute
- **JW** — Results only, lead with outcome
- **TDS / JC** — Technical framing, action plan, owners and timelines

---

## Output Sections

1. One-Line Case
2. What We're Seeing
3. The Opportunity
4. Phase 1 | Fast Actions
5. Phase 2 | Structural
6. Success Metrics
7. Risks + Mitigations
8. Ask

---

## How to Run

Open `oge-cx-business-case-builder.html` in a browser.

> **Note:** The Generate button calls the Anthropic API. It works out of the box inside Claude.ai. To host elsewhere, add your own API key to the `fetch` headers in the script.

---

## Writing Rules Baked In

- No em dashes
- No AI-sounding constructions
- Opportunity-rich framing only — never "problem" language
- Phase 1 and Phase 2 always clearly separated
- Statistics must trace to a named source
