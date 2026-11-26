# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Stack

Static HTML/CSS (no build step), hosted on GitHub Pages at readygate.dev (repo readygatedev/readygate.dev). Paddle.js (v2, CDN) for checkout.

## Users

Product managers of any technical level, including PMs who have never opened a terminal. They write tickets or specs for a development team and want them right the first time. The site must explain what Claude Code is and why a PM would run something in it, without assuming technical vocabulary.

## Product Purpose

ReadyGate is a plugin for Claude Code (Anthropic's coding agent) that helps a PM go from a feature idea to tickets developers can build and QA can test. It reads the real codebase (or, with no code yet, the product brief), says whether the feature fits, finds gaps, asks the PM only the product questions they must answer, and writes Markdown tickets: user story, scope, business rules, Given/When/Then acceptance criteria, happy path, dev notes. Success: the PM's tickets stop coming back with "what should happen when…?".

## Positioning

Gates instead of guesses. It will not write a ticket while a product decision is open, will not claim anything about the code it hasn't read (every claim cites `file:line`), respects the team's standing decisions file, and keeps the product repo read-only. Other AI ticket writers fill gaps with plausible inventions; ReadyGate stops and hands the decision back.

## Operating Context

Used inside Claude Code (terminal or IDE) in a PM workspace next to the product repo. Commands: free `/pm-init`, `/pm-discover`, `/pm-ticket`, `/pm-new`, `/pm-backlog`; Pro adds `/pm-push` (Jira, Linear, GitHub Issues), `/pm-board`, `/pm-prototype`, `/pm-review`, `/pm-apply-ticket-changes` and enforcement hooks.

## Capabilities and Constraints

- Free: MIT, public repo github.com/readygatedev/readygate.
- Pro: $49 one-time, one person, delivered as read access to a private GitHub repo (buyer enters GitHub username at checkout); updates for 0.x and 1.x; 14-day refund policy, refund ends the license.
- Paddle is the merchant of record. Seller: Ayoub Ben Thabet, Tunisia. Contact hello@readygate.dev.
- Runs on the user's own Claude Code plan; typical cost per feature $1–4 on API pricing.
- Legal pages required by Paddle: /terms, /refunds, /privacy.

## Brand Commitments

- Name "ReadyGate" and the existing icon (icon.png) are binding. Everything else about the look may change.
- Voice: plain, direct, specific; no hype.
- Look: the user chose the category standard (familiar modern SaaS landing page), played straight at full craft. Bar to match: Linear (linear.app) and Cal.com (cal.com). Chosen 2026-11-26 over bolder directions.

## Evidence on Hand

- Real excerpts from demo runs on examples/acme-shop (in the public README): the refusal to generate when an answer contradicts the code (`runPayouts.ts:7`), finding suspended sellers still being paid (`sellers.ts:14-20`), the Blocked verdict from DECISIONS.md, and a real ticket excerpt (BR-01/02, AC-01/02/04).
- No customers, testimonials, logos, user counts or press exist. Do not fabricate any.
- Benchmarks and test numbers are not approved for the site.

## Product Principles

1. Never guess a product decision; ask.
2. Every claim about the product is grounded in something real.
3. The PM stays in control: nothing is written or pushed without their explicit go-ahead.
4. Understandable by a non-technical PM.

## Accessibility & Inclusion

No product-specific requirement established beyond WCAG AA basics; light and dark themes; works at phone width.
