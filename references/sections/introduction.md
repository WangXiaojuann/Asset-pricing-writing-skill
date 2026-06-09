# Introduction

Use this guide for introductions, motivation, contribution framing, result previews, and introduction-level literature positioning.

Workflow: first apply the Cochrane Rules, then follow Core Logic as the writing order, then choose the closest Framework for the introduction type. Use the selected skeleton as structure only, not as wording to copy. Use only facts supplied by the user. Omit any move that cannot be supported by user-supplied facts.

## Cochrane Rules

- Start with what the paper does and what its major contribution is.
- Do not merely state the conclusion; give the fact, estimate, comparison, or model implication behind it.
- Do not open with philosophy, generic literature interest, broad policy importance, or other throat-clearing.
- Explain the paper's contribution before positioning it against the literature.
- Keep the literature review brief and focused on the two or three closest papers.
- Give proper credit without arguing that prior work is wrong.
- Keep the introduction tight; roadmap paragraphs are optional and should not replace the contribution.
- Do not force a limitation, boundary, or future-research ending in an introduction.

## Core Logic

Use this as an ordering priority, not a checklist. For a full introduction, include the moves needed to make the question, contribution, results, and positioning clear.

1. Specific asset-pricing question, puzzle, decision, or benchmark restriction.
2. What the benchmark, standard approach, or closest literature explains, and what question, margin, comparison, or object remains open.
3. The paper's move: data, model, design, estimator, or reassessment.
4. Result preview in the same order as the paper's evidence.
5. Contribution positioning by object, mechanism, data, method, or criterion.
6. Optional close: contribution-to-literature, clean implication, short roadmap, or scope condition only when supplied and useful.

## Frameworks

Use skeletons as structure, not as wording to copy mechanically. Skeletons control order and coverage, not phrasing. Choose the closest framework, follow its move sequence, and replace the structure with the user's supplied facts.

### 1. Puzzle To Mechanism

Use when the paper explains an anomaly, return pattern, price reaction, predictability result, or state-dependent premium.

Move sequence: empirical puzzle -> standard view struggles -> mechanism intuition -> test design -> results by prediction -> alternatives -> contribution.

Skeleton:

```text
[Empirical fact] is puzzling because [benchmark model/view] would suggest [opposite or weaker pattern].
Existing explanations emphasize [view A] or [view B], but they leave open [missing force].
We study [mechanism] using [data/model/design], which links [observable object] to [theoretical primitive].
The mechanism predicts that [pricing object] should be stronger among [group/state] and weaker among [comparison group/state].
The evidence follows this pattern: [result cluster 1], [result cluster 2], and [result cluster 3 if supplied].
```

### 2. Canonical Model Challenge

Use for CAPM, ICAPM, SDF, factor models, present-value restrictions, consumption-based models, or benchmark pricing restrictions.

Move sequence: model prediction -> empirical tension -> unresolved question -> revised test/model -> benchmark comparison -> interpretation.

Skeleton:

```text
[Canonical model] predicts that [pricing restriction].
However, [empirical evidence/fact family] raises a tension for this restriction.
The difficulty is that standard tests [combine/measure/average over] [component A] and [component B].
This paper evaluates [target object] by [method/design/model comparison].
We show where [benchmark] succeeds, where it fails, and what this implies for [asset-pricing task].
```

### 3. Method Or Measurement

Use for estimators, high-dimensional prediction, omitted-factor problems, model uncertainty, weak factors, latent factors, Bayesian methods, or new measurement protocols.

Move sequence: common practice -> hidden weakness -> target object -> framework -> validation -> application -> changed conclusion.

Skeleton:

```text
A common practice is to evaluate [model/object] using [standard approach].
This can answer a different object when [statistical/economic complication] is present.
We target [estimand/object] and develop [method/measure/framework] to recover it under [condition].
The approach is disciplined by [theory/simulation/identification condition] and applied to [asset-pricing setting].
The application changes [estimate/model ranking/inference] relative to [benchmark approach].
```

### 4. New Data Or Identification

Use when the contribution rests on newly observed behavior, proprietary data, administrative data, institutional variation, a shock, a linkage, or a cleaner comparison.

Move sequence: unobserved margin -> data/variation gap -> new source or linkage -> identification logic -> baseline evidence -> heterogeneity/mechanism -> contribution.

Skeleton:

```text
[Economic margin] is central for [pricing object], but standard data do not observe [required object].
We use [data/source/variation] to measure [object] at the [unit] level.
The design compares [treated/high-exposure units] with [benchmark units] around [variation].
This allows us to test whether [pricing outcome] responds to [economic primitive].
The results show [baseline effect] and are strongest where [mechanism] predicts.
```

### 5. Debate Or Reassessment

Use when the paper reorganizes an established literature, revisits an anomaly, corrects a test, or reconciles conflicting evidence.

Move sequence: contested evidence -> why existing tests are incomplete -> comprehensive correction or new criterion -> changed evidence -> revised interpretation.

Skeleton:

```text
The evidence on [topic] has led to conflicting interpretations of [pricing object].
Existing tests leave [distinction] unresolved, making it difficult to distinguish [explanation A] from [explanation B].
We reassess this evidence using [correction/data/criterion].
The reassessment shows that [result survives/disappears/changes] once [condition] is considered.
This changes the interpretation of [pricing object] by showing [qualified result].
```

### 6. Decision Or Portfolio Implication

Use for portfolio choice, asset management, model uncertainty, Bayesian learning, implementable strategies, and decision-relevant pricing.

Move sequence: decision problem -> uncertainty/constraint -> framework -> economic metric -> quantitative implication -> when it matters.

Skeleton:

```text
[Decision maker] must choose [portfolio/action] using estimates of [unknown object].
Standard approaches often abstract from [uncertainty/friction], which can change [economic metric].
We develop [framework] that incorporates [uncertainty/friction] into [decision/pricing object].
The framework is evaluated by [economic metric], not only by [statistical metric].
The results show when [decision/model choice] changes and when it does not.
```
