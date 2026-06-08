# Chapter 1a Content Architecture

This document is the internal editorial architecture artifact for `v0.2-alpha`.
It is not the learner-facing notebook draft.

No full 1a notebook prose is being written in this milestone. This scaffold records
the structure required for later human-reviewed decisions about notebook 1a.

## Human Brief

Editorial placeholder.

- Purpose: TBD by the human editor.
- Intended learner value: TBD by the human editor.
- Editorial constraints: Do not write learner-facing notebook prose here.

## Core Question

- Proposed core question: What does expected utility provide as a baseline
  model of risky choice, and what do its failures reveal about the limits of
  explaining risky choice through final wealth?
- Decision status: approved through merged PR #26 for issue #17.

## Storyline

- Main 1a storyline: Notebook 1a first introduces expected utility as the
  baseline model that turns risky choice into the evaluation of lotteries
  through expected utility over final wealth. It then shows that this baseline
  is powerful but too coarse for several central patterns of risky choice.
  Small-stakes risk aversion reveals that final-wealth curvature cannot
  plausibly explain ordinary local risk attitudes. Samuelson's aggregation
  paradox shows that the unit in which a risk is evaluated, isolated gamble
  versus aggregated sequence, matters for choice. The common consequence and
  common ratio versions of the Allais paradox show that EU's independence
  structure fails in important lottery comparisons. The notebook ends by
  organizing these failures as unresolved diagnoses, with at most a brief
  roadmap sentence noting that later notebooks will ask how alternative models
  address these problems.
- Core failure sequence:
  1. Expected utility baseline: explain what EU is, where it comes from, and
     what problem it solves, but keep this setup short.
  2. Small-stakes risk aversion: use Rabin-style calibration as the main
     diagnostic that final-wealth curvature is the wrong explanation for
     ordinary local risk attitudes.
  3. Samuelson aggregation paradox: emphasize that the evaluation unit matters;
     the same gamble can be evaluated differently when framed as one isolated
     risk versus an aggregated or repeated sequence.
  4. Allais paradoxes: treat Allais as the third core failure family, parallel
     to small-stakes risk aversion and Samuelson aggregation. Its common
     consequence and common ratio versions should sit one level below the
     Allais family and should show that EU's independence structure fails in
     important lottery comparisons.
- Decision status: approved through merged PR #26 for issue #17.

## Content Boundaries

- Included in 1a:
  - A short setup of expected utility as the baseline model of risky choice.
  - Small-stakes risk aversion as the first core failure.
  - Samuelson's aggregation paradox as the second core failure.
  - The common consequence and common ratio versions of the Allais paradox as
    the third core failure family.
  - A concise synthesis of what each failure notices about the limits of
    expected utility.
- Alternative EU failures: Do not name or open additional EU-failure topics in
  the current 1a architecture. Future versions may add them if the human editor
  reopens the boundary decision, but the current beta path should use only the
  three approved diagnostics.
- Deferred to 1b: Building reference-dependent preferences, exogenous
  reference points, and loss aversion as a model.
- Deferred to 1c: Expectations-based or endogenous reference points.
- Deferred to 1d: Probability weighting and related detailed probability-side
  explanations.
- Non-goals:
  - Do not write learner-facing 1a notebook prose in this milestone.
  - Do not turn 1a into a broad survey of non-EU models.
  - Do not present reference points, loss aversion, probability weighting, or
    any other later model as the answer to 1a's diagnoses.
  - Do not build prospect theory or cumulative prospect theory inside 1a.
  - Do not make Allais a bridge to probability weighting in 1a.

## Source Set

The approved 1a source set is intentionally limited to sources needed by the
approved storyline: expected utility baseline, small-stakes risk aversion,
Samuelson aggregation, and Allais independence failure.

The 1a-specific bibliography file is `references/ch01_1a.bib`. The top-level
`references.bib` file may remain as a shared or legacy project bibliography, but
1a source approval is tracked here and in `references/ch01_1a.bib`.

New beta-stage 1a core sources require human editor approval in the linked issue
or pull request before they are added to the notebook draft.

| Source | Planned Use | Source Role | Verification Status |
|---|---|---|---|
| Bernoulli 1738 | Anchor the historical expected-utility move from expected value toward utility-based risk evaluation. | core | Selected from human-supplied reference list; entry added to `references/ch01_1a.bib`. |
| Bernoulli 1954 | Provide the readable English translation for the Bernoulli introduction and St. Petersburg discussion. | support | Selected from human-supplied reference list; entry added to `references/ch01_1a.bib`. |
| von Neumann and Morgenstern 1944 | Anchor the modern expected-utility baseline over lotteries. | core | Selected from human-supplied reference list; entry added to `references/ch01_1a.bib`. |
| Mas-Colell, Whinston, and Green 1995 | Provide a standard textbook reference for lotteries, preferences, and expected-utility representation. | support | Selected from human-supplied reference list; entry added to `references/ch01_1a.bib`. |
| Pratt 1964 | Support the distinction between risk aversion in the small and in the large without turning it into a technical teaching unit. | support | Selected from human-supplied reference list; entry added to `references/ch01_1a.bib`. |
| Rabin 2000 | Carry the small-stakes calibration diagnosis against final-wealth curvature. | core | Selected from human-supplied reference list; entry added to `references/ch01_1a.bib`. |
| Rabin and Thaler 2001 | Provide teaching support for the economic intuition behind the Rabin calibration result. | support | Selected from human-supplied reference list; entry added to `references/ch01_1a.bib`. |
| Samuelson 1952 | Support the role of the independence axiom in the expected-utility structure used by the Allais diagnosis. | support | Selected from human-supplied reference list; entry added to `references/ch01_1a.bib`. |
| Samuelson 1963 | Carry the aggregation or fallacy-of-large-numbers diagnosis. | core | Selected from human-supplied reference list; entry added to `references/ch01_1a.bib`. |
| Allais 1953b | Carry the common consequence and common ratio diagnosis of independence failure. | core | Selected from human-supplied reference list; entry added to `references/ch01_1a.bib`. |
| Markowitz 1952 | Support the narrow point that wealth-utility shape is not simply a global concavity story. | support | Selected from human-supplied reference list; entry added to `references/ch01_1a.bib`. |
| Friedman and Savage 1948 | Provide optional background on classic wealth-utility explanations of risk attitudes. | extension | Selected from human-supplied reference list; entry added to `references/ch01_1a.bib`. |

Boundary note: prospect theory, reference-dependent preferences, probability
weighting, rank-dependent utility, subjective expected utility, experimental
elicitation methods, behavioral-economics surveys, and reference-dependent
applications are not part of the approved 1a source set unless the human editor
reopens the source decision.

## Source Map Skeleton

| Component | Planned Use | Source or Origin | Source Role | Verification Status |
|---|---|---|---|---|
| Expected utility introduction | Move from expected value toward utility-based risk evaluation and motivate why EU is the natural baseline. | Bernoulli 1738; Bernoulli 1954 | core; support | Entries added to `references/ch01_1a.bib`. |
| Modern EU baseline | Define the expected-utility benchmark over lotteries at the level needed for 1a. | von Neumann and Morgenstern 1944; Mas-Colell, Whinston, and Green 1995 | core; support | Entries added to `references/ch01_1a.bib`. |
| Wealth curvature background | Explain why risk aversion is usually represented through utility curvature, without expanding into a full risk-aversion theory. | Pratt 1964; Markowitz 1952; Friedman and Savage 1948 | support; support; extension | Entries added to `references/ch01_1a.bib`. |
| Small-stakes risk aversion | Show that final-wealth curvature cannot plausibly explain ordinary local risk attitudes. | Rabin 2000; Rabin and Thaler 2001 | core; support | Entries added to `references/ch01_1a.bib`. |
| Aggregation paradox | Show that the evaluation unit matters: an isolated gamble and an aggregated sequence need not receive the same treatment. | Samuelson 1963 | core | Entry added to `references/ch01_1a.bib`. |
| Independence failure | Show that common consequence and common ratio comparisons expose the independence-structure failure. | Allais 1953b; Samuelson 1952 | core; support | Entries added to `references/ch01_1a.bib`. |
| Figure, code, simulation, or teaching design | Use project-generated examples only if they directly illustrate one approved diagnostic. | Almost Behavioral Economics original implementation | original | No external source required unless the component adapts a listed source. |

## Notebook Section Outline

Map the approved architecture to the English notebook template. Keep this as an
outline until the v0.2-beta learner-facing notebook draft begins.

| Notebook Template Section | Planned 1a Role | Drafting Status |
|---|---|---|
| Abstract | TBD | Not drafted |
| Learning Goals | TBD | Not drafted |
| Prerequisites | TBD | Not drafted |
| Opening Problem | TBD | Not drafted |
| Baseline Model | TBD | Not drafted |
| Key Tension | TBD | Not drafted |
| Core Idea | TBD | Not drafted |
| Guided Example / Experiment | TBD | Not drafted |
| What This Teaches Us | TBD | Not drafted |
| Key Takeaways | TBD | Not drafted |
| Glossary | TBD | Not drafted |
| Source Map | TBD | Not drafted |
| References | TBD | Not drafted |
| Related | TBD | Not drafted |

## Component Plan

Editorial placeholder.

- Examples: TBD by the human editor.
- Figures: TBD by the human editor.
- Code or simulations: TBD by the human editor.
- Glossary entries: TBD by the human editor.
- Citation and reference checks: TBD after source approval.

## 1a to 1b Transition

- How 1a should end: 1a ends by organizing the failures of expected utility as
  unresolved diagnoses. It should not present a new model, derive reference
  dependence, or make a solution claim.
- Allowed roadmap sentence: 1a may include one brief navigation sentence saying
  that later notebooks will ask how alternative models handle local gains and
  losses, reference points, and probability-side distortions.
- What 1a must not pre-emptively build: 1a must not build reference-dependent
  preferences, exogenous reference points, expectations-based reference points,
  probability weighting, or prospect theory.
