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
- Decision status: proposed from human-editor discussion; pending PR review.

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
- Decision status: proposed from human-editor discussion; pending PR review.

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

Editorial placeholder.

- Core sources: TBD by the human editor.
- Supporting sources: TBD by the human editor.
- Sources explicitly deferred: TBD by the human editor.
- `references.bib` update needed: TBD after source approval.

## Source Map Skeleton

| Component | Planned Use | Source or Origin | Source Role | Verification Status |
|---|---|---|---|---|
| Main theoretical component | TBD | TBD | TBD | Not verified |
| Example or empirical pattern | TBD | TBD | TBD | Not verified |
| Figure, code, simulation, or teaching design | TBD | TBD | TBD | Not verified |
| Transition or related extension | TBD | TBD | TBD | Not verified |

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
