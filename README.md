# Theoretical Economics Paper Writing

An Agent Skill for doing economic theory with an agent: sketching minimal models, attempting proofs, constructing counterexamples, repairing assumptions, testing extensions, and then designing, drafting, restructuring, and reviewing the resulting paper. It treats a theory project as a search for a fixed point between defensible assumptions, interesting statements, and proofs that certify them, and it keeps formal claims faithful while making the economic environment, equilibrium concept, mechanism, contribution, and scope recoverable by a reader.

用于经济学理论研究与论文写作的 Agent Skill：从直觉搭最小模型、尝试证明、构造反例、修补假设、检验扩展，再到论文的写作与审查。它把理论研究视为在假设、命题、证明之间寻找不动点，重点处理模型完整性、均衡概念、经济机制、比较静态、福利分析、贡献定位和论文表达，而不是套用固定的“顶刊文风”模板。

## What it does

Every request is first classified as a research task or a writing task.

**Research tasks** move the model. The skill sketches two or three minimal models from a stated intuition, spins off variants one primitive at a time, strips a model to the smallest example that still delivers the prediction, attempts proofs and counterexamples, proposes the weakest assumption that rescues a false statement, and tests extensions, microfoundations, and simplifications. It reads "prove X" as "determine whether X holds", separates the prover from the verifier, and labels every claim as proved, refuted, conditional, or open with its exact gap.

**Writing tasks** keep the model fixed and audit the paper at three distinct levels:

1. **Formal truth** — whether definitions, assumptions, propositions, proofs, and computations support the claim.
2. **Economic truth** — whether timing, information, feasible deviations, incentives, beliefs, clearing conditions, and equilibrium support the interpretation.
3. **Contribution truth** — whether the novelty claim matches precise comparisons with the closest literature.

It supports:

- microeconomic and game theory;
- mechanism and market design;
- information economics and contract theory;
- decision theory and social choice;
- political-economy, industrial-organization, and network theory;
- macroeconomic, dynamic, and general-equilibrium theory;
- the theoretical backbone of mixed or structural papers;
- titles, abstracts, introductions, literature positioning, referee reports, submission builds, and final-PDF review.

It is not intended for primarily empirical identification or data analysis, classroom exercises, policy memos without a formal model, detached pure-mathematics proofs, or mechanical LaTeX and bibliography maintenance.

## Core workflow

Research tasks iterate the fixed-point loop, changing one corner at a time:

```text
assumptions <-> statements <-> proofs
   |
   +-- attempt a proof or a counterexample
   +-- on failure, diagnose the corner that is wrong
   +-- change one assumption, quantifier, or clause; rerun
   +-- verify independently; report each claim's status and remaining gap
```

Both modes reconstruct a private model ledger before substantial work:

```text
economic question
-> agents, timing, information, actions, and constraints
-> benchmark and consequential departure
-> equilibrium concept and selection
-> main result and proof status
-> economic mechanism
-> welfare, policy, or distributional implication
-> precise literature delta
```

Results are explained through a mechanism chain:

```text
primitive or constraint
-> affected behavioral margin
-> best response, strategic response, or clearing feedback
-> equilibrium outcome
-> welfare or distributional consequence, when supported
```

## Repository structure

```text
.
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    ├── research-loop.md
    ├── model-and-claim-integrity.md
    ├── published-theory-practice.md
    ├── reader-referee-and-release.md
    └── subfield-checks.md
```

`SKILL.md` contains the high-frequency workflow. The reference files are loaded only when the task requires the research loop, deeper model auditing, literature positioning, subfield-specific checks, or whole-manuscript review.

## Installation

Install as a personal Codex skill:

```bash
git clone https://github.com/h-lu/theoretical-economics-paper-writing.git ~/.codex/skills/theoretical-economics-paper-writing
```

Or install inside a repository:

```bash
mkdir -p .codex/skills
git clone https://github.com/h-lu/theoretical-economics-paper-writing.git .codex/skills/theoretical-economics-paper-writing
```

Restart or reload the agent environment if it does not discover the skill immediately.

## Example prompts

```text
Use $theoretical-economics-paper-writing. I suspect polarization can arise from
costly attention to policy dimensions. Give me three minimal models that capture
this, and for each say what is elegant, what is fragile, and what theorem would
be worth proving.
```

```text
Use $theoretical-economics-paper-writing to decide whether Theorem 1 still holds
without the regularity assumption: prove it or construct a counterexample, and
if it fails, propose the weakest assumption that rescues it.
```

```text
Use $theoretical-economics-paper-writing to strip this model to two types and
two periods, then list every surviving assumption and what breaks when each is
removed.
```

```text
Use $theoretical-economics-paper-writing to audit whether the off-path beliefs
in this signaling model support the claimed perfect Bayesian equilibrium.
```

```text
Use $theoretical-economics-paper-writing to rewrite this mechanism-design
introduction without expanding the contribution or changing the theorem scope.
```

```text
Use $theoretical-economics-paper-writing to review the comparative statics and
welfare analysis in this recursive competitive-equilibrium model.
```

```text
Use $theoretical-economics-paper-writing to prepare a referee-style report that
separates formal, economic, contribution, and exposition issues.
```

## Design principles

- Preserve task scope: an assessment does not authorize a rewrite, and a research task moves one corner of the model at a time.
- Never let the context that produced a proof grade it; a requested verdict is not evidence.
- Treat model logic and citations as low-freedom, evidence-bound work.
- Keep paper architecture adaptable to the economic question.
- Avoid universal quotas for pages, abstract length, propositions, or appendix placement.
- Use current primary literature for contribution and venue judgments.
- Require fresh evidence before claiming that a manuscript or artifact passed a check.

The design extends the compact, reference-routed approach of [mathematical-paper-skills](https://github.com/h-lu/mathematical-paper-skills) with economics-specific checks for timing, information, equilibrium multiplicity, comparative statics, welfare, implementation, and quantitative boundaries. The research loop follows Pietro Ortoleva and Fedor Sandomirskiy's Markus' Academy mini-series [*AI for Economic Theorists and Mathematicians*](https://markusacademy.substack.com/p/ai-for-economic-theorists-and-mathematicians) (2026): theory as a fixed point of assumptions, statements, and proofs (a framing they credit to Guillaume Haeringer); sketch, attack, repair, and inspiration as the high-value uses; prover separated from verifier; LaTeX in, never PDF.

## License

[MIT](LICENSE)
