# Eval Run Log

Method: each eval prompt was run against a fresh Claude Sonnet agent whose only instruction was to read SKILL.md, adopt it as its operating manual, and answer the prompt as in a live chat. Responses were graded against the checks in evals.json by a separate reviewer. Conversation-dependent evals (provisional-override, whats-next-navigation) were run with the prior turn simulated in the prompt.

## Run 1: v0.4 (2026-07-05, 10 evals)

6 clean passes. 4 drifts found:

- Interview-only responses dropped the required closing line (3 of 10 responses).
- Two responses leaked machinery ("I have the skill loaded", "The manual tells me...").
- proof-gate-superlative: agent wrote provisional copy unprompted and kept the unproven superlative as "Option A".

All fixed in v0.5 (closing line mandatory for every response type; machinery mentions banned; stop-and-ask first at the gate, provisional only on explicit request, superlative banned from all variants).

## Run 2: v0.6 (2026-07-05, 12 evals)

9 clean passes, including all new behaviors: light-mode cap held (~210 words, 3 rewrites), territories offered at the gate with no fake claims, critique mode produced verdict plus line-by-line markup, clean-pass wrote the hero without manufactured weakness, light-mode market check stated the assumed axis in one line.

3 drifts found:

- proof-gate-superlative: opened with procedural narration ("The manual requires proof...").
- provisional-override: asked for confirmation again instead of treating "just write it anyway" as the explicit request.
- clean-pass: narrated internal analysis before the artifact.

Fixes applied: procedure narration banned explicitly; "just write it anyway" defined as the explicit request; "open with a finding, not a plan" rule; proof-gate opening shape (risk sentence, then spine, then territories).

Retest of the two hard failures: provisional-override passed clean (immediate labeled provisional, no superlative, spine attached). proof-gate-superlative passed on substance but still opened with one procedural sentence; the opening-shape rule was added after this retest and has not been re-verified.

## v0.7 status

v0.7 applied 12 fixes from an external 5-agent audit and added 5 evals (three-turn arc, naming, founder narrative, category memo, rival fetch; 17 total).

## Run 3: v0.7 (2026-07-05, 17 evals, Opus agents)

Substance: 17/17 passed their checks. The audit fixes held under test:

- Proof-gate responses opened with the prescribed shape (risk sentence, then spine, then territories). The superlative appeared in no draft or variant, including one run that explicitly refused to launder it ("not 'unmatched speed', which smuggles the same claim back in").
- Sacrifice-cannot-be-assumed appeared consistently, often verbatim reasoning: "a refusal I invent costs you nothing."
- Claim-proof alignment surfaced unprompted: "if the real proof points at a different axis, the honest move is to reposition onto that axis."
- Strategic territories were used at every gate without a single fake claim.
- Three-turn arc: interview prioritized proof and sacrifice, all seven facts carried forward with zero re-asking, gates run before the artifact, hero built on the supplied proof.
- Light-mode cap held (3 rewrites, under 250 words). Naming run delivered 5 tagged candidates with dunk risk. Clean-pass recognized the passing position and wrote the artifact without manufactured weakness.
- Provisional override complied in the same response with correct labeling.

Form: 9/17 responses prefixed internal planning ("This is a light-mode request, the manual says...") before the user-facing content. Partly a harness artifact: the eval prompt asks agents to return their response as a single final message, which invites the preamble. The anti-narration rules are already explicit in SKILL.md; no further rule text was added. Future eval harnesses should instruct: "Do not include planning or notes before the response." Track whether this appears in real installed-skill usage, where planning normally stays in the agent's private reasoning.

No skill changes were made from this run. v0.7 ships as tested.

## Known residual risk

Models tend to open proof-gate responses with procedural preamble despite the rules. Mostly mitigated, not proven eliminated. Judge v0.7 priorities from real positioning jobs, not further synthetic rounds.
