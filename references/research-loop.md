# Research Loop: Assumptions, Statements, Proofs

Read this reference only for research tasks: sketching a model from an intuition, generating variants or minimal examples, attempting a proof, constructing a counterexample, repairing an assumption, or testing extensions, microfoundations, and simplifications.

A theory project searches for a fixed point: defensible assumptions, interesting statements, and proofs that certify them. Any of the three may move. The job is to make each loop cheap, local, and honestly reported.

## Contents

- Run the loop one corner at a time
- Sketch models from an intuition
- Spin off variants and strip to the minimum
- Treat a proof request as a determination
- Attack, repair, and mine failed proofs
- Construct checkable counterexamples
- Separate the prover from the verifier
- Explore several routes independently
- Test extensions, microfoundations, and simplifications
- Report status and hand off cleanly

## Run the loop one corner at a time

Start from the model ledger in [model-and-claim-integrity.md](model-and-claim-integrity.md), or build one from the user's sketch. Then iterate:

1. Fix the current assumptions and the statement to be certified.
2. Attempt a proof or a counterexample.
3. On failure, diagnose which corner is wrong: an assumption too weak, a statement too strong or too trivial, or a proof route that cannot close.
4. Change that one corner (one assumption, one quantifier, one clause) and rerun. Do not redesign the whole model to rescue one step.

Keep a short log of each move: what changed, why, and what it did to the result. The log is the user's record of the search, not part of the manuscript.

## Sketch models from an intuition

When the user supplies a mechanism they believe in but no model, propose two or three minimal models. For each, state:

- primitives: states, signals, actions, types, preferences;
- timing: who knows, chooses, and observes what, and when;
- solution concept: Bayesian, maxmin, rational inattention, dynamic, or another;
- predictions: the comparative statics, testable implications, or examples the model delivers;
- what is elegant, what is fragile, and which theorem would be worth proving.

Prefer the smallest environment in which the mechanism can operate. Do not pad a sketch with generality that has not yet earned its place.

## Spin off variants and strip to the minimum

To generate variants, change one primitive at a time (preferences, information, timing, menu structure, equilibrium concept) and report which comparative statics survive, which flip, and which become ambiguous.

To simplify, strip the model to the smallest example that still delivers the main prediction: two types and two periods, binary states and two actions, or similar. Then list every assumption that survives and what breaks when each is removed. The dependency list is the deliverable; the small model is its evidence.

## Treat a proof request as a determination

"Prove X" reveals the verdict the user wants. Read it as "determine whether X holds under the stated assumptions, then prove or refute it." Do not let the requested direction stand in for evidence, and do not produce a confident argument for a statement whose truth is still open.

Keep proving, refuting, and repairing as separate efforts with separate framing, even within one session. Run them in parallel when independent contexts are available; otherwise finish one before starting the next.

Decompose any non-trivial proof into lemmas that can be checked one at a time. A reduction to a lemma as strong as the original statement is not progress unless it comes with a genuinely new proof of that lemma. Do not call a step routine, standard, or immediate unless it has been verified in the present setting.

## Attack, repair, and mine failed proofs

**Attack.** Read the proof as a hostile referee. Identify the weakest step: an unverified interchange of limits or quantifiers, an existence claim without a construction, a boundary or tie case, a measurability or regularity condition used but not assumed, an off-path belief never specified, a fixed-point argument whose hypotheses are not checked.

**Repair.** When the statement is false or the route cannot close, ask which added or strengthened assumption rescues it, and whether that assumption is economically defensible and still leaves the result interesting. Propose the weakest such assumption and say what it excludes.

**Inspiration.** A wrong proof can still identify the attractive route, expose a hidden assumption, or name a missing lemma. Mine it: extract the route and the lemma, state them as open, and attempt them separately. Do not carry any conclusion from a failed proof into the deliverable.

## Construct checkable counterexamples

A counterexample is hard to find and easy to check; prefer it to a vague claim that a statement "seems false." Make it explicit: parameter values, type or state spaces, strategies or allocations, and the computation showing that every hypothesis holds and the conclusion fails. Verify the hypotheses that look innocuous as carefully as the ones that look binding. When the example can be computed, compute it.

Record which assumption the counterexample defeats. That is the corner of the fixed point that cannot move.

## Separate the prover from the verifier

Never let the context that produced a proof grade it. When an independent subagent or fresh context is available:

1. Run the prover and set its output aside unread.
2. Hand the output to a verifier that sees the statement, the assumptions, and the proof, but not the prover's reasoning and not the verdict anyone hopes for. Instruct it to find the weakest step and to return either a concrete gap or a clean pass.
3. If they disagree, either adjudicate with a third context or feed the reported gap back to the prover for one repair round. Repeat until the result clears or the gap is stable.

Only a cleared output enters the deliverable. If no fresh context is available, run the attack checklist explicitly in the current context, say that the check was not independent, and label the result accordingly.

## Explore several routes independently

When several independent contexts can run at once, use them for a diverse portfolio: different formulations, invariants, reductions, or solution concepts. Do not tell most explorers which route currently looks best; early independence prevents collapse onto one attractive but incomplete reduction. Mark a route as blocked when it stalls at a lemma of theorem strength, and reopen it only for a materially new mechanism. Require concrete lemmas, constructions, or counterexamples from each route; discard status reports and optimism.

## Test extensions, microfoundations, and simplifications

Once the machinery exists, ask what else it can do and what it does not need.

- **Extensions:** change information, preferences, timing, menu structure, or equilibrium concept; report which results survive, which flip, and which require new proofs. An extension earns a place in the paper only if it tests the mechanism or establishes a boundary; see the extensions rule in SKILL.md.
- **Microfoundations:** for a reduced-form assumption, ask whether it can be derived from search, attention costs, ambiguity, private signals, or an institutional arrangement. State exactly what the microfoundation adds and which parameters it pins down.
- **Simplifications:** apply the strip-to-minimum procedure above and report the assumption-dependency list.

## Report status and hand off cleanly

Label every claim in the deliverable with one status: proved, refuted by a stated counterexample, conditional on a named added assumption, or open with the exact remaining gap. On failure, return the strongest rigorously established derivation and its precise missing step, not a best-effort narrative or an explanation of why the problem is hard.

Say when a proof step reproduces a known result or technique so the user can cite it; do not present aggregated literature as a new derivation. Say when a step relies on machinery outside the paper's usual toolkit, and give the theorem, source, and exact hypotheses used, so the user can check what they cannot verify by inspection.

When the session has taken a wrong turn, is looping, or must move to a new context, write a self-contained Markdown brief: the problem, the working assumptions, results so far with their status, what was tried, where it failed, and dead ends to avoid. The same brief is the right artifact when the user needs to escalate a blocked step to a stronger model or a coauthor.

The framing and use cases here follow Pietro Ortoleva and Fedor Sandomirskiy, [*AI for Economic Theorists and Mathematicians*](https://markusacademy.substack.com/p/ai-for-economic-theorists-and-mathematicians) (Markus' Academy, 2026).
