# Positioning Products (v0.7)

[![Add to your agent](https://skills.sh/b/soheilmomeniii/positioning-products)](https://skills.sh/soheilmomeniii/positioning-products)

**New here?** Read the [Guide](GUIDE.md) (method + how-to), or the designed [PDF](Positioning-Products-Guide.pdf).

> AI made building cheap. It made being understood expensive. The scarce edge is meaning: whether a market can say what you are, want it, and believe it is where the world is going.

An agent skill that turns a vague idea, product, company, book, or personal brand into a sharp, defensible position, then writes the copy. It diagnoses before it writes, interviews you when facts are thin, checks your rivals' actual copy before calling you differentiated, refuses to ship copy on unproven claims (but will write labeled provisional copy if you insist), critiques your existing drafts line by line instead of replacing them, and always ends by telling you where you are and the next move.

Built on the **Ekram Method**, a positioning and narrative method for technology. The method is credited to Ekram (@ekrahm); this skill is a faithful reconstruction and operating procedure, not an original theory.

## Install (pick what your tool supports)
- **skills.sh (recommended):** `npx skills add soheilmomeniii/positioning-products`
- **Claude Code:** unzip and drop the `positioning-products/` folder into `~/.claude/skills/` (personal) or `<project>/.claude/skills/` (project). It loads automatically.
- **Cowork / one-click:** rename this file from `.zip` to `.skill` and open it to get a "Save skill" button. (A `.skill` is just this zip renamed.)
- **Any other agent:** open `positioning-products/SKILL.md` and paste it into the agent's system prompt or skills directory. The `references/` files load on demand.

## How to use
Just ask. For example:
- "position my startup" (it will interview you if context is thin)
- "write a homepage hero for X"
- "review this homepage copy: [paste]" (line-by-line keep/kill/rewrite)
- "fix this vague line: we're building the future of Y"
- "is this a Jordan or a Thiel play?"

It diagnoses first, pushes back on vague positioning, and closes every answer with your next action. For long strategy work it can keep a position file in your workspace so "what's next" survives between sessions.

## What's inside
- `SKILL.md`: the operator manual (the skill itself, canonical over references).
- `references/`: distilled method, artifact playbooks, brand/culture/founder, narrative/attention/launch, examples, glossary, worksheets (loaded on demand).
- `evals/evals.json`: 12 test prompts with pass-checks, so you can verify it behaves.

## What changed in v0.7
From an external 5-agent audit (4 critical, 3 high, 5 medium findings, all addressed):
- **Claim-proof alignment**: examples must prove the claim actually being scored; a mismatch redirects proof collection or triggers honest repositioning.
- **Qualitative superlatives gated**: "most trusted / loved / intuitive" now require third-party rankings, NPS/retention data, named references, or audits. Testimonials alone do not pass.
- **Mode tiebreaker**: full beats critique beats light; length constraints compress, never downgrade; "go deeper" escalates.
- **Sacrifice cannot be assumed**: like proof, it requires direct input. A sacrifice invented for the user costs them nothing.
- **Second-pass interview rule**: when 5+ facts are missing, questions go to proof and sacrifice first, one follow-up round of up to two questions allowed.
- **Ban list expanded to 30 words**, split into hard-banned (21) and flagged-with-justification (9).
- **Vocabulary split**: always-jargon vs normal-English-unless-used-as-method-label, with a swap test.
- **Multi-gate blocker priority**: name all weak terms; fix Authentic, then Differentiated, then Relevant.
- **Verification checklist extended**: claim-proof alignment, ban-list enforcement, explain/compress/provoke gate on every name and headline, dunk-risk check, market-check confirmation.
- **5 new evals** (17 total): three-turn interview-to-artifact arc, naming, founder narrative, category memo, rival fetch. Not yet run; see evals/RESULTS.md.
- Example 3 in the case bank replaced to avoid template repetition.

## What changed in v0.6
- **Light-mode brevity cap**: under 250 words by default; a single headline gets at most 3 rewrites plus one sentence of diagnosis.
- **Less-friction market check**: in light mode the skill states the assumed rival axis in one line and proceeds; fetching or asking is full-mode behavior.
- **Strategic territories**: when proof is missing, the skill can write 2-3 honest positioning directions with the proof needed for each. Strategy no longer stalls at the proof gate; only copy does.
- **Landing-page playbook**: full page structure (hero, trust strip, is/is-not, what's inside, proof or source-integrity contract, sample lines, primary + secondary CTA).
- **Book/artifact launch playbook**: position by repeatable line, named reader, mechanism, source/proof contract, one primary action, compressed launch sequence.
- Evals updated for the new rules (brevity cap measured, territories sanctioned at the gate); full 12-eval suite re-run against live agents.

## What changed in v0.5
Tested: the 10 prior evals were run against live agents (2 more were added after, 12 total). Six passed clean; four exposed drift, now fixed:
- Interview responses dropped the closing next-action line. Now mandatory for every response type.
- Two responses leaked the machinery ("the manual tells me..."). Now banned: the skill never mentions itself or its process.
- The proof gate produced provisional copy unprompted, with the unproven superlative left in as an option. Now: first move at the gate is always stop-and-ask; provisional only on explicit request; the superlative may not appear in any variant.

New capabilities:
- **Critique mode**: paste existing copy, get a verdict on the position underneath plus line-by-line keep/kill/rewrite markup, not a wholesale replacement.
- **Market check**: when the rival is a named company, the skill fetches (or asks for) their actual copy before scoring differentiation.
- **Artifact playbooks** (`references/artifacts.md`): structure, limits, and kill-lists for homepage heroes, launch posts, one-liners/bios, deck narrative arcs, category memos, and naming.
- **Position file**: for multi-session strategy work, the skill offers to keep a `position-[name].md` recording facts, gate scores, blockers, and next action.
- **Pass calibration**: when a gate passes cleanly, it says so in one line and moves on. No manufactured weakness.
- **Wider case bank**: Liquid Death (consumer/commodity), ServiceTitan (boring B2B), Atomic Habits (book/creator) join the crypto and SaaS cases, plus a book/creator copy pattern.
- 2 new evals: critique-mode markup, clean-pass without manufactured weakness (12 total).

## v0.4
- Method vocabulary analysis-only; light mode closes with one line; provisional path added to the proof gate; no em dashes; SKILL.md canonical; 4 new evals.
