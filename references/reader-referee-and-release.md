# Reader, Referee, and Release Checks

Read this reference only for a whole-manuscript comprehension task, referee-style report, seminar brief, submission build, or final PDF review.

## Test whether the economic argument can be recovered

Prepare a self-contained brief in the user's requested language and at the requested level. Cover the argument rather than reproducing the section order:

1. the economic question or puzzle;
2. the environment, timing, information, and solution concept;
3. the benchmark and the model's consequential departure;
4. the principal result in readable form and then its exact scope;
5. the mechanism from incentives to equilibrium;
6. the hardest formal or economic bridge;
7. the welfare, distributional, policy, or empirical implication actually supported;
8. the closest literature and precise difference;
9. the main boundary, alternative channel, or unproved claim.

Use equations, timing diagrams, examples, or figures only when they shorten the reconstruction. Do not turn the brief into a list of proposition numbers.

Locate the earliest cognitive break. Typical breaks occur when the reader cannot tell who observes a variable, why a deviation is feasible, which equilibrium is being selected, how a partial response becomes an equilibrium effect, or which assumption produces the mechanism. Repair that point before polishing later prose.

## Run a cold-reader test

When an independent subagent or fresh context is safely available, provide only the manuscript or relevant artifact and ask the reader to answer:

- What is the economic question?
- Who knows and chooses what, and when?
- What is the equilibrium or solution concept?
- What is the main result and its domain?
- Which incentive, constraint, or feedback generates it?
- Which assumption is economically essential?
- What is not claimed?
- How does the result differ from the nearest work named in the paper?

Also ask the cold reader to identify ambiguities, hidden assumptions, internal contradictions, and claims whose support it cannot locate. Do not leak the intended diagnosis or answer. Treat success as evidence of recoverability, not as proof of correctness or novelty.

If a fresh context is unavailable, generate the questions and give the user a short protocol for obtaining an independent reading. Do not simulate independence while retaining the full drafting conversation.

## Write a referee-style report

Respect the user's requested role and confidentiality. Separate observations by evidentiary level:

- **Formal:** definitions, equilibrium, theorem scope, proof, and computation.
- **Economic:** question, mechanism, assumption content, welfare, and interpretation.
- **Contribution:** relation to precise prior results and the claimed delta.
- **Exposition:** architecture, notation, local clarity, examples, and appendices.

Lead with a neutral reconstruction of the paper's question, approach, main result, and contribution claim. Then report findings in descending consequence:

- **Blocker:** The model is undefined, a central result may be false, the equilibrium concept does not support the claim, or a required source is inapplicable.
- **Major:** The formal result may survive, but the mechanism, scope, welfare analysis, positioning, or paper architecture requires substantive work.
- **Minor:** A local explanation, notation, ordering, or presentation issue is repairable without changing the result.
- **Unverified:** Available evidence is insufficient; do not silently treat the item as passed.

When several findings need comparison, use:

```text
severity | dimension | location | evidence | consequence | smallest next step
```

Use dimensions such as `FORMAL`, `MODEL`, `EQUILIBRIUM`, `MECHANISM`, `WELFARE`, `LITERATURE`, and `EXPOSITION`. Distinguish a verified error from a suspected gap or request for clarification. Do not recommend rejection or acceptance unless the user explicitly requests a recommendation and supplies the venue standard and sufficient evidence.

## Review the full manuscript as a reader

Check whether an economist can recover:

- the question, benchmark, and principal departure;
- the complete model and order of moves;
- the equilibrium concept and handling of multiplicity;
- the exact main result and mechanism;
- the role of central assumptions;
- the dependency path through the proofs;
- the welfare or policy standard;
- the precise contribution and main limitation.

Check that terminology and notation are stable, definitions precede use, examples remain within theorem scope, all appendix results are called from the main text, and every central literature comparison has a traceable source. Prefer one authoritative location for each assumption, mechanism explanation, and scope boundary.

## Inspect a submission-ready artifact

Identify the authoritative source version, build entry point, target venue, and applicable current author instructions. Build with the project's normal toolchain until citations and cross-references stabilize. Read the log for fatal errors, unresolved references, missing inputs, duplicate labels, font issues, and layout warnings that affect the paper.

Inspect the rendered PDF page by page, not only the source. Check:

- the first page, title, abstract, and introduction;
- model timing, definitions, propositions, proof overviews, and equation breaks;
- tables, figures, notes, captions, legends, and grayscale legibility;
- appendix openings, theorem numbering, bibliography, hyperlinks, and final page;
- anonymization, acknowledgments, supplements, and other venue-specific requirements.

Follow several paths from the main propositions to their definitions, lemmas, proof appendices, computations, and cited sources. Ensure that the paper and its declared supplements contain the material needed to audit the new claims, while allowing standard published results to be cited precisely rather than re-proved.

When a fixed artifact matters, record the source version, PDF page count, build command, and hash. State exactly which checks were run and which were not. Successful compilation, a clean cold read, or a favorable venue comparison does not certify correctness, novelty, external validity, or acceptance.
