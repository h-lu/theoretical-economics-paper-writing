# Research Loop: Assumptions, Statements, Proofs

Read this reference for research tasks: sketching a model from an intuition, generating variants or minimal examples, attempting or checking a proof, constructing a counterexample, repairing an assumption, or testing extensions, microfoundations, and simplifications.

A theory project searches for a fixed point: defensible assumptions, interesting statements, and proofs that certify them. Any of the three may move. Move one at a time, and report the status of every claim.

## Contents

- Run the loop one corner at a time
- Sketch models from an intuition
- Vary, extend, microfound, and strip to the minimum
- Treat a proof request as a determination
- Attack, repair, and mine proofs
- Construct checkable counterexamples
- Separate the prover from the verifier
- Report status and hand off cleanly

## Run the loop one corner at a time

Start from the ledger in SKILL.md, built as far as the material allows; for a sketch from an intuition, build it per candidate model. The loop begins once a candidate model and statement are fixed:

1. Fix the current assumptions and the statement to be certified.
2. Attempt a proof or a counterexample.
3. On failure, diagnose which corner is wrong: an assumption too weak, a statement too strong to prove or too weak to be interesting, or a proof route that cannot close.
4. Change that one corner (one assumption, one quantifier, one clause) and rerun. Do not redesign the whole model to rescue one step.
5. Stop and report when the user's original statement has been decided, when the same corner has moved twice without progress, or when the rescuing assumption would change the economic question.

A requested extension or simplification may move several primitives at once; it is exempt from the one-corner rule but must report every assumption that moved. Keep a short log of each move: what changed, why, and what it did to the result. The log is the user's record of the search, not part of the manuscript.

When the user asked only to check or assess a claim, run the loop through attack and verification, then report the verdict and the exact gap. Offer a repairing assumption as a proposal; do not apply it.

## Sketch models from an intuition

When the user supplies a mechanism they believe in but no model, propose two or three minimal models. For each, state:

- primitives: states, signals, actions, types, preferences;
- timing: who knows, chooses, and observes what, and when;
- solution concept (Nash, Bayesian, perfect Bayesian, competitive, or another) and the preference, information, or updating model that carries the departure;
- predictions: the comparative statics, testable implications, or examples the model delivers;
- what is elegant, what is fragile, and which theorem would be worth proving.

Prefer the smallest environment in which the mechanism can operate. Do not pad a sketch with generality that has not yet earned its place. Label proposed assumptions as proposals, not as the user's. Name the nearest existing models when you know them, and say when you have not searched.

## Vary, extend, microfound, and strip to the minimum

Once machinery exists, ask what else it can do and what it does not need.

- **Variants and extensions:** change one primitive at a time (preferences, information, timing, menu structure, horizon, equilibrium concept) and report which results survive, which flip, which become ambiguous, and which need new proofs. Under multiplicity, say whether a result survives in every equilibrium, some equilibrium, or a selected branch. An extension earns a place in the paper only if it tests the mechanism or establishes a boundary; see "Use extensions and quantitative material diagnostically" in SKILL.md.
- **Microfoundations:** for a reduced-form assumption, ask whether it can be derived from search, attention costs, ambiguity, private signals, or an institutional arrangement. State exactly what the microfoundation adds and which parameters it pins down.
- **Simplifications:** strip the model to the smallest example that still delivers the main prediction (two types and two periods, binary states and two actions, or similar). Then list every assumption that survives and what breaks when each is removed. The dependency list is the deliverable; the small model is its evidence.

## Treat a proof request as a determination

"Prove X" reveals the verdict the user wants. Read it as "determine whether X holds under the stated assumptions, then prove or refute it," and say that you are doing so. Do not let the requested direction stand in for evidence, and do not produce a confident argument for a statement whose truth is still open.

Keep proving, refuting, and repairing as separate efforts. Do not blend them in one argument. Run them in separate contexts when possible, each seeded only with the statement, the assumptions, and the source, not with each other's output or the hoped-for verdict. When a proof attempt stalls, switch explicitly to refutation and say so.

Decompose any non-trivial proof into lemmas that can be checked one at a time. A reduction to a lemma as strong as the original statement is not progress unless it comes with a genuinely new proof of that lemma. Do not call a step routine, standard, or immediate unless it has been verified in the present setting.

When several contexts can run at once, give each a different route (formulation, invariant, reduction, or solution concept) and withhold which one currently looks best. Require a lemma, construction, or counterexample from each; discard status reports. Mark a route blocked when it stalls at a lemma of theorem strength, and do not stop after the first wave fails: synthesize what the routes found, then launch new formulations.

## Attack, repair, and mine proofs

**Attack.** Read the proof as a hostile referee, whether you or the user wrote it. Identify the weakest step: an unverified interchange of limits or quantifiers, an existence claim without a construction, a boundary or tie case, a measurability or regularity condition used but not assumed, an off-path belief never specified, a fixed-point argument whose hypotheses are not checked.

**Repair.** When the statement is false or the route cannot close, ask which added or strengthened assumption rescues it, and whether that assumption is economically defensible and still leaves the result interesting. Propose the weakest rescuing assumption you can find, say what it excludes, and do not claim it is minimal unless that is proved.

**Inspiration.** A wrong proof can still identify the attractive route, expose a hidden assumption, or name a missing lemma. Mine it: extract the route and the lemma, state them as open, and attempt them separately. Do not carry the failed proof's conclusion into the deliverable; carry its verified lemmas, labeled.

## Construct checkable counterexamples

Before a long proof attempt, test the statement on small cases or a parameter grid when it can be computed. A failing case is a counterexample candidate; a passing grid is evidence, not proof.

Prefer an explicit counterexample to a claim that a statement "seems false"; it is the cheapest thing for the user to verify. Make it explicit: parameter values, type or state spaces, strategies or allocations, and the computation showing that every hypothesis holds and the conclusion fails. Verify the hypotheses that look innocuous as carefully as the ones that look binding.

Record which hypothesis the counterexample exploits. That hypothesis cannot be dropped, so the repair must strengthen it or weaken the statement.

## Separate the prover from the verifier

Never let the context that produced a proof grade it. This includes you: when you wrote the proof, or when the user's manuscript is the prover, obtain an independent check before reporting a verdict.

When a fresh context or subagent is available:

1. Give the verifier only the statement, the assumptions, and the proof text, not the prover's reasoning and not the verdict anyone hopes for. Ask for the weakest step and either a concrete gap or "no gap found."
2. On a gap, allow at most two repair rounds through the prover. If the same gap survives, report the statement as open with that gap. If prover and verifier disagree about whether a gap is real, adjudicate with a third context.
3. Label a statement proved only after it clears the verifier. Everything else enters the deliverable with its status and the exact gap.

Every brief handed to a prover, verifier, explorer, or adjudicator states the task, the context supplied, the output form, the criterion for success, and whether the recipient is to help, attack, verify, repair, or adjudicate.

If no fresh context is available, run the attack checklist explicitly in the current context, say that the check was not independent, and label the result accordingly.

## Report status and hand off cleanly

Label every claim in the deliverable with one status: proved, refuted by a stated counterexample, conditional on a named added assumption, or open with the exact remaining gap. When the certified statement differs from the one the user posed, show both side by side and mark the user's original as refuted, open, or superseded. On failure, return the strongest rigorously established derivation and its precise missing step, not a best-effort narrative or an explanation of why the problem is hard.

Before calling a result new, search for it as in published-theory-practice.md; if you cannot search, label novelty as unverified. Say when a proof step reproduces a known result or technique so the user can cite it. Say when a step relies on machinery outside the paper's usual toolkit, and give the theorem, source, and exact hypotheses used, so the user can check what they cannot verify by inspection.

When the session has taken a wrong turn, is looping, or must move to a new context, write a self-contained Markdown brief: the problem, the working assumptions, results so far with their status, what was tried, where it failed, and dead ends to avoid. The same brief is the right artifact when the user will hand the blocked step to a coauthor or another model.

The fixed-point framing is due to Guillaume Haeringer; the use cases follow Pietro Ortoleva and Fedor Sandomirskiy, [*AI for Economic Theorists and Mathematicians*](https://markusacademy.substack.com/p/ai-for-economic-theorists-and-mathematicians) (Markus' Academy, 2026).
