# Section: Abstract

The abstract is a self-contained minipaper: one paragraph, typically 100–300 words. It is published, indexed, and translated separately from the paper, so it must stand alone.

## It answers four questions

1. What is the problem / what does the paper do?
2. How is it solved — what method?
3. What is the main result? Solved fully or partially?
4. Why does it matter — to science or to the reader?

## Hard rules

- **No display formulas, and avoid math symbols entirely** where narration can carry the meaning. "We prove that the viscous solution converges to the inviscid one with rate 1/2 in the $L^1$-norm, improving to rate 1 when the flux is strictly convex and the entropy solution is piecewise smooth" — not two lines of PDE.
- **No bare citation numbers.** An abstract detached from its reference list makes "[10]" meaningless. If a citation is truly needed (the paper extends a specific result), give full bibliographic information minus the title: "Saranen [Math. Comp., 48 (1987), pp. 485–502] proved ...; we extend his results to open curves." Citing one's own prior method: "proposed by the author(s) in [full citation]".
- **Do not open with "In this paper" / "This paper".** Some journals ban it. Start with the content: "We prove ...", "A fast and accurate scheme ... is presented".
- **One person, consistently.** If the draft already uses one person consistently (first-person "we" is conventional in computational math), keep it. Third person throughout is the safest choice when rewriting a mixed-person abstract; never mix "we report" and "it is shown" arbitrarily in one paragraph.
- **Name the concrete contribution.** "Some numerical experiments have been carried out" and "A numerical comparison of these methods is presented" say nothing. Except for surveys, the abstract must state what is new (theory, method, or finding) and, when useful, the method's distinct features ("unconditionally stable for fixed physical parameters", "optimal computational complexity").
- **Do not assemble it from copied Introduction/Conclusion sentences.** Write it after the first draft, with fresh wording, so entering the paper still feels new.
- Short, clear sentences only — abstracts get machine-translated; long tangled sentences multiply mistranslation risk. Zero tolerance for typos and grammar errors: a sloppy abstract tells the referee the whole paper is rough.

## Shape examples

- Pure math, one theorem: the abstract can be one sentence stating the main result ("The main result characterizes small actions of surface groups on R-trees").
- Computational: purpose -> method idea -> theoretical results -> what the numerics verified -> possible extensions. Highlight the method's distinctive features.
