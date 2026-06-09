# Data

Use this guide for data sections, sample construction, variable definitions, measurement, summary statistics, institutional data, data linkages, high-dimensional predictor construction, model-data mapping, and portfolio-formation setup.

Workflow: first apply the Cochrane Rules, then follow Core Logic as the writing order, then choose the closest Framework for the data-section type. Use the selected skeleton as structure only, not as wording to copy. Use only facts supplied by the user. Omit any move that cannot be supported by user-supplied facts.

## Cochrane Rules

- Include only data details needed to understand the main empirical result.
- Do not turn the data section into a warm-up exercise, cleaning log, or long description of well-known datasets.
- Describe the data action first, then explain why it matters and compare it with alternatives only after the action is clear.
- Explain material filters, timing choices, and transformations by their measurement, economic, or identification role.
- Document data construction well enough that central numbers can be reproduced from the paper and its appendices.
- Move secondary data checks, alternative constructions, and extensive variations to an appendix when they do not change the main inference.

## Core Logic

Use this as an ordering priority, not a checklist. Include only moves needed to make the sample, variables, timing, and main empirical design reproducible.

1. Economic object and why the data are needed.
2. Primary data source, then market returns, accounting controls, and factor/benchmark data.
3. Universe, sample period, inclusion criteria, exclusion criteria, and final unit.
4. Main variable or measure, before secondary controls.
5. Timing: information date, formation date, return horizon, and rebalancing frequency.
6. Portfolio, factor, or estimation setup if it belongs in the data section.
7. Summary statistics and why the variation matters.
8. Coverage, selection, or measurement limits only when they materially affect interpretation.

## Frameworks

Use skeletons as structure, not as wording to copy mechanically. Skeletons control order and coverage, not phrasing. Choose the closest framework, follow its move sequence, and replace the structure with the user's supplied facts.

### 1. Standard Asset, Factor, Or Portfolio Construction

Use for equity, bond, option, fund, or portfolio samples and factor or strategy construction.

Move sequence: test object -> database/universe -> filters -> availability and lags -> sort/breakpoints/weights/rebalancing -> long-short or factor definition -> summary statistics.

Skeleton:

```text
This section describes [data sources], the construction of [main variables], and the [portfolio/estimation] procedure used in the empirical analysis.
The baseline sample consists of [units] that satisfy [inclusion criteria] over [sample period].
We exclude [observations] because [economic or measurement reason].
At [formation date], we sort [universe] into [number] portfolios based on [sorting variable] using [breakpoint rule].
The [factor/strategy] return is the return on [long leg] minus the return on [short leg].
Portfolios are [value/equal]-weighted and rebalanced [frequency].
```

### 2. Latent Economic Object To Proxy

Use for expected returns, mispricing, beliefs, attention, liquidity, uncertainty, constraints, quality, profitability, demand, exposures, or other latent objects.

Move sequence: latent object -> proxy rationale -> formula and units -> timing and sign -> measurement error only if material -> validation or alternative proxy.

Skeleton:

```text
Because [latent object] is not directly observable, we proxy for it using [observable measure], which captures [economic margin].
We define [variable] as [function of inputs], where [input A] denotes [definition] and [input B] denotes [definition].
Higher values of [variable] correspond to greater [economic object].
If measurement error is material, state its likely direction only when the user supplies a defensible reason.
We validate the measure using [summary statistic/benchmark/alternative proxy].
```

### 3. Proprietary, Administrative, Or Micro Data

Use for household, fund, intermediary, trading, holdings, survey, administrative, proprietary, and institutional data.

Move sequence: source credibility and coverage -> unit -> raw record to research variable -> merge with market/accounting data -> sample restrictions -> descriptive variation -> optional data limits.

Skeleton:

```text
We obtain [data type] from [source], which records [raw object/observed margin] at the [unit/frequency] level.
We merge these records with [market/accounting/returns data] using [matching key] at the [unit]-[time] level.
The final sample contains [N] [unit]-[time] observations for [N units] unique [units].
[Optional] The coverage limitation is [limitation], which affects interpretation by [scope condition].
```

### 4. Multi-Source Matching, Network, Or Linkage

Use for supply-chain links, fund holdings, peer links, network exposure, investor-firm matching, analyst-firm matching, and other relational data.

Move sequence: relationship object -> sources -> eligible pairs/links -> intensity or exposure -> aggregation -> sample effect if material -> alternative link or placebo if supplied.

Skeleton:

```text
We define [relationship object] using [source A] and [source B].
Eligible links require [link criterion] and are measured at [frequency].
For each [unit], we compute [link intensity/exposure] as [aggregation rule].
We aggregate [pair-level/link-level object] to the [firm/fund/portfolio] level using [weights].
[Optional] The match changes the sample from [initial sample] to [matched sample], mainly because [coverage reason].
```

### 5. Machine Learning, High-Dimensional Predictors, Or Forecast Sample

Use for many predictors, factor zoo, return prediction, model selection, train/test splits, and forecasting portfolios.

Move sequence: target -> predictor universe -> information timing -> preprocessing -> missing handling -> estimation and evaluation protocol -> out-of-sample forecast -> portfolio setup.

Skeleton:

```text
The forecast target is [outcome] over [horizon].
Each predictor enters the model only when it is observable by [information date].
We standardize [predictors] within each [time period] so that [comparison/estimation purpose].
Missing values are handled by [method], and we compare the results with [alternative method].
The estimation and evaluation protocol is [rolling/expanding/training-validation-test/other protocol], so that each forecast is out of sample.
```

### 6. Model Calibration, Moments, Or Measurement Alignment

Use when the data section maps model variables to empirical counterparts, moments, test assets, or calibration targets.

Move sequence: model variable -> empirical counterpart -> timing alignment -> item definitions -> test assets/moments -> restrictions justified by model consistency.

Skeleton:

```text
The empirical counterpart of [model variable] is [data variable].
We align [stock/flow/accounting/market object] by measuring [variable] at [date] and returns over [horizon].
The calibration targets [moments] because they discipline [model margin].
The nontargeted moments are [moments], which are used to evaluate [mechanism/model implication].
```
