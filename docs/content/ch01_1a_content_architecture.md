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
| Rabin calibration example | Use a small favorable 50-50 gamble and a calibration implication table to show why final-wealth curvature cannot plausibly explain ordinary local risk attitudes. | Rabin 2000; Rabin and Thaler 2001; Almost Behavioral Economics original teaching table | core; support; original | Static teaching component approved for beta planning; exact prose and final numerical detail remain beta-stage work. |
| Samuelson aggregation contrast | Use an isolated-gamble row and a minimal aggregated-sequence distribution table to show that the evaluation unit matters. | Samuelson 1963; Almost Behavioral Economics original teaching table | core; original | Static teaching component approved for beta planning; exact distribution formatting remains beta-stage work. |
| Allais comparison tables | Use one two-part lottery table for common consequence and common ratio comparisons, with normalized abstract payoffs, to expose the independence-structure failure. | Allais 1953b; Samuelson 1952; Almost Behavioral Economics original teaching table | core; support; original | Static teaching component approved for beta planning; exact payoff normalization remains beta-stage work. |
| Lightweight dynamic table | Allow a beta-stage toggle or expandable table only if it directly clarifies an approved diagnostic and has a complete static fallback. | Almost Behavioral Economics original implementation | original | Optional; not required for beta. |
| Code, widgets, simulations, summary figure, or full proofs | Do not carry these forward by default. They may be reconsidered only if the human editor reopens the component decision. | Not needed | not needed | Explicitly excluded from beta planning by default. |

## Notebook Section Outline

Map the approved architecture to the English notebook template. Keep this as a
high-granularity outline until the v0.2-beta learner-facing notebook draft
begins. The outline may name planned points, questions, source dependencies, and
expected outputs, but it must not become full notebook prose.

### Abstract

- Diagnostic route summary
  - Purpose: preview the notebook's path from expected utility as the risky-choice
    baseline to the three approved diagnoses of its limits.
  - Main claim or question: expected utility is a powerful baseline, but
    small-stakes risk aversion, aggregation, and Allais-style comparisons expose
    limits of final-wealth expected utility.
  - Source dependence: approved storyline from issue #17; approved source-set and
    boundary decisions from issues #18 and #19.
  - Expected output: a short beta-stage summary of the route, not a full argument
    or solution claim.

### Learning Goals

- Explain the minimal expected-utility baseline
  - Purpose: set the learner expectation that 1a starts from EU as the benchmark.
  - Main claim or question: how does EU evaluate risky choices through lotteries,
    probabilities, and utility over final wealth?
  - Source dependence: Bernoulli 1738; Bernoulli 1954; von Neumann and
    Morgenstern 1944; Mas-Colell, Whinston, and Green 1995.
  - Expected output: one ability target about explaining the minimal EU baseline.
- Identify the small-stakes risk-aversion problem
  - Purpose: make Rabin-style calibration one of the explicit learner outcomes.
  - Main claim or question: why is final-wealth curvature implausible as an
    explanation for ordinary local risk aversion?
  - Source dependence: Pratt 1964; Rabin 2000; Rabin and Thaler 2001.
  - Expected output: one ability target about recognizing the small-stakes
    diagnosis.
- Distinguish isolated from aggregated risk evaluation
  - Purpose: make Samuelson's aggregation diagnosis a separate learner outcome.
  - Main claim or question: why can the unit of risk evaluation matter for choice?
  - Source dependence: Samuelson 1963.
  - Expected output: one ability target about comparing isolated and aggregated
    gambles.
- Explain the Allais pressure on independence
  - Purpose: make the Allais family a separate learner outcome without turning
    1a into probability weighting.
  - Main claim or question: how do common consequence and common ratio comparisons
    challenge EU's independence structure?
  - Source dependence: Allais 1953b; Samuelson 1952.
  - Expected output: one ability target about the Allais independence diagnosis.

### Prerequisites

- Introductory microeconomics: utility, preferences, marginal reasoning.
- Probability theory / statistics basics: probabilities, expected value, simple
  lotteries.
- Basic calculus: curvature and concavity intuition.
- Mathematical notation for models: simple equations and payoff-probability
  tables.

No prior behavioral economics is required.

### Opening Problem

- Motivation for testing the baseline
  - Purpose: create the reason to examine EU's limits before introducing the
    formal baseline.
  - Main claim or question: if EU is the standard baseline for risky choice, can
    it explain ordinary risk attitudes, aggregation judgments, and classic
    lottery-choice reversals?
  - Source dependence: approved storyline from issue #17; light baseline context
    from Bernoulli 1738, Bernoulli 1954, and von Neumann and Morgenstern 1944 if
    needed.
  - Expected output: a short motivational opening that names the three challenge
    directions without working through them.

### Baseline Model

- Expected value to expected utility
  - Purpose: establish why utility enters a model of risky choice.
  - Main claim or question: expected value is too crude when outcomes differ in
    utility, so the baseline evaluates expected utility rather than expected
    monetary value alone.
  - Source dependence: Bernoulli 1738; Bernoulli 1954.
  - Expected output: compact historical and conceptual setup, not a long
    treatment of the St. Petersburg problem.
- Modern lottery representation
  - Purpose: define the minimal benchmark used by the later diagnoses.
  - Main claim or question: EU evaluates lotteries through probabilities and
    utilities over final wealth.
  - Source dependence: von Neumann and Morgenstern 1944; Mas-Colell, Whinston,
    and Green 1995.
  - Expected output: concise model statement with only equations that clarify the
    later argument.
- Wealth curvature as the standard risk-aversion explanation
  - Purpose: set up the final-wealth curvature account that the first diagnosis
    will pressure.
  - Main claim or question: concavity of utility over final wealth is the standard
    EU representation of risk aversion, but 1a should keep this background short.
  - Source dependence: Pratt 1964; Markowitz 1952; Friedman and Savage 1948.
  - Expected output: bounded curvature setup without expanding into a full
    risk-aversion theory.

### Key Tension

- Final-wealth curvature versus local risk attitudes
  - Purpose: preview the first diagnostic tension.
  - Main claim or question: can global utility curvature explain ordinary
    small-stakes risk aversion without implausible large-stakes implications?
  - Source dependence: Rabin 2000; Rabin and Thaler 2001.
  - Expected output: short tension statement that prepares the guided example.
- Isolated gamble versus aggregated sequence
  - Purpose: preview the second diagnostic tension.
  - Main claim or question: why might a gamble rejected in isolation look
    different when evaluated as part of a repeated or aggregated sequence?
  - Source dependence: Samuelson 1963.
  - Expected output: short tension statement that keeps the evaluation-unit issue
    distinct from curvature.
- Independence structure versus Allais comparisons
  - Purpose: preview the third diagnostic tension.
  - Main claim or question: why do common consequence and common ratio comparisons
    put pressure on EU's independence structure?
  - Source dependence: Allais 1953b; Samuelson 1952.
  - Expected output: short tension statement that does not turn Allais into a
    probability-weighting lesson.

### Core Idea

- Three diagnoses, not three isolated curiosities
  - Purpose: organize the approved failures into one conceptual lens before the
    examples.
  - Main claim or question: small-stakes risk aversion, aggregation, and Allais
    comparisons diagnose different limits of EU: curvature, evaluation unit, and
    independence.
  - Source dependence: approved storyline from issue #17; approved boundaries
    from issue #19.
  - Expected output: an organizing frame for the rest of 1a, not a new model.
- No solution model inside 1a
  - Purpose: protect the boundary between diagnosis in 1a and later model
    construction.
  - Main claim or question: what should 1a leave unresolved rather than explain
    with reference dependence, loss aversion, or probability weighting?
  - Source dependence: content-boundary decision from issue #19.
  - Expected output: a clear diagnostic stance that may support a brief roadmap
    sentence later.

### Guided Example / Experiment

- Rabin-style small-stakes calibration check
  - Purpose: show why final-wealth curvature cannot plausibly carry ordinary
    local risk aversion.
  - Main claim or question: what large-stakes implications follow if EU curvature
    is calibrated to reject modest favorable gambles?
  - Source dependence: Rabin 2000; Rabin and Thaler 2001; Pratt 1964 as
    background.
  - Expected output: planned example slot for the small-stakes diagnosis; exact
    numbers, figures, code, or widgets belong to issue #21.
- Samuelson aggregation contrast
  - Purpose: show that the evaluation unit matters for risky choice.
  - Main claim or question: how can the same type of gamble look different when
    considered alone versus as part of an aggregated sequence?
  - Source dependence: Samuelson 1963.
  - Expected output: planned example slot for isolated-versus-aggregated
    evaluation; exact design choices belong to issue #21.
- Allais common consequence and common ratio comparisons
  - Purpose: show that the Allais family pressures the independence structure of
    EU.
  - Main claim or question: how do common consequence and common ratio comparisons
    reveal the independence failure?
  - Source dependence: Allais 1953b; Samuelson 1952.
  - Expected output: planned example slot for the Allais diagnosis; exact lottery
    tables, figures, or code belong to issue #21.

### What This Teaches Us

- Curvature diagnosis
  - Purpose: synthesize what the small-stakes example adds beyond the baseline
    model.
  - Main claim or question: final-wealth curvature is too coarse to explain
    ordinary local risk attitudes.
  - Source dependence: Rabin 2000; Rabin and Thaler 2001; Pratt 1964.
  - Expected output: short synthesis target, not a takeaway list.
- Evaluation-unit diagnosis
  - Purpose: synthesize what the aggregation example adds.
  - Main claim or question: risk evaluation can depend on whether a gamble is
    considered in isolation or as an aggregate.
  - Source dependence: Samuelson 1963.
  - Expected output: short synthesis target, distinct from the final key
    takeaways.
- Independence diagnosis
  - Purpose: synthesize what the Allais example adds.
  - Main claim or question: EU's independence structure is vulnerable in classic
    lottery comparisons.
  - Source dependence: Allais 1953b; Samuelson 1952.
  - Expected output: short synthesis target that does not introduce probability
    weighting.
- Ending stance for later notebooks
  - Purpose: explain why the notebook ends with unresolved diagnoses.
  - Main claim or question: how should 1a close the parallel diagnoses while
    leaving later notebooks to continue the chapter's model-building work?
  - Source dependence: content-boundary decision from issue #19.
  - Expected output: bounded ending logic and light chapter navigation.

### Key Takeaways

Key takeaways should mirror the learning goals as conclusion-style statements,
not repeat the learning goals as ability statements. They should not introduce
new claims; they should compress the prior synthesis.

- Expected-utility baseline
  - Purpose: close the baseline thread.
  - Main claim or question: EU is the baseline model for risky choice, not the
    endpoint of the chapter's explanation.
  - Source dependence: Bernoulli 1738; Bernoulli 1954; von Neumann and
    Morgenstern 1944; Mas-Colell, Whinston, and Green 1995.
  - Expected output: one concise conclusion-style takeaway.
- Small-stakes diagnosis
  - Purpose: close the curvature thread.
  - Main claim or question: final-wealth curvature cannot plausibly explain
    ordinary small-stakes risk aversion.
  - Source dependence: Rabin 2000; Rabin and Thaler 2001.
  - Expected output: one concise conclusion-style takeaway.
- Aggregation diagnosis
  - Purpose: close the evaluation-unit thread.
  - Main claim or question: the unit of evaluation matters for risky choice.
  - Source dependence: Samuelson 1963.
  - Expected output: one concise conclusion-style takeaway.
- Independence diagnosis
  - Purpose: close the Allais thread.
  - Main claim or question: Allais-style comparisons pressure EU's independence
    structure.
  - Source dependence: Allais 1953b; Samuelson 1952.
  - Expected output: one concise conclusion-style takeaway.

### Glossary

List candidate glossary terms only; do not write definitions in this outline.

- expected utility
- lottery
- final wealth
- risk aversion
- utility curvature
- small-stakes risk aversion
- aggregation
- independence axiom
- common consequence
- common ratio

### Source Map

- Expected-utility baseline components
  - Purpose: map the baseline setup to its approved sources.
  - Main claim or question: which sources support the historical and modern EU
    benchmark?
  - Source dependence: Bernoulli 1738; Bernoulli 1954; von Neumann and
    Morgenstern 1944; Mas-Colell, Whinston, and Green 1995.
  - Expected output: source-map rows for the expected-value-to-utility move and
    the modern lottery benchmark.
- Wealth-curvature background
  - Purpose: map the risk-aversion background without expanding it into a full
    theory unit.
  - Main claim or question: which sources support the limited curvature setup?
  - Source dependence: Pratt 1964; Markowitz 1952; Friedman and Savage 1948.
  - Expected output: source-map row for bounded curvature background.
- Approved diagnostic examples
  - Purpose: map each diagnostic example to the approved source set.
  - Main claim or question: which source carries each of the three approved
    failure diagnoses?
  - Source dependence: Rabin 2000; Rabin and Thaler 2001; Samuelson 1963; Allais
    1953b; Samuelson 1952.
  - Expected output: source-map rows for small-stakes risk aversion, aggregation,
    and independence failure.
- Original teaching design
  - Purpose: reserve space for project-generated examples, figures, code, or
    simulation design if issue #21 approves them.
  - Main claim or question: what original components directly illustrate an
    approved diagnostic?
  - Source dependence: Almost Behavioral Economics original implementation.
  - Expected output: source-map row for original teaching design, used only if
    the beta draft includes such components.

### References

- Approved source-set reference list
  - Purpose: ensure the beta draft's references stay tied to cited, mentioned,
    or used sources.
  - Main claim or question: which approved 1a sources were actually used in the
    notebook?
  - Source dependence: `references/ch01_1a.bib`; source-set decision from issue
    #18.
  - Expected output: references section limited to sources actually cited,
    mentioned, or used in the beta draft, with new core sources requiring human
    editor approval.

### Related

- Later reference-dependent models
  - Purpose: identify a conceptually related later direction without explaining
    it inside 1a.
  - Main claim or question: should the beta draft briefly point to later
    reference-dependent treatments of local gains, losses, and reference points?
  - Source dependence: content-boundary decision from issue #19.
  - Expected output: possible related-direction note for 1b and 1c if genuinely
    useful; no concrete link commitment in this outline.
- Later probability-side models
  - Purpose: identify the probability-side follow-up without making Allais a
    probability-weighting lesson.
  - Main claim or question: should the beta draft briefly point to later
    probability-side treatments after the Allais diagnosis?
  - Source dependence: content-boundary decision from issue #19.
  - Expected output: possible related-direction note for 1d if genuinely useful;
    no explanation of probability weighting inside 1a.

## Component Plan

The 1a component plan should use static teaching components by default. Each
component must serve one approved diagnosis in the storyline. Components should
not make 1a into a computational behavioral economics notebook, and components
that are not needed should not be carried into beta by default.

### Required Examples

- Rabin-style calibration example
  - Status: required.
  - Form: static payoff and calibration tables.
  - Pedagogical purpose: show the calibration logic that makes final-wealth
    curvature an implausible explanation for ordinary small-stakes risk
    aversion.
  - Planned design: start from an abstract 50-50 favorable gamble such as
    `lose 100 / gain 110`, then show the small-stakes rejection, the local
    curvature implication, and the resulting implausible large-stakes
    implication.
  - Source or origin: Rabin 2000 as core; Rabin and Thaler 2001 as support;
    project-generated teaching tables as original presentation.
  - Not needed: full theorem proof, general calibration theorem derivation,
    parameter sliders, or simulation.
- Samuelson aggregation contrast
  - Status: required.
  - Form: static isolated-versus-aggregated distribution table.
  - Pedagogical purpose: show that the unit of risk evaluation matters; an
    isolated gamble and an aggregated sequence need not invite the same
    judgment.
  - Planned design: use the Samuelson-style 50-50 structure
    `lose 100 / gain 200`, then contrast one isolated gamble with a minimal
    distribution table for many independent repetitions.
  - Source or origin: Samuelson 1963 as core; project-generated teaching table
    as original presentation.
  - Not needed: full probability derivation, simulation, or interactive
    aggregation widget.
- Allais comparison tables
  - Status: required.
  - Form: one static two-part lottery table.
  - Pedagogical purpose: show that the common consequence and common ratio
    versions of the Allais paradox put pressure on EU's independence
    structure.
  - Planned design: place common consequence in the first part and common ratio
    in the second part, using normalized abstract payoffs rather than historical
    currency labels.
  - Source or origin: Allais 1953b as core; Samuelson 1952 as support for the
    independence axiom; project-generated teaching table as original
    presentation.
  - Not needed: probability-weighting explanation, dynamic calculation, or a
    separate visual for each Allais variant.

### Optional Components

- Lightweight dynamic table
  - Status: optional for beta only.
  - Form: a toggle, expandable table, or other light table interaction.
  - Use condition: include only if it clarifies one approved diagnostic and the
    static version already carries the full argument.
  - Required fallback: the learner-facing notebook must remain complete if the
    dynamic behavior is unavailable.

### Components Not Needed

- Summary figure or summary table: not needed. The three required examples
  should carry the diagnostic structure without an extra synthesis visual.
- Code cells, widgets, simulations, dashboards, and parameter sliders: not
  needed by default. Code may be reconsidered only if the beta draft reveals a
  specific explanatory need.
- Full mathematical proofs: not needed. 1a should teach the diagnostic force of
  the examples, not prove the general theorems.

### Glossary and Citation Checks

- Glossary entries remain the candidate terms listed in the outline unless beta
  drafting reveals that a component requires a new local term.
- Citation and reference checks should verify that adapted component structures
  are tied to Rabin 2000, Rabin and Thaler 2001, Samuelson 1963, Allais 1953b,
  and Samuelson 1952 as planned.

## 1a Ending Stance

- How 1a should end: 1a ends by organizing the three failures of expected
  utility as parallel unresolved diagnoses. It should close with the claim that
  expected utility remains the baseline, but risky choice needs explanations
  that track more than expected utility over final wealth.
- Chapter navigation: 1a may include one brief navigation sentence saying that
  the next notebook begins with reference points and gains/losses as one way the
  chapter starts moving beyond final-wealth expected utility; later notebooks
  continue the chapter's treatment of expectations and probability-side issues.
- What 1a must not pre-emptively build: 1a must not build reference-dependent
  preferences, exogenous reference points, expectations-based reference points,
  probability weighting, or prospect theory.
