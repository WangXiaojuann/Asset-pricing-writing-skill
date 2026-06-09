# Sentence Functions

Use this file for sentence-level polishing in empirical asset-pricing prose. These functions help diagnose what a sentence should accomplish; they are not templates to apply by default.

Workflow: first identify the sentence's job, then use the closest function to diagnose whether the sentence states that job clearly, precisely, and with the right claim strength. Preserve the user's sentence structure when it is already clear and source-backed. Use the source-style patterns only as fallback shapes for weak, vague, translated, overlong, or poorly ordered sentences; do not copy them mechanically or reuse the same phrasing across different passages. Omit any pattern that cannot be supported by user-supplied facts.

## 1. State The Research Object

Use when: the sentence needs to name the question, pricing object, model object, or empirical object.

Core move: object -> action -> setting or criterion.

Source-style patterns:

- This paper studies [pricing object] in [setting].
- We examine whether [economic force] affects [pricing object].
- We analyze [object] using [data/model/design].
- We ask whether [benchmark implication] holds for [asset/test assets/setting].
- The analysis focuses on [object], rather than [nearby object].
- The question is whether [channel/model/data] explains [pattern].
- To isolate [economic object], we consider [setting/model/sample].

Avoid:

- Do not open with a broad field-level claim when the research object is available.
- Do not state a question that the supplied facts do not answer.

## 2. State The Paper's Move

Use when: the sentence needs to say what the paper does after the object is clear.

Core move: paper action -> method/data/model -> target object.

Source-style patterns:

- We develop [method/model/framework] to estimate [target object].
- We construct [measure/portfolio/test assets] to capture [economic margin].
- We use [data/source/variation] to identify [effect/channel].
- We compare [model/specification] with [benchmark].
- We revisit [claim/test/practice] using [correction/criterion].
- We extend [standard approach] by allowing for [complication].
- We map [model variable] to [empirical counterpart].

Avoid:

- Do not write that the paper "fills a gap" unless the gap is stated concretely.
- Do not describe procedures before naming what they are meant to recover.

## 3. State The Main Finding

Use when: the sentence should report the main empirical or theoretical result directly.

Core move: result -> object -> direction or conclusion.

Source-style patterns:

- We find that [main variable] predicts [outcome].
- We show that [model/method] [prices/explains/predicts] [object].
- We document [pattern] in [sample/setting].
- The evidence shows that [effect] is [direction/magnitude].
- The results suggest that [interpretation].
- The main result is that [object] changes when [condition] is accounted for.
- The evidence points to [answer] rather than [alternative].
- We find no/little evidence of [effect/channel].

Avoid:

- Do not write "we examine whether" when the result is already supplied.
- Do not strengthen "suggests" into "proves" or "establishes" unless the design supports it.

## 4. Report Table Or Figure Evidence

Use when: the sentence introduces or interprets a table, panel, column, figure, or diagnostic plot.

Core move: table/figure -> object reported -> main pattern.

Source-style patterns:

- Table [X] reports [statistic/result] for [sample/test assets].
- Panel [A] shows [estimate/pattern] for [group/specification].
- Column [X] reports/presents [regression/test] with [controls/specification].
- Figure [X] plots [object] against [comparison/time/state].
- The first row reports [metric] for [baseline model].
- The last column adds [control/factor/fixed effect].
- The table shows that [estimate/pattern] is [direction/magnitude].
- The figure shows that [pattern] is concentrated in [period/group/state].

Avoid:

- Do not say "Table X shows" without stating what the reader should see.
- Do not describe every column when only one estimate matters for the claim.

## 5. Report Magnitude And Precision

Use when: the sentence needs economic magnitude, statistical precision, frequency, or units.

Core move: estimate -> unit/frequency -> precision -> economic scale.

Source-style patterns:

- The spread is [estimate] per [frequency], with a t-statistic of [t].
- The coefficient on [variable] is [estimate], implying/indicating that [economic change] changes [outcome] by [magnitude].
- The alpha is [estimate] per [frequency] and is [statistically/economically] [large/small].
- The estimate is [direction] and [statistically significant/indistinguishable from zero].
- A [unit/interquartile/one-standard-deviation] increase in [variable] is associated with [effect size].
- The [alpha/pricing error] falls/drops to [estimate] after [benchmark/control] is added.
- The improvement is economically meaningful because [metric/comparison].

Avoid:

- Do not report a t-statistic or standard error unless supplied by the user.
- Do not call an estimate economically large without a scale or comparison.

## 6. Compare With A Benchmark

Use when: the sentence needs a null, benchmark model, comparison group, or alternative method.

Core move: object -> benchmark -> contrast -> implication.

Source-style patterns:

- Relative to [benchmark], [model/specification] delivers [improvement/failure].
- Compared with [comparison group], [treated/high-exposure group] has [pattern].
- The result is stronger for [group] than for [group].
- The estimate remains [direction/significance] after [control/fixed effect] is added.
- Adding [factor/control] reduces [alpha/spread/pricing error] when [supplied comparison] is used.
- [Model A] prices [test assets] better than [model B] under [criterion].
- [Model/benchmark] fails to explain [pattern].

Avoid:

- Do not imply that a benchmark fails unless the supplied evidence shows failure.
- Do not compare with a model, factor, or sample that the user did not mention.

## 7. Interpret A Coefficient Or Pricing Error

Use when: the sentence needs to translate a number into an economic interpretation.

Core move: estimate -> comparison -> economic meaning.

Source-style patterns:

- The coefficient on [variable] is [estimate].
- The coefficient estimate implies [economic magnitude].
- The loading of [portfolio/asset] on [factor] is [direction/magnitude].
- The pricing error is defined as [definition].
- The pricing error is [direction/magnitude], indicating that [model/specification] [prices/fails to price] [test assets].
- The estimate is [direction/significance], indicating that [interpretation].
- The intercept remains [direction/significance] after [benchmark/factor] is added.

Avoid:

- Do not interpret a coefficient without specifying the dependent variable or economic scale.
- Do not equate correlation with a mechanism unless the design supports the mechanism.

## 8. Explain A Mechanism Or Channel

Use when: the sentence connects evidence to an economic mechanism, model channel, or interpretation.

Core move: mechanism -> predicted pattern -> observed pattern.

Source-style patterns:

- The model/theory predicts that [effect] should be stronger when [condition].
- This pattern is consistent with [channel].
- The evidence points to [mechanism] as a source of [pricing object].
- The result is driven by [component/channel], not by [alternative] when supplied.
- The channel operates through [margin], which affects [price/return/demand].
- The model explains [pattern] through [state variable/friction].
- The evidence supports [interpretation] without requiring [stronger claim].

Avoid:

- Do not introduce a mechanism that the user did not supply.
- Do not write "consistent with" as if it proves the mechanism.

## 9. Report Robustness Or Alternative Tests

Use when: the sentence summarizes a robustness check, alternative construction, placebo, or specification change.

Core move: concern -> alternative design -> result change -> inference.

Source-style patterns:

- The result is robust to [alternative measure/specification/sample].
- The estimate remains [direction/magnitude] after controlling for [control].
- The result remains similar/unchanged when [sample/design] is modified.
- The result remains [direction/significance] with [fixed effects/benchmark/alternative weighting].
- The placebo test finds little evidence of [effect].
- The alternative specification produces [similar/weaker/stronger] estimates.
- As a placebo test, we examine [placebo object].

Avoid:

- Do not list many checks one by one when they do not change the inference.
- Do not claim robustness unless the user supplied the check and its result.

## 10. State Null, Weak, Or Mixed Evidence

Use when: the supplied result is null, weak, statistically imprecise, mixed, or limited.

Core move: absent or mixed effect -> precision or scope -> interpretation.

Source-style patterns:

- We find little evidence that [effect] is driven by [channel].
- The estimate is statistically indistinguishable from zero.
- The test does not reject [null/model] for [setting].
- We find mixed evidence across [samples/specifications].
- The result weakens when [condition] is imposed.
- [Model/specification] fails to explain [test assets/pattern].
- The evidence does not support [stronger claim].

Avoid:

- Do not hide a null result behind vague language.
- Do not turn mixed evidence into a clean positive result.
- Do not call a null result informative unless the user supplies the precision, design, or comparison that makes it informative.

## 11. Transition To The Next Test

Use when: the sentence needs to move the reader from one empirical or theoretical step to the next.

Core move: completed result -> reason for next step -> next object.

Source-style patterns:

- We next examine [object].
- To understand the source of [pattern], we turn to [test/decomposition].
- We now compare [model] with [benchmark].
- We begin by [showing/documenting/estimating] [stylized fact/object].
- We then test whether [mechanism] predicts [heterogeneity].
- To address [concern], we repeat the analysis using [alternative design].
- Having established [result], we examine [next object].

Avoid:

- Do not use roadmap transitions to compensate for poor ordering.
- Do not preview a test that is not supplied by the user.

## 12. Control Claim Strength

Use when: the sentence risks overclaiming, needs hedging, or must distinguish evidence from proof.

Core move: evidence -> warranted interpretation -> excluded overclaim.

Source-style patterns:

- The evidence is consistent with [interpretation].
- The result suggests [interpretation], rather than [stronger claim].
- This evidence should not be interpreted as implying [unsupported conclusion].
- The analysis cannot rule out [alternative], but it shows [supported claim].
- The evidence supports [claim] within [sample/setting].
- This result does not imply [unsupported conclusion].
- The pattern is difficult to reconcile with [alternative] when [alternative] is supplied.

Avoid:

- Do not use hedging to make an unsupported claim sound safe.
- Do not add alternatives or caveats that are not in the user's facts.

## 13. Describe Data Or Measurement Construction

Use when: the sentence needs to define a sample, measure, variable, matching rule, or portfolio construction step.

Core move: data action -> object -> timing/unit -> reason if material.

Source-style patterns:

- We use [data source] to measure [object].
- The sample consists of [units] over [sample period].
- We define [variable] as [construction].
- We construct [portfolio/factor/measure] from [inputs].
- We sort [universe] on [variable] at [formation date].
- We merge [data source A] with [data source B] using [key].
- We exclude [observations] because [measurement/economic reason].
- Higher [measure] indicates/corresponds to greater [economic object].

Avoid:

- Do not turn data construction into a cleaning log.
- Do not explain a filter unless it affects measurement, identification, or reproducibility.

## 14. State Model Implications

Use when: the sentence needs to connect a formal model, assumption, proposition, or SDF relation to a testable implication.

Core move: model structure -> restriction/result -> empirical implication.

Source-style patterns:

- The model implies that [pricing object] depends on [state/exposure/channel].
- Under [condition], [restriction] holds.
- Proposition [X] shows that [result].
- The Euler equation [number] implies [moment restriction].
- The SDF prices [test assets] if [condition] holds.
- The comparative static predicts that [effect] increases with [state variable].
- The testable implication is that [outcome] should vary with [observable].
- The simulation examines/assesses whether [mechanism] can generate [moment].

Avoid:

- Do not introduce unnecessary notation before the economic object is clear.
- Do not present a general model if the paper uses only the specialized case.
