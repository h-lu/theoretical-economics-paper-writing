---
name: theoretical-economics-paper-writing
description: Do theoretical-economics research and writing. Research tasks: sketch minimal models from an intuition, generate variants and minimal examples, attempt proofs, construct counterexamples, repair assumptions, and test extensions, microfoundations, and simplifications. Writing tasks: design, draft, restructure, or review theory papers for coherent models, faithful claims, transparent mechanisms, credible literature positioning, and field-appropriate exposition. Use for micro theory, games, mechanism or market design, information or contract theory, decision or social-choice theory, political economy, and macro or general-equilibrium theory; including front matter, literature or venue assessment, whole-paper architecture, model timing and information, equilibrium definitions, propositions and proofs, comparative statics, welfare or policy, extensions, quantitative illustrations, referee reports, rewrites, submission builds, and final-PDF review. For mixed or structural papers, use only for the theory component. Do not use for primarily empirical analysis, classroom problems, policy memos without a formal model, pure-mathematics proofs detached from any economic model, or mechanical LaTeX, copyediting, citation-formatting, and bibliography fixes.
---

# Theoretical Economics Paper Writing

## Purpose

Help an economist search for the fixed point of a theory project (defensible assumptions, interesting statements, and proofs that certify them) and then turn the result into a paper whose economic question, model, result, mechanism, and scope can be recovered by a reader. In research work, move one corner of the model at a time and report the exact status of every claim. In writing work, improve the argument and exposition without silently changing the environment, equilibrium concept, proof status, or substantive claim.

## Identify the task mode and match the requested scope

Decide first whether the request is research or writing.

- **Research tasks** ask to sketch, prove, refute, repair, extend, microfound, simplify, or test a model or claim. Assumptions, statements, and proofs are all open to change, but change one corner at a time, keep a record of what moved and why, and never let the direction the user hopes for stand in for evidence. Follow [research-loop.md](references/research-loop.md).
- **Writing tasks** ask to assess, outline, draft, revise, position, or review a manuscript whose model and claims are fixed. Do only the level of work requested. Treat an assessment as read-only, an outline as architecture rather than prose, and a local revision as authority to change only the named passage. Do not redesign the model, add results, rewrite the whole manuscript, or move proofs merely because those changes might help.

When a writing request turns out to require a model or theorem change, separate that research task from the writing task, identify what must be re-proved, and say so before proceeding.

Read the manuscript, project instructions, source files, and authoritative cited results relevant to the task before editing. Preserve unrelated work and any frozen claims, proofs, referee responses, or replication records.

Treat a supplied fragment as a fragment. Do not infer omitted assumptions, equilibrium conditions, proposition content, or proof support from the author's summary. When the necessary source is unavailable, label the affected diagnosis or rewrite as conditional and avoid opening with an unsupported assertion that the missing result "establishes" the claim.

## Load references selectively

Do not read every reference by default.

| Task | Read |
|---|---|
| Model sketching, variants, minimal examples, proof attempts, counterexamples, assumption repair, extensions, microfoundations, simplification, or any task whose answer may change whether a claim is true | [research-loop.md](references/research-loop.md) |
| Model primitives, timing, information, equilibrium, proposition scope, proof status, comparative statics, welfare, policy, or any rewrite that may alter a claim | [model-and-claim-integrity.md](references/model-and-claim-integrity.md) |
| Contribution positioning, venue fit, title, abstract, introduction, related literature, whole-paper architecture, or learning current field register from published papers | [published-theory-practice.md](references/published-theory-practice.md) |
| A field-specific model audit or exposition decision in games, mechanism design, information, contracts, matching, decision/social choice, macro, dynamic, or general-equilibrium theory | [subfield-checks.md](references/subfield-checks.md) |
| A whole-manuscript comprehension test, referee-style report, seminar brief, submission build, or final PDF review | [reader-referee-and-release.md](references/reader-referee-and-release.md) |

For a local prose revision whose economic meaning and formal statement are already fixed, this file is normally enough.

## Reconstruct the economic argument before writing or proving

Privately recover a compact model ledger:

- the economic question or puzzle;
- the agents, institution, horizon, timing, information, actions, and constraints;
- the benchmark and the new friction, information structure, incentive, or institutional feature;
- the solution or equilibrium concept and any selection rule;
- the principal result with its parameter domain and proof status;
- the mechanism from primitives to behavior, equilibrium feedback, and outcome;
- the positive, welfare, distributional, or policy conclusion actually supported;
- the precise difference from the nearest literature.

Infer these items from the project when possible rather than turning the ledger into a questionnaire. If a material item cannot be recovered, identify the smallest missing choice or unsupported step before drafting around it. In a research task the ledger is the object being iterated: record each version as assumptions, statements, or proofs move.

Audit the paper at three levels, in this order:

1. **Formal truth:** Do definitions, assumptions, propositions, proofs, and computations support the stated claim?
2. **Economic truth:** Do timing, information, feasible deviations, incentives, market clearing, beliefs, and the equilibrium concept support the stated mechanism and interpretation?
3. **Contribution truth:** Does the paper's account of novelty match precise comparisons with the closest prior work?

Do not try to repair a failure at an earlier level with more confident prose at a later level.

## Design the paper around the economic result

Before a substantial rewrite, prepare a compact architecture containing:

- the question, main result, and mechanism;
- the benchmark and the economically meaningful departure from it;
- the order in which the reader meets agents, timing, information, and constraints;
- the dependency path from primitives to equilibrium to the main propositions;
- the job of each section, example, figure, and extension;
- the division between the main text, formal appendix, online supplement, and material to remove.

Choose the architecture that fits the paper. Do not impose a universal sequence, page count, abstract length, proposition count, or rule that all proofs belong in an appendix. Keep the new economic mechanism and decisive logical bridges visible in the main narrative; move routine or reusable technical work only when the reader can still reconstruct the result.

Use parsimony as a diagnostic rather than a slogan. Ask what each state, type, action, friction, and source of heterogeneity changes in the mechanism, result, or interpretation. Do not simplify away the equilibrium feedback or institutional feature the paper needs to answer its question.

## Present the model as an economic environment

Explain what each modeling object does before asking the reader to manipulate it. Make the order of moves and information sets unambiguous. Distinguish primitives from endogenous objects, strategies from realized actions, beliefs from true distributions, feasibility from optimality, and individual conditions from equilibrium conditions.

Define the solution concept at the level needed for the results. State how multiplicity is handled; do not write as if a correspondence were a unique outcome. Explain the economic role of assumptions, separating substantive restrictions from those used for existence, uniqueness or selection, comparative statics, tractability, or computation.

Use notation when it reduces ambiguity. Prefer agents, choices, incentives, information, constraints, prices, allocations, and beliefs as grammatical subjects. Avoid letting a long block of symbols substitute for the economic environment.

## State results with mechanism and scope

For each important result, make four layers recoverable:

1. the formal statement, with hypotheses, domains, quantifiers, equilibrium branch, and welfare criterion where relevant;
2. the plain-language conclusion;
3. the mechanism: primitive or constraint -> behavioral margin -> best response or clearing effect -> equilibrium outcome;
4. the boundary: what fails, reverses, becomes ambiguous, or remains unproved outside the stated scope.

Test a claimed mechanism against a diagnostic counterfactual: remove or relax the named friction, constraint, or feedback and ask whether the conclusion disappears or changes. If it does not, reconsider whether that feature is actually the driver.

Interpret comparative statics as equilibrium statements, not isolated derivatives, unless the result is genuinely partial. Distinguish local from global, weak from strict, generic from universal, and existence from uniqueness. For welfare or policy claims, name the evaluator, information set, transfer treatment, feasibility and implementation requirements, and affected groups. Keep positive implications separate from normative recommendations.

Give a proof overview when the route is not evident. Identify the decisive economic step and then the technical devices that establish it. Do not call an assumption innocuous, standard, or technical unless its role has been checked. If a cited result requires adaptation, treat the adaptation as part of the paper's mathematics.

## Write front matter after understanding the body

Write the title, abstract, and introduction from the recovered argument rather than from generic motivation. Make the economic question, model departure, principal result, mechanism, and essential scope visible without expanding the contribution. Use the conditional published-practice reference for detailed front-matter or positioning work. Rewrite the title and abstract after the body is stable.

## Use extensions and quantitative material diagnostically

Include an extension when it tests a mechanism, relaxes a consequential assumption, establishes a boundary, or shows portability. Do not accumulate variants that merely add parameters or reproduce the baseline logic.

Label examples, simulations, calibration, estimation, and quantitative counterfactuals by their actual evidentiary status. Record parameter values, algorithms, tolerances, equilibrium selection, and code or data versions when they affect the conclusion. Never present a numerical pattern as a general proposition.

## Revise for an economist-reader

Find the earliest point where a reader loses one of these threads:

- who knows and chooses what, and when;
- which constraint or incentive drives behavior;
- how individual responses aggregate or feed back through equilibrium;
- what the main result says and does not say;
- which assumption carries the economics;
- why the result differs from the closest benchmark or paper.

Repair that break first by deleting, merging, reordering, renaming, or adding a local explanation. Remove repeated motivation, repeated notation, administrative lemmas, and extensions without a distinct economic job before adding more exposition.

After any claim-bearing rewrite, compare the old and new passages and check that no assumption, qualifier, equilibrium selection, welfare standard, sign, domain, proof status, or citation boundary disappeared.

## Finish at the appropriate level

For a research task, label each claim as proved, refuted by a stated counterexample, conditional on a named added assumption, or open with the exact remaining gap; report what was verified independently and which steps the user must still check. For an assessment, return prioritized findings with locations, evidence, and consequences; do not rewrite. For an outline, return the argument map, section architecture, dependency path, and unresolved decisions. For a local draft, verify the affected claims and read the passage in context. For a literature or positioning task, report the compared sources and versions, the relevant comparison dimensions, the supported delta, unresolved uncertainty, and the search boundary. For a full rewrite, check the entire claim map, cross-references, bibliography links, compilation, and rendered PDF. For a referee or reader task, use the conditional reference's independent-reader protocol.

State exactly what was checked. Do not claim that the model is correct, a proof is complete, the results are novel, the paper is understood by the field, the venue is suitable, or acceptance is likely unless the available evidence supports that narrower conclusion.
