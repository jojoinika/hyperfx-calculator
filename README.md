# HyperFX — FX Settlement Cost Calculator

An interactive calculator that helps cross-border fintech teams quantify the real cost of the pre-funded float model — and see what on-demand FX liquidity via HyperFX could save them.

## What this is

Built as part of a Marketing & Communications Manager application to Polytope Labs.

The brief I set myself: a fintech CFO needs to feel the problem in their own numbers before they'll take a meeting. Generic statistics ("the naira lost 70% of its value") don't land the same way as "here is what that means for your specific monthly volume and float size." This calculator makes that personal.

## What it does

Enter three inputs:

1. **Monthly transaction volume** — how much your fintech processes per month on the Nigeria corridor
2. **Float as % of volume** — how much of that you hold as pre-funded naira (typical range: 20–40%)
3. **Annual naira devaluation rate** — how much NGN you expect to lose against USD (default: 35%, which is conservative given the 2023–2025 reality)

The calculator outputs in real time:

- **Capital locked in float** — the idle capital on your balance sheet right now
- **Value lost to devaluation over 12 months** — in USD terms, what that naira float loses as the currency moves
- **Effective cost per transaction** — the hidden devaluation cost as a % of your volume
- **What changes with HyperFX** — capital unlocked, devaluation eliminated, total 12-month benefit

Below the calculator: a plain-English explainer of the float problem and how HyperFX solves it, followed by a waitlist sign-up form.

## Why this format

The goal was to build something a fintech Head of Payments could share with their CFO in a Slack message — "put in your numbers and tell me what you think." 

## Tech

Single-file HTML. No dependencies, no framework, no build step. All calculations run in vanilla JS. Deployable directly to GitHub Pages.

## Deploy to GitHub Pages

1. Fork or clone this repo
2. Go to **Settings → Pages**
3. Set source to `main` branch, `/ (root)`
4. Your site will be live at `https://yourusername.github.io/hyperfx-calculator`


- Negative results (costs) in red, positive results (savings) in green — immediate visual language that needs no explanation
- No login, no data sent anywhere — a CFO will not enter real company data into a tool that requires an account

---

*Built by Josephine Inika as a portfolio piece for a Polytope Labs application.*
