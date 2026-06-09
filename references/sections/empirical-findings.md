# Empirical Findings

Use this guide for empirical results, table discussions, portfolio sorts, factor tests, alphas, pricing errors, prediction results, robustness, mechanisms, heterogeneity, null results, and economic-performance paragraphs.

Workflow: first apply the Cochrane Rules, then follow Core Logic as the writing order, then choose the closest Framework for the empirical-finding type. Use the selected skeleton as structure only, not as wording to copy. Use only facts supplied by the user. Omit any move that cannot be supported by user-supplied facts.

## Cochrane Rules

- Start empirical sections with the main result.
- Do not put warm-up exercises, long data descriptions, preliminary estimates, replications, failed specifications, or side discussions before the main result.
- Show the stylized facts that drive the result, not only estimates and p-values.
- Explain identification in economic terms: source of variation, error term, instruments, controls, and reverse-causality concerns when relevant.
- Describe the variation behind each important estimate, especially when fixed effects change the comparison.
- Explain economic magnitude, not only statistical significance.
- Include standard errors or comparable precision measures for important numbers when supplied.
- Put extensive robustness checks and secondary variations in an appendix when they do not change the main inference.
- Use robustness prose sparingly in the main text; summarize clusters of checks unless a check changes inference, addresses a central identification concern, or establishes scope.

## Core Logic

Before writing, identify the exact evidence object:

- raw return, excess return, abnormal return, alpha, pricing error, factor premium, beta, coefficient, t-statistic, p-value, R2, out-of-sample R2, Sharpe ratio, GRS/Wald/J statistic, utility gain, certainty equivalent.

Use this as an ordering priority, not a checklist. For section openings, lead with the main result. For table-specific paragraphs, include purpose and design only if needed to read the estimate.

1. Purpose of the test or table.
2. Design reminder needed to read the result.
3. Central pattern or estimate.
4. Metric, magnitude, precision, and frequency when supplied.
5. Benchmark, null, factor model, or comparison group.
6. Economic interpretation.
7. Transition to the next test, model comparison, or boundary only when it materially affects interpretation.

## Frameworks

Use skeletons as structure, not as wording to copy mechanically. Skeletons control order and coverage, not phrasing. Choose the closest framework, follow its move sequence, and replace the structure with the user's supplied facts.

### 1. Portfolio-Sort Premium

Use for characteristic portfolios, long-short spreads, factor construction, and anomaly sorts.

Move sequence: table purpose -> sorting variable and holding period -> monotonicity/spread -> raw/excess/adjusted object -> benchmark -> economic interpretation or next empirical step.

Skeleton:

```text
Table [X] reports [raw/excess/risk-adjusted] returns for portfolios sorted on [signal] over [holding period].
Returns [increase/decrease] from [portfolio group] to [portfolio group], and the [high-minus-low] spread is [estimate] per [frequency], with a t-statistic of [t].
The spread remains [direction/significance] after [adjustment/control], suggesting that [signal] is not simply capturing [benchmark characteristic].
[Optional] The effect is concentrated in [subsample/side of the sort], which points to [interpretation] rather than a broad unconditional premium.
```

### 2. Regression Slope Or Fama-MacBeth Finding

Use for panel regressions, Fama-MacBeth tests, event regressions, predictive regressions, and coefficient interpretation.

Move sequence: regression purpose -> outcome/key regressor/controls -> sign and magnitude -> precision -> comparison to baseline -> economic scale -> interpretation or next empirical step.

Skeleton:

```text
Table [X] presents [Fama-MacBeth/panel/time-series] regressions of [dependent variable] on [key variable] and [controls].
The coefficient on [key variable] is [estimate] with a t-statistic of [t], indicating a [positive/negative] relation between [variable] and [outcome].
The estimate changes little after adding [controls/fixed effects], which reduces the concern that the result is driven by [alternative channel].
Interpreted economically, a [unit/interquartile/one-standard-deviation] increase in [variable] is associated with [effect size] in [outcome].
```

### 3. Alpha Or Benchmark Absorption

Use for time-series factor regressions, anomaly absorption, strategy evaluation, and benchmark factor comparisons.

Move sequence: factor model -> alpha/intercept -> benchmark comparisons -> attenuation or persistence -> factor loadings if supplied -> subsumption claim.

Skeleton:

```text
Table [X] reports time-series regressions of [portfolio/strategy] returns on [benchmark factors].
The [model]-alpha is [estimate] per [frequency] with a t-statistic of [t].
Adding [factor set] reduces the alpha from [estimate] to [estimate], indicating that [benchmark risk] absorbs part of the return spread.
The alpha remains [positive/negative/significant] across [benchmarks], suggesting that [strategy/signal] captures a component not spanned by [factor models].
```

### 4. Cross-Sectional Pricing Or Model Fit

Use for test-asset pricing, SDF tests, GMM, pricing errors, model comparisons, spanning, subsumption, and factor horse races.

Move sequence: test assets and model -> metric -> benchmark ranking -> rejection or relative fit -> source of fit or failure -> economic interpretation.

Skeleton:

```text
Table [X] compares [model] with [benchmark models] in pricing [test assets].
The model delivers [pricing-error metric] of [estimate], compared with [benchmark estimate] for [benchmark model].
Although the joint test [rejects/does not reject] the model, the relative fit improves along [metric], especially for [test-asset set].
This evidence supports [relative performance claim] because [source of fit or failure].
```

### 5. Prediction, Out-Of-Sample, Or Economic Performance

Use for forecasting, machine learning, portfolio choice, managed portfolios, certainty equivalents, and implementable strategies.

Move sequence: in-sample versus out-of-sample -> prediction metric -> portfolio/utility translation -> benchmark -> estimation risk or constraints -> feasible implication.

Skeleton:

```text
Table [X] reports out-of-sample [R2/RMSE/forecast error] for [models] relative to [benchmark forecast].
[Model class] produces [positive/lower] out-of-sample performance for [assets], whereas [benchmark] performs [worse/comparably].
Small changes in predictive accuracy translate into [portfolio/utility/Sharpe] gains of [estimate] under [portfolio rule].
The in-sample performance overstates attainable performance because [parameters/weights] must be estimated before the out-of-sample period.
```

### 6. Heterogeneity, State Dependence, Or Decomposition

Use for state dependence, interaction tests, split samples, leg-level decompositions, subgroup results, external-validity checks, and diagnostic comparisons.

Move sequence: heterogeneity question -> relevant group, state, or component -> estimate or pattern -> economic scale -> diagnostic interpretation -> next test if needed.

Skeleton:

```text
Table [X] examines whether [result] varies across [groups/states/components].
The estimate is [larger/smaller] in [subsample/state/component], with a difference of [estimate] and a t-statistic of [t].
This pattern shows that [economic object] is concentrated in [where the variation appears].
The decomposition helps distinguish [interpretation A] from [interpretation B] when those interpretations are supplied.
```

### 7. Mechanism Or Channel Test

Use when the user supplies a mechanism prediction, a channel variable, and a relevant alternative explanation.

Move sequence: mechanism prediction -> stronger/weaker group or channel variable -> test -> result -> channel interpretation -> alternative only if supplied.

Skeleton:

```text
If [mechanism] explains the main result, the effect should be stronger among [group] and weaker among [group].
Table [X] shows that the estimate is [larger/smaller] in [subsample], consistent with [mechanism].
The interaction between [signal] and [mechanism variable] is [estimate] with a t-statistic of [t].
When [alternative explanation] is supplied, these patterns are harder to reconcile with [alternative explanation].
```

### 8. Robustness, Boundary, Or Null Result

Use for alternative measures, samples, specifications, placebo tests, falsification tests, mixed results, and scope conditions.

Move sequence: concern -> alternative design -> result change -> scope or null interpretation -> connection to main claim.

Skeleton:

```text
To address the concern that [issue], Table [X] repeats the analysis using [alternative design].
The estimate remains [direction] and [similar/lower/higher] in magnitude, indicating that the main result is not driven by [concern].
The effect weakens when [condition], suggesting that [boundary condition] limits the interpretation.
We find little evidence of [effect] in [placebo/sample], which helps distinguish [main channel] from [alternative channel].
```

### 9. Stylized Fact, Figure, Or Diagnostic Pattern

Use for figures, descriptive patterns, characteristic importance, model diagnostics, decompositions, and other evidence that is not primarily a coefficient table.

Move sequence: figure or diagnostic purpose -> visible pattern -> economic scale -> relation to main result -> implication or next test.

Skeleton:

```text
Figure [X] plots [object] against [comparison/state/time].
The central pattern is [pattern], with [economic scale] between [group/period] and [group/period].
This pattern matters because it shows [variation or fact] behind [main result].
It motivates [next test/model comparison/interpretation].
```
