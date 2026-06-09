# Abstract

Use this guide for abstracts, short paper summaries, contribution summaries, and compact paper pitches.

Workflow: first apply the Cochrane Rules, then follow Core Logic as the writing order, then choose the closest Framework for the abstract type. Use the selected skeleton as structure only, not as wording to copy. Use only facts supplied by the user. Omit any move that cannot be supported by user-supplied facts.

## Cochrane Rules

- Keep the abstract within the journal convention: roughly 100-150 words unless the user gives a different constraint.
- Use the abstract to communicate one central contribution.
- Do not mention other literature in the abstract unless the user's facts require a benchmark or reassessment claim.
- Make the abstract concrete: say what the paper finds, not what it looks for.
- Do not write process descriptions such as `data are analyzed`, `theorems are proved`, or `discussion is made` without stating the result.
- Write the abstract as one compact paragraph unless the user asks for another format.

## Core Logic

Write the abstract in this order unless the user's draft clearly requires another:

1. Research object, puzzle, method, or data move.
2. Main obstacle or benchmark.
3. Paper's method, model, data, or design.
4. Main result, stated with metric and direction when supplied.
5. Economic interpretation, model implication, or revision of prior inference.

Good abstract verbs are concrete: `propose`, `develop`, `show`, `find`, `document`, `estimate`, `test`, `compare`, `identify`, `reassess`.

## Frameworks

Use skeletons as structure, not as wording to copy mechanically. Skeletons control order and coverage, not phrasing. Choose the closest framework, follow its move sequence, and replace the structure with the user's supplied facts.

### 1. Method Or Framework Abstract

Use for new estimators, pricing tests, factor construction, machine-learning frameworks, SDF methods, or model-comparison protocols.

Move sequence: tool/framework -> target problem -> distinctive operation -> property -> application -> implication.

Skeleton:

```text
We propose [method/framework/model] for [asset-pricing task] in [setting].
The approach [core operation], allowing [capability] while addressing [constraint].
Under [economic/statistical framework], [method] delivers [object/result] that [property].
Applied to [data/test assets/portfolios], it [comparison result] relative to [benchmark].
The results imply that [economic interpretation or use case].
```

### 2. Puzzle Or Mechanism Abstract

Use for anomalies, return predictability, risk-premium puzzles, factor failures, belief or attention mechanisms, household or intermediary channels, and mispricing versus risk debates.

Move sequence: puzzle -> proposed channel -> test design -> main relation -> where it is strongest -> bounded mechanism interpretation.

Skeleton:

```text
[Phenomenon] is difficult to reconcile with [benchmark model/view].
We study whether [mechanism/channel] explains [phenomenon].
Using [variation/data/design], we find that [main relation].
The effect is stronger when [mechanism condition] and weaker when [opposing condition].
These patterns are consistent with [mechanism] rather than [alternative explanation].
```

### 3. Reassessment Or Critique Abstract

Use when the paper revisits accepted evidence, changes inference after a correction, shows low power, accounts for transaction costs or constraints, or revises a model-ranking conclusion.

Move sequence: accepted practice/claim -> flaw or missing condition -> correction/test -> changed inference -> qualified implication.

Skeleton:

```text
The literature commonly [practice/claim] when evaluating [asset-pricing object].
We show that this approach can be misleading because [specific reason].
After [correction/test/design change], [previous finding] [weakens/disappears/changes].
The revised evidence indicates that [more limited conclusion].
Thus, [broader claim/use] should be interpreted as [qualified interpretation].
```

### 4. Theory Or Quantitative Model Abstract

Use for equilibrium models, incomplete-market models, intermediary constraints, preference or belief models, calibrated models, and counterfactual quantitative exercises.

Move sequence: model environment -> key ingredient -> pricing prediction -> calibration/estimation/evidence -> implication and scope.

Skeleton:

```text
We develop [model type] in which [risk/friction/belief/agent] affects [asset-pricing object].
The model links [state variable/choice/friction] to [expected returns/prices/allocations] through [channel].
It predicts that [return/pricing/portfolio implication] varies with [state or cross-sectional attribute].
Calibrated or estimated using [moments/data], the model matches [target facts] and [untargeted result if supplied].
The mechanism has implications for [risk premia/portfolio choice/capital allocation/welfare].
```

### 5. New Data Or Measurement Abstract

Use for new datasets, new measures, new facts, newly observable frictions, institutional data, survey data, holdings data, or administrative data.

Move sequence: data/measure -> central fact -> asset-pricing link -> validation/mechanism -> what the measure reveals.

Skeleton:

```text
Using [new data/measure], we document [previously unmeasured fact].
[Measure] is associated with or predicts [asset-pricing outcome] in [setting].
The relation is concentrated among [subsample/condition] and survives [controls/benchmarks].
Additional tests indicate that [mechanism] accounts for the pattern.
The findings reveal [economic object] that is difficult to observe using [standard data/measure].
```
