# Model

Use this guide for theory sections, model sections, SDF frameworks, equilibrium restrictions, propositions, prediction derivations, estimator frameworks, simulations, calibrations, and quantitative model discussions.

Workflow: first apply the Cochrane Rules, then follow Core Logic as the writing order, then choose the closest Framework for the model-section type. Use the selected skeleton as structure only, not as wording to copy. Use only facts supplied by the user. Omit any move that cannot be supported by user-supplied facts.

## Cochrane Rules

- Use theory only to the extent needed to understand the paper's main result.
- If the paper's main contribution is empirical, keep the model to the minimum structure required for the empirical work.
- Do not present a general model and then specialize it for the data.
- Work out the specialized model that is actually taken to the data.
- Explain the economic object before introducing notation or symbols.
- After a formal result, state the intuition and the testable or estimable implication.
- State the structure directly; reserve assumption language for restrictions that matter for identification, tractability, or interpretation.

## Core Logic

Use this as an ordering priority, not a checklist. Start with the object and the specialized model actually used, then follow the selected framework's math or empirical architecture. Omit moves that do not apply.

1. Pricing, prediction, or decision object.
2. Economy, agents, assets, timing, and information.
3. Key friction, belief, constraint, state variable, or econometric problem.
4. Assumptions and their roles.
5. Equilibrium, estimator, SDF, or pricing relation.
6. Proposition, theorem, comparative static, or testable restriction.
7. Economic intuition.
8. Empirical mapping, calibration, simulation, or implementation.
9. Scope, simplification, or limit only when supplied and material for interpreting the result.

## Frameworks

Use skeletons as structure, not as wording to copy mechanically. Skeletons control order and coverage, not phrasing. Choose the closest framework, follow its move sequence, and replace the structure with the user's supplied facts.

### 1. Full Equilibrium Model

Use for structural asset-pricing models, intermediary models, incomplete-market models, and general equilibrium papers.

Move sequence: research object -> economy/timing -> agents/preferences/assets/frictions -> shocks/state variables -> optimization -> market clearing -> equilibrium definition -> pricing relation -> channels -> empirical restrictions.

Skeleton:

```text
This section develops a [model/framework] to link [primitive/friction] to [pricing object].
We consider an economy populated by [agents] who trade [assets] over [horizon/timing].
The key state variables are [state variables], which summarize [economic force].
Agents choose [controls] to maximize [objective] subject to [constraints].
A competitive equilibrium consists of [prices, allocations, policies] such that [optimization] and [market clearing] hold.
The resulting pricing relation shows that [pricing object] depends on [state/exposure/channel].
```

### 2. Parsimonious Mechanism Model

Use when the model disciplines an empirical relation rather than providing a complete equilibrium environment.

Move sequence: relation to explain -> minimal primitives -> choice or payoff function -> first-order condition or decision rule -> observable mapping -> regression implication -> optional scope condition.

Skeleton:

```text
The model is deliberately parsimonious: it isolates [core mechanism].
[Agent] chooses [action] given [state/friction], which affects [price/return/demand].
The friction enters through [cost/constraint/belief distortion], which affects [margin of choice].
Substituting the decision rule into [pricing object] yields [testable implication].
The sign of [coefficient] is predicted to be [positive/negative] because [economic force].
```

### 3. Beliefs, Attention, Or Learning Model

Use for underreaction, overreaction, sentiment, disagreement, attention, salience, Bayesian learning, and belief distortions.

Move sequence: puzzle -> information or signal environment -> belief, attention, or disagreement friction -> updating or decision rule -> price, demand, or return implication -> proposition or simulation.

Skeleton:

```text
[Puzzle] arises because investors observe [signal/information set] but process it through [belief/attention/disagreement friction].
Beliefs or attention evolve with [state variable or signal], which changes [demand/discount rate/expected payoff].
The pricing rule implies that [return/pricing object] varies with [belief state].
The proposition gives the conditions under which [overreaction/underreaction/premium] appears.
```

### 4. SDF, Factor-Pricing, Or Spanning Framework

Use for risk premia, alphas, candidate SDFs, factor comparisons, spanning, redundancy, admissible SDFs, and moment restrictions.

Move sequence: Euler/no-arbitrage condition -> candidate SDF or factor model -> pricing object -> normalization/spanning -> alpha/risk-price/redundancy condition -> statistic/moment -> empirical implementation.

Skeleton:

```text
We start from the Euler equation for [payoff/test assets].
The candidate SDF is spanned by [factors], with normalization [normalization].
Under [spanning/regularity condition], the model prices [test assets] if [moment restriction] holds.
Failure of the restriction appears as [alpha/pricing error/test statistic].
We evaluate this implication using [moments/test assets/estimator].
```

### 5. Estimator Or Identification Framework

Use for IPCA, three-pass estimators, Bayesian SDFs, set identification, latent factors, weak factors, generated regressors, and high-dimensional estimators.

Move sequence: identification problem -> observables/unobservables -> DGP and assumptions -> estimator steps -> target interpretation -> theorem/asymptotics -> finite-sample diagnostics -> empirical use.

Skeleton:

```text
The target object is [risk premium/alpha/SDF/pricing error/expected return].
It is hard to estimate because [latent factor/high-dimensional/omitted-variable/selection problem].
Assumption [X] ensures that [latent object] can be recovered from [observables].
Given [observables], the estimator proceeds in [number] steps.
Step [k] estimates [object]; step [k+1] maps it into [risk premium/SDF/pricing error].
The theorem characterizes the sampling behavior of [estimator] as [sample dimensions] grow.
```

### 6. Calibration, Simulation, Or Quantitative Model

Use for dynamic programming, calibrated equilibrium, SMM, Monte Carlo validation, counterfactuals, and mechanism decomposition.

Move sequence: model mechanism -> states/controls -> Bellman/SDF/FOC -> numerical solution -> parameter discipline -> targeted moments -> untargeted implications or validation -> sensitivity or counterfactual only if supplied -> pricing implication.

Skeleton:

```text
The calibration asks whether [mechanism] can generate [asset-pricing moment].
For calibration, parameters are divided into [externally set] and [targeted] groups.
We choose [parameter] to match [moment] because it primarily governs [model margin].
Model-implied moments are computed from simulated data after [burn-in/sample treatment].
The nontargeted moments validate [mechanism/model implication].
[Optional] The counterfactual shuts down [channel] while holding [other primitives] fixed.
```
