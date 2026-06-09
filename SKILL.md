---
name: asset-pricing-writing-polisher
description: Rewrite, polish, diagnose, translate into English, or draft prose for empirical asset-pricing and top-finance-journal papers using paragraph logic from classic and recent JF/JFE/RFS/JPE papers. Use this skill whenever the user works on abstracts, introductions, data sections, model/theory sections, empirical findings, table discussion, portfolio sorts, factor tests, alphas, pricing errors, robustness, mechanisms, heterogeneity, or conclusions, including requests for JF, JFE, or RFS style. Preserve the user's facts, numbers, citations, equations, tables, variable names, and claim strength; do not invent empirical content.
---

# Asset Pricing Writing Polisher

Use this skill for polishing, rewriting, translating, diagnosing, or drafting empirical asset-pricing prose. Preserve the user's facts, notation, citations, tables, equations, numbers, and claim strength.

## Core Workflow

1. Always read `references/general-rules.md` first.
2. Treat the user's text as the only source of facts.
3. For simple sentence or paragraph polishing, keep the user's structure and do not load `references/sections/`.
4. For section-level drafting, strong rewriting, or explicit abstract/introduction/data/model/empirical/conclusion work, load the closest guide from `references/sections/`.
5. If a section guide is used, follow its move sequence but treat skeletons as structure only, not wording to copy.
6. Polish in layers: paragraph logic first, sentence structure second, lexical choice third.
7. Use `references/sentence-functions.md` only when sentence structure is weak, vague, translated, overlong, or poorly ordered.
8. Use `references/lexical-choices.md` only as a wording and collocation reference.
9. Run `references/de-ai-rules.md` as the final de-AI audit.

## Section Routing

Load these files only when section-level guidance is needed:

- `abstract.md`: abstract, contribution summary, or paper pitch.
- `introduction.md`: introduction, motivation, contribution framing, or literature positioning.
- `data.md`: data, sample construction, variables, measures, or portfolio-formation setup.
- `model.md`: model, theory, SDF framework, propositions, simulations, or calibration.
- `empirical-findings.md`: empirical results, table discussion, alphas, pricing errors, robustness, mechanisms, heterogeneity, or prediction.
- `conclusion.md`: conclusion, implications, limitations, or final remarks.

## Non-Negotiables

- Do not invent results, magnitudes, sample periods, citations, mechanisms, channels, robustness checks, factor models, or interpretations.
- Do not strengthen claim language beyond the supplied design.
- Preserve LaTeX commands, equations, labels, notation, table/figure/equation references, factor names, variable names, and portfolio-leg definitions.
- If a missing design element changes interpretation, flag it rather than guessing.
