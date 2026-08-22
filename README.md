# Theoretical Economics Paper Writing

An Agent Skill for designing, drafting, restructuring, and reviewing theoretical economics papers. It helps preserve formal claims while making the economic environment, equilibrium concept, mechanism, contribution, and scope recoverable by a reader.

用于经济学理论论文写作与审查的 Agent Skill，重点处理模型完整性、均衡概念、经济机制、比较静态、福利分析、贡献定位和论文表达，而不是套用固定的“顶刊文风”模板。

## What it does

The skill audits a paper at three distinct levels:

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

The skill reconstructs a private model ledger before substantial writing:

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
    ├── model-and-claim-integrity.md
    ├── published-theory-practice.md
    ├── reader-referee-and-release.md
    └── subfield-checks.md
```

`SKILL.md` contains the high-frequency workflow. The reference files are loaded only when the task requires deeper model auditing, literature positioning, subfield-specific checks, or whole-manuscript review.

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

- Preserve task scope: an assessment does not authorize a rewrite.
- Treat model logic and citations as low-freedom, evidence-bound work.
- Keep paper architecture adaptable to the economic question.
- Avoid universal quotas for pages, abstract length, propositions, or appendix placement.
- Use current primary literature for contribution and venue judgments.
- Require fresh evidence before claiming that a manuscript or artifact passed a check.

The design extends the compact, reference-routed approach of [mathematical-paper-skills](https://github.com/h-lu/mathematical-paper-skills) with economics-specific checks for timing, information, equilibrium multiplicity, comparative statics, welfare, implementation, and quantitative boundaries.

## License

[MIT](LICENSE)
