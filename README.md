# Position, or Be Positioned

**The Ekram Method as your positioning advisor.**

AI made building cheap. It made being understood expensive.

[![Add to your agent](https://skills.sh/b/soheilmomeniii/positioning-with-ekram)](https://skills.sh/soheilmomeniii/positioning-with-ekram)

Positioning with Ekram turns vague products, books, protocols, companies, and personal brands into clear market positions before writing the homepage, launch post, name, bio, or pitch. It fixes the market story first, then writes the words.

It diagnoses the customer, substitute, proof, timing, and sacrifice before writing copy. It interviews you when facts are thin, checks your rivals' actual copy before calling you differentiated, refuses to ship copy on claims you cannot prove, critiques your existing drafts line by line instead of replacing them, and ends every answer by telling you where you stand and your next move.

Built on the **Ekram Method**, a positioning and narrative method for technology. The method is credited to Ekram (@ekrahm); this skill is a faithful reconstruction and operating procedure, not an original theory. It is a specialist by design: every rule it applies traces to the method. It is not a general copywriter, and any technique that cannot be traced to the method stays out of its output.

## Install

`npx skills add soheilmomeniii/positioning-with-ekram`

Other tools:
- **Claude Code:** drop the `positioning-with-ekram/` folder into `~/.claude/skills/` (personal) or `<project>/.claude/skills/` (project). It loads automatically.
- **Cowork / one-click:** rename the packaged file from `.zip` to `.skill` and open it for a "Save skill" button.
- **Any other agent:** open `SKILL.md` and paste it into the agent's skills directory or system prompt. The `references/` files load on demand.

## What it is

- A positioning advisor, not a copy generator.
- A copy system that starts with diagnosis.
- A pressure test for your claims, rivals, proof, timing, and sacrifice.
- A way to turn strategy into public language a market can repeat.

## What it is not

- A generic prompt pack or a general copywriter.
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
- `references/`: method sequence, artifact playbooks, brand and culture and founder work, narrative and attention and launch, examples, glossary, worksheets, sourced quotes. Loaded on demand.
- `evals/`: 21 test prompts with pass-checks so you can verify behavior, plus the full run log.

## Evals

The skill ships with 22 eval prompts and pass-checks in `evals/evals.json`, plus a run log in `evals/RESULTS.md`.

Latest results, reported plainly. v0.10 is a consolidation release: after days of eval-driven patching the manual had grown to the point where subjects dropped old stable rules while satisfying new ones, so it was rewritten from 671 lines to 390 with every rule stated once. Run 13 (v0.10, all 21 prompts, Claude Sonnet subjects): 13 pass, 7 partial, 1 fail, the best full-suite score to date, with zero em dashes across all 21 responses and the two chronic failures (manufactured weakness on clean passes, incomplete category memos) passing cleanly. Earlier cross-model runs on v0.9.x: Opus subjects 13/4/0, GPT-family subjects 7/5/5; protocol discipline varies by model family, and the run log records the harness for every run.

Known residual risk, documented in `evals/RESULTS.md`: naming requests on thin facts flip between correctly withholding candidates and shipping them with an assumed sacrifice (the one fail in Run 13), and founder stories can still carry a sentence or two of unsupported color. Read the log before trusting any of this.

## Version history

Current: v0.10.1 (v0.10 consolidation plus the deep-turn close rule) (SKILL.md rewritten to 390 lines from 671, full-suite Run 13: 13 pass, 7 partial, 1 fail, best score to date). Named positioning-products through v0.8.3. See `CHANGELOG.md` for the full history.
