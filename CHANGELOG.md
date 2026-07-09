# Changelog

All notable changes to the **Positioning Products** skill (built on the Ekram Method) are documented here. Newest first.

## v0.8.3
From eval Run 6 (v0.8.2: 9 pass / 2 partial / 0 fail on the 11 re-run evals; variance loops exposed three residual leaks):
- **No-invention rule for narrative artifacts**: founder/origin stories are built only from supplied facts; invented color is fabricated proof. Thin stories ask for one real detail instead of writing a fictional one.
- **Sequence completion under the proof gate**: the gate freezes copy, never the sequence; full-mode runs deliver every remaining stage with labeled assumptions even when proof is deferred.
- **Navigation close discipline**: "what's next" responses close with the one-line Next form, never the full stage block.

## v0.8.2
From Somo's independent blind eval run on v0.8 (20 isolated subagents, pass/partial/fail grading: 9 pass, 10 partial, 1 fail; archived in evals/):
- **Multi-turn arc rule**: staged conversations produce every turn as its own complete response with its own stage control; never collapse the arc into the final artifact.
- **Launch architecture required**: a launch request must ship the launch architecture (phases with what each proves, coordination signal, dunk-risk check) in the same response; diagnosis alone is a failed launch response.
- **Naming template hardened**: fixed four-part candidate line (Name. tag. Thesis. Risk.), periods not dashes; adds the risk read both runs found missing.
- **Category memo template**: six required blocks (name test, what it replaces, category question, adjacent players, category-of-one risk, missing proof); skipping one fails the memo.
- Grading standard adopted: pass/partial/fail with per-check results and harness notes, logged per run in evals/RESULTS.md.

## v0.8.1
From eval run 4 (20 evals, strict two-grader protocol; 9 clean / 5 form-issue / 6 fail, failures logged in evals/RESULTS.md):
- **Deliverable floor**: if supplied facts are enough with labeled assumptions, the artifact ships in the same response; "full strategy" always produces the full sequence; a missing rival paste defers only the Differentiated score; fact-narrating artifacts (founder story) never blocked on sacrifice.
- **Provisional numbers ban**: no measurable or absolute claim anywhere in provisional copy (headline, subhead, body) unless user-supplied.
- **Naming tags enforced**: every name candidate tagged exactly explain / compress / provoke plus a one-line thesis; no substitute taxonomies.
- **Adjacent players named**: Thiel-path category work names 2-3 real adjacent players in the memo itself; deferring is failing.
- **Ban scope extended**: hard-banned words and em dashes now explicitly banned in the agent's own analysis and narrative framing, lists, and name-candidate lines, not just artifacts.

## v0.8
From a 10-skill competitive audit (skills.sh top positioning/marketing skills, 2026-07-09). Not yet pushed to GitHub.
- **Multiple-choice interviews**: every interview question now carries 2-3 numbered candidate answers inferred from context, plus an open option. Candidates must be specific enough to be wrong. All questions in one message.
- **Three entry modes**: direct request → guided interview; context dump → silent extraction, ask only what's missing; "just guess" → best-guess with labeled assumptions.
- **Validate In Market (new stage 9)**: signal-ranked testing (outbound reply > sales-call conversion > CTR > social), a quantified bar set before the test (default: beat the incumbent position by 20%+ on the chosen signal), phased rollout for repositioning, honest failure reading (return to the failing gate, not louder copy). "validate" added to the stage list; full-mode next action names the first test, signal, and bar.
- **Graded critique**: verdict opens with a score out of 10 derived from D x R x A plus legibility; new "Raise it:" line names the two changes that move the score most.
- **AI-tell ban list**: 10 cadence tells ("let's delve into", "isn't just X, it's Y", ...) banned in artifacts and analysis, plus the thousand-products test.
- **Workspace context check**: before interviewing in full mode, read any existing position file, product/marketing context file, or pointed-to readme, and strike answered questions.
- **New `references/quotes.md`**: the method's spine as verbatim sourced Ekram lines (year + URL), read when the user challenges a rule or asks why it holds. No competitor ships sourced receipts.
- **3 new evals** (20 total): multiple-choice interview flow, validation stage, graded critique. Not yet run against live agents.

## v0.7
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
- **5 new evals** (17 total): three-turn interview-to-artifact arc, naming, founder narrative, category memo, rival fetch. Run against live agents: 17/17 passed on substance, with a form caveat (some runs prefixed internal planning) logged in `evals/RESULTS.md`.
- Example 3 in the case bank replaced to avoid template repetition.

## v0.6
- **Light-mode brevity cap**: under 250 words by default; a single headline gets at most 3 rewrites plus one sentence of diagnosis.
- **Less-friction market check**: in light mode the skill states the assumed rival axis in one line and proceeds; fetching or asking is full-mode behavior.
- **Strategic territories**: when proof is missing, the skill can write 2-3 honest positioning directions with the proof needed for each. Strategy no longer stalls at the proof gate; only copy does.
- **Landing-page playbook**: full page structure (hero, trust strip, is/is-not, what's inside, proof or source-integrity contract, sample lines, primary + secondary CTA).
- **Book/artifact launch playbook**: position by repeatable line, named reader, mechanism, source/proof contract, one primary action, compressed launch sequence.
- Evals updated for the new rules (brevity cap measured, territories sanctioned at the gate); full 12-eval suite re-run against live agents.

## v0.5
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
