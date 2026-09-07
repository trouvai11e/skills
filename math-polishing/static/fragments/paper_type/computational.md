# Paper type: Computational / applied

Typical architecture:

`Problem or governing equations -> Numerical (or experimental) method -> Theoretical analysis -> Numerical results -> Conclusions`

## Problem section

- Introduce the governing equations (differential, integral, operator equations, or the optimization problem) and the notation; explain the physical meaning of unknown functions and parameters where the audience needs it.
- Do model simplifications here, with reasons, rather than scattering them through the method section.

## Method section

- The numerical scheme is the heart of the paper. Content is concrete, so the writing task is ordering and completeness, not decoration. Define every discretization parameter.

## Numerical results section

This section looks easy (figures, tables, data) but is where drafts most often fail. Requirements:

1. **Reproducibility.** Describe the experiments in enough detail — parameter values, stopping criteria, machine/software where relevant — that a reader can reproduce the results.
2. **Benchmark choice.** Prefer recognized benchmark problems of real difficulty over trivial one-dimensional examples. The best examples show the new algorithm clearly outperforming existing ones. Examples with known exact solutions are ideal when available.
3. **Comparison.** Compare with previous or alternative methods, state the differences, and explain the reasons where possible.
4. **Commentary is mandatory.** Never list data without interpretation: discuss the method's strengths, comparison with others, meaningful observations, and agreement with theoretical predictions. A figure or table with no discussion should not be in the paper.
5. **Economy.** Keep only representative figures and tables; merge related ones. Twenty figures is a red flag — cut toward half. One or two displays per phenomenon suffice; narrate the rest.

Reporting language for figures/tables ("Figure 2 shows ...", "in good agreement with ...") is in `references/math-phrasebook.md`.

## What numerics can claim

Numerical experiments may: deepen understanding of the method, confirm theoretical predictions, calibrate user-defined parameters, or reveal behavior better than theory predicted (a prompt for follow-up theory). The conclusion section should say which of these the paper's experiments actually did.
