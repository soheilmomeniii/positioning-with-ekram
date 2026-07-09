# Position, or Be Positioned

**The positioning operator for builders.**

AI made building cheap. It made being understood expensive.

[![Add to your agent](https://skills.sh/b/soheilmomeniii/positioning-products)](https://skills.sh/soheilmomeniii/positioning-products)

Positioning Products helps builders turn vague products, books, protocols, companies, and personal brands into clear market positions before writing the homepage, launch post, name, bio, or pitch. It fixes the market story first, then writes the words.

It diagnoses the customer, substitute, proof, timing, and sacrifice before writing copy. It interviews you when facts are thin, checks your rivals' actual copy before calling you differentiated, refuses to ship copy on claims you cannot prove, critiques your existing drafts line by line instead of replacing them, and ends every answer by telling you where you stand and your next move.

Built on the **Ekram Method**, a positioning and narrative method for technology. The method is credited to Ekram (@ekrahm); this skill is a faithful reconstruction and operating procedure, not an original theory.

## Install

`npx skills add soheilmomeniii/positioning-products`

Other tools:
- **Claude Code:** drop the `positioning-products/` folder into `~/.claude/skills/` (personal) or `<project>/.claude/skills/` (project). It loads automatically.
- **Cowork / one-click:** rename the packaged file from `.zip` to `.skill` and open it for a "Save skill" button.
- **Any other agent:** open `SKILL.md` and paste it into the agent's skills directory or system prompt. The `references/` files load on demand.

## What it is

- A positioning operator, not a copy generator.
- A copy system that starts with diagnosis.
- A pressure test for your claims, rivals, proof, timing, and sacrifice.
- A way to turn strategy into public language a market can repeat.

## What it is not

- A generic prompt pack.
- A slogan generator.
- A hype machine for unproven claims.
- For people who want nicer words instead of harder thinking.

## Before / After

**Creator product**

Before: "We're building an AI marketing platform for creators."

After: "A launch operator for solo creators who sell paid products, not audience attention."

Why it is better:
- names the customer: solo creators who sell products
- names the outcome: launches, not reach
- names the substitute logic: against audience-growth tools
- avoids generic hype

**Startup homepage hero**

Before: "The modern platform for data-driven revenue teams."

After: "Pipeline review software for B2B sales managers who forecast in spreadsheets and miss quota by surprise."

Why it is better:
- names who: B2B sales managers
- names the painful moment: surprise quota misses
- names the substitute: spreadsheets
- promises a specific job, not a category

**Book or protocol**

Before: "A book about productivity and building better habits."

After: "A field manual for people who have read every habit book and still cannot start."

Why it is better:
- names the reader by their real state: tried everything, still stuck
- names the substitute: other habit books
- promises a mechanism, not a topic
- earns attention on a crowded shelf

## How to use

Just ask:
- "position my startup" (it interviews you if context is thin)
- "write a homepage hero for X"
- "review this homepage copy: [paste]" for line-by-line keep, kill, rewrite
- "fix this vague line: we're building the future of Y"
- "is this a Jordan or a Thiel play?"

It diagnoses first, pushes back on vague positioning, and closes every answer with your next action. For long strategy work it can keep a position file in your workspace so "what's next" survives between sessions.

## What's inside

- `SKILL.md`: the operator manual, canonical over references.
- `references/`: method sequence, artifact playbooks, brand and culture and founder work, narrative and attention and launch, examples, glossary, worksheets, and a sourced quote bank (the method's spine as verbatim lines with year and link). Loaded on demand.
- `GUIDE.md` and `Positioning-Products-Guide.pdf`: the method and how to use it.
- `evals/`: 20 test prompts with pass-checks so you can verify behavior, plus run logs and an independent blind-run report.

## Evals

The skill ships with 20 eval prompts and pass-checks in `evals/evals.json`, plus a run log in `evals/RESULTS.md` and an independent blind-run report archived alongside it.

v0.8 was tested twice, independently: a strict two-grader run and a separate blind run (9 pass, 10 partial, 1 fail). Both found the same thing: the method held, the protocol discipline leaked. The fixes that followed (v0.8.1 through v0.8.3) were re-tested on the 11 non-pass evals: 9 pass, 2 partial, 0 fail, with variance loops on the five least stable behaviors. Three residual leaks found in those loops are fixed in v0.8.3 but have not been re-run as a full suite; the complete history, per-run numbers, and known residual risks are in `evals/RESULTS.md`. This skill's own rule applies to itself: no claim without a receipt, and the receipts are in the log.

## Version history

Current: v0.8.3, built from a 10-skill competitive audit and two independent 20-eval runs (multiple-choice intake, market validation stage, graded critique, sourced quote bank, plus discipline fixes). See `CHANGELOG.md` for the full history.
