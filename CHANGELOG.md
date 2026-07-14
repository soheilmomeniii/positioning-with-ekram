# Changelog

All notable changes to the **Positioning with Ekram** skill (built on the Ekram Method) are documented here. Newest first. Named positioning-products through v0.8.3; renamed in v0.9 to match what it is: the Ekram Method as your positioning advisor.

## v0.10.1
From Somo's field report on v0.10: responses stopped giving a next move in later turns of live sessions. Root cause: evals graded single responses, so the close held there and died in conversation flow, where short follow-up turns read as chat, not deliverables.
- **Every turn means every turn**: option picks, side answers, acknowledgments, and two-line replies deep in a session all close with the one-line Next form. The shorter the reply, the more the Next line matters.
- **New eval** `deep-turn-close` (22 total): a four-turn session ending in "ok cool"; every turn must close with a concrete, product-specific next move. Passed 2 of 2 loops on this release, including the two-word turn.

## v0.10
The consolidation release. SKILL.md rewritten from 671 lines to 390 after Runs 11-12b showed rule saturation: patches were fixing one eval by breaking another, and subjects dropped old stable rules while satisfying new ones.
- **Every rule stated once**: the five overlapping no-manufactured-asks rules merged into one section (One Place To Ask); the interview cluster collapsed from eleven paragraphs to five; the decision ledger folded into stage chaining; market check and fallback reconciliation merged.
- **Thin-copy trap scoped**: final copy (headlines, name candidates, hero variants, launch posts) waits for proof and sacrifice; provisional structures ship (territories, six-block memo with labeled assumptions, launch architecture, fact-based stories). Fixes the v0.9.4 regression that blocked category memos.
- **Verification cut from 25 checks to 16.**
- Run 13 (full 21, sonnet): 13 pass / 7 partial / 1 fail, best full-suite score across all runs; clean-pass and category-memo both pass cleanly for the first time; zero em dashes in all 21 responses. Remaining knife edge: naming-request write-vs-withhold flip, two unsupported sentences in founder stories.

## v0.9.4 candidate
From the crash-safe targeted checkpoint after v0.9.3 candidate. The first case, `vague-ai-trader-tool`, still failed because thin copy requests pulled the agent into headline-writing before proof and sacrifice were supplied.
- **Thin-copy trap rule**: fragmentary requests like "make this sound better: AI tool for traders" no longer draft polished artifacts just because light mode was selected. They get a provisional diagnostic frame plus questions only.
- **First-pass thin-input question order**: customer, substitute, proof, sacrifice. If only two questions fit, proof and sacrifice win. If sacrifice is missing, one question must force it.
- **No overclaim on validation**: v0.9.4 candidate is patched and statically checked against the eight targeted failures, but still needs a blind model re-run before release-grade claims.

## v0.9.3 candidate
From package review after v0.9.2. Goal: reduce knife edges without adding generic copywriting craft.
- **Action layer**: major full-mode outputs now turn strategy into work: decisions made, ship next, do not do, proof needed, first channel. This attacks the recurring "beautiful brief, no work order" failure.
- **Decision ledger**: late stages now pull from customer, enemy, substitute, category, promise, proof, sacrifice, axis, and action. This keeps the anti-drift benefit without forcing stiff exact-word repetition.
- **Rival fallback reconciliation**: when browsing is unavailable, the skill asks for rival copy, defers Differentiated, continues non-comparative strategy with assumptions, and blocks comparative artifacts until the paste lands.
- **Founder story playbook**: founder narratives now use a point-of-action structure and a dedicated artifact playbook so missing beats are omitted or requested instead of filled with fictional color.
- **README corrected**: current version and eval status now reflect the v0.9.2/v0.9.3 candidate state instead of stale v0.9 claims.
- Not yet full-suite re-run. Targeted gate before release: `vague-ai-trader-tool`, `positioning-book-launch`, `category-memo`, `clean-pass-no-manufactured-weakness`, `founder-narrative`, `rival-fetch`, `three-turn-arc`, and `naming-request`.

## v0.9.2
From Run 10, Somo's second external run (GPT-family subjects via native Codex subagents, 17 evals: 7 pass / 5 partial / 5 fail; harness held at moderate confidence; archived in evals/). Headline finding: protocol discipline is model-dependent (Opus 13/4/0, GPT 7/5/5 on the same skill); fixes remove knife edges instead of adding prose.
- **Provisional-frame rule**: thin facts never force pure interview or pure copy. Every thin-facts response opens with one labeled diagnostic frame (lazy position, likely substitute, direction), then the questions. Final artifacts still wait for proof and sacrifice.
- **Clean-pass advance rule**: when customer, substitute, proof, timing, and sacrifice are all supplied, gates pass unless contradicted and the artifact ships in that response; no new asks manufactured after it ships.
- Rejected from the same report: stopping full-mode strategy at the rival paste request (contradicts the deliverable floor), and two "missing rule" claims for rules that have existed since v0.8.2 (multi-turn arcs, naming tags).

## v0.9.1
From Run 9, Somo's external Codex run on v0.9 (Opus 4.6 subjects, 17 evals: 13 pass / 4 partial / 0 fail; standing checks 17/17; archived in evals/):
- **Richness rule**: the interview weighs how rich supplied material is, not just how many facts are missing. Rich partial material means assume everything assumable and ask only proof and sacrifice; never re-ask an implied fact.
- **Immediate category-name test**: a user-proposed category name is tested against explain/compress/provoke in the same response, independent of the open interview.
- **Mandatory rival paste-request**: when browsing is unavailable, asking the user to paste the rival's copy is required, and folds into the interview questions.
- Cross-model note: founder-narrative flips by model family (sonnet invents, opus over-interviews). Both directions now have explicit rules against them.

## v0.9
From field use: responses opened sharp and closed generic. Root cause was architectural: every diagnostic stage was templated, the artifact itself was a placeholder governed only by ban lists, and closing fields accepted one-word label fills.
- **Stage chaining**: each stage consumes the one before it and must reuse its exact nouns; the later the stage, the more of its words come from earlier sections. A late stage with no noun from Facts is drift, rewritten before advancing. Sacrifice and fork test get paste-under-another-product tests.
- **Artifact gate**: the artifact is assembled from the diagnosis, never written fresh. Four required carries in full mode (substitute, sacrifice, proof point, diagnosis nouns), compressed floor in light mode.
- **Rival-logo test**: the thousand-products test promoted from sentence level to artifact level. Any line that reads true under the nearest rival's name gets rewritten or cut.
- **Point-of-action templating**: playbooks reread immediately before drafting; mode templates now state the gate at the Output slot.
- **Concrete close rule**: one-word fills fail the stage block; every closing field carries a product-specific noun and every next action passes the tomorrow-morning test (executable without a clarifying question).
- **New eval** `artifact-carries-diagnosis` (21 total): the Output section alone must reconstruct customer, substitute, and sacrifice; closes graded for concreteness.
- **Silent gate**: the artifact gate and its tests run silently; the response never prints the checklist or announces a test was run. Added after Run 7 caught the new gate inducing machinery narration.
- **Specialist identity**: the operator is a positioning advisor working one method, never a general copywriter; any technique that cannot be traced to the method stays out of the output. Briefly added generic thread-craft and landing-page copywriting rules with worked examples; removed same week as off-method. Launch threads are now governed by method concepts only: coordination signal as its own quotable line, sacrifice as refusal, prove before you say, dunk-risk check.
- **Playbooks traced to the method**: v0.6-era copywriting details removed from artifacts.md (10-word headline cap, CTA verb examples, character counts, CTA-count caps, one-idea-per-slide, the naming type taxonomy that contradicted the manual's own taxonomy ban, domain/trademark checks). Each playbook part now states the method concept it applies: four questions in the headline, prove before you say in the proof strip, who shows up in the trust strip, sacrifice in the is-not column and the CTA count, narrative singularity in the deck arc, the name is the thesis in naming. Structures stay only where they map to method stages.
- Run 7 (full 21, sonnet): 11 pass / 8 partial / 2 fail. Drift check 20/21, concrete-close check 21/21; the strong-start-generic-end failure did not reproduce. Residuals are pre-existing tics (em dashes, story invention, light-mode word cap), logged in evals/RESULTS.md.

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
