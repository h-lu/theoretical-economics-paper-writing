# Model and Claim Integrity

Read this reference only when model primitives, timing, information, equilibrium, proposition scope, proof status, comparative statics, welfare, policy, or claim-bearing prose may change.

The aim is to preserve both formal and economic truth. Keep the audit outside the manuscript unless the user requests it.

## Contents

- Fix a model ledger
- Close the environment
- Match the solution concept to the claim
- Protect proposition scope
- Audit the mechanism separately from the proof
- Check comparative statics
- Check welfare and policy language
- Use imported results accurately
- Preserve computational boundaries
- Check the rewrite seam

## Fix a model ledger

Record only the fields material to the paper:

```text
Question or puzzle:
Agents and types:
Horizon and timing:
Information and beliefs:
Actions, messages, contracts, or mechanisms:
Preferences, technology, resources, and constraints:
Institution or market-clearing rule:
Solution/equilibrium concept and selection:
Parameters and domains:
Main claim and proof status:
Mechanism chain:
Welfare criterion or policy objective:
Source anchors:
What the result does not imply:
```

Anchor each claim to a definition, proposition, proof, computation, or primary source. Use a table only when several cases or versions need comparison.

## Close the environment

Check that the model specifies every object needed to determine behavior and outcomes:

- Give domains for types, actions, states, signals, transfers, prices, and allocations.
- State who observes each object and at what time.
- Make the feasible strategy or contract space consistent with the timing and information.
- Define beliefs on and, when required, off the equilibrium path.
- Account for resource, budget, participation, incentive, promise-keeping, and market-clearing constraints that the claimed outcome uses.
- Distinguish a primitive distribution from an induced distribution and an expected payoff from a realized payoff.
- Do not define an equilibrium object by assuming the existence, uniqueness, measurability, or regularity proved later.

Treat an omitted element as harmless only after showing that it cannot change the relevant choice or equilibrium.

## Match the solution concept to the claim

Write the complete equilibrium conditions before compressing their exposition. Check admissible deviations, optimization at every required information set, belief consistency, clearing or consistency conditions, and any transversality or boundary conditions.

Keep these distinctions explicit:

- equilibrium existence, characterization, uniqueness, and selection;
- a strategy profile, an outcome path, and an outcome distribution;
- on-path behavior and off-path restrictions;
- dominant-strategy, ex post, Bayesian, interim, and ex ante incentive conditions;
- planner allocations, implementable allocations, decentralized equilibria, and observed outcomes;
- stationary equilibria, transition paths, and comparative steady states.

If several equilibria remain, state whether the result holds for every equilibrium, some equilibrium, a selected branch, or only locally around one equilibrium.

## Protect proposition scope

For each affected result, record:

- assumptions and parameter domains;
- quantifier order and the dependence of thresholds or constants;
- whether the conclusion is weak, strict, local, global, generic, almost sure, asymptotic, or numerical;
- whether it concerns actions, allocations, prices, payoffs, distributions, welfare, or implementation;
- whether the status is proved, conditional, conjectural, computational, calibrated, or heuristic.

Trace every clause to the proof or computation that supports it. Check boundary values, ties, zero-probability events, discontinuities, non-convexities, multiple best responses, and empty feasible sets when relevant. Do not generalize from a worked example or a numerical grid.

## Audit the mechanism separately from the proof

Write the proposed chain as:

```text
primitive or institutional change
-> changed feasible set, information, payoff, or incentive
-> behavioral margin or deviation
-> strategic, price, or aggregate feedback
-> equilibrium outcome
-> welfare or distributional consequence, if supported
```

Verify each arrow. A correct derivative or fixed-point argument does not by itself establish the stated economic interpretation. Conversely, a plausible story does not prove the equilibrium claim. Identify competing channels and the assumption or parameter restriction that determines which channel dominates.

## Check comparative statics

Specify the parameter variation and what remains fixed. Distinguish a partial response from the total equilibrium response, and account for endogenous prices, beliefs, participation, entry, constraints, or policy rules that adjust.

Record the equilibrium branch and the sense in which the comparison is valid. Do not turn a local derivative into a global monotonicity result, a weak inequality into a strict one, or a single-crossing argument into uniqueness without the needed conditions. For set-valued equilibria, state the order or selection used for comparison.

## Check welfare and policy language

Name the welfare criterion and its timing: ex ante, interim, ex post, steady state, transition, or discounted path. State the population, weights, transfer treatment, outside options, and whether private and social costs coincide. Separate efficiency, Pareto improvement, distributional effects, revenue, consumer surplus, and the objective of a particular planner.

Before recommending a policy, check feasibility, information requirements, commitment, incentive compatibility, participation, budget balance, implementation, and equilibrium responses. State results conditional on the model rather than presenting them as unconditional claims about the world.

## Use imported results accurately

Read the precise theorem and enough surrounding material to determine which hypotheses matter. Record the version and stable link, plus the theorem number and page when available. Translate objects and assumptions into the manuscript's notation.

Classify the use as:

- **direct:** the objects, domains, and hypotheses match;
- **adapted:** a new restriction, extension, argument, or change of setting is required;
- **inapplicable:** a material hypothesis or object does not match.

Treat an adaptation as part of the present paper's mathematics and prove it. Similar terminology or an informal citation is not evidence of applicability.

## Preserve computational boundaries

For a computed equilibrium or quantitative illustration, record the parameterization, discretization, algorithm, stopping rule, tolerances, initial conditions, branch selection, random seed where relevant, and code version. Check residuals and constraints, not only solver convergence. Test whether the substantive conclusion survives reasonable grids, tolerances, initializations, and nearby parameters.

Call the output illustrative, computational, calibrated, or estimated as appropriate. Do not use it to certify existence, uniqueness, global optimality, or a general comparative static unless an argument establishes that claim.

## Check the rewrite seam

Compare the original and revised claim-bearing passages. Confirm that no primitive, timing clause, information condition, solution concept, selection rule, hypothesis, domain, sign, welfare standard, or proof-status label was lost or altered for style.

If a source proves a weaker statement, an equilibrium condition is missing, the mechanism chain breaks, or the rewrite changes the conclusion, stop that part of the edit. Report the smallest unresolved step and the passages it affects. Do not repair a model or proof gap with prose.
