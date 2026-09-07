# Diagnose the failure mode before editing

Before rewriting, identify the main problem(s):

## Structural / focus

- too many theorems and lemmas — the paper loses its center (a ten-page paper with a dozen theorems)
- theorem statements missing hypotheses that were introduced during the derivation
- lemmas dumped together at one spot instead of placed just before the theorem that uses them
- sectioning too fragmented (half-page subsections) or too monolithic (a long paper with no visible landmarks)
- no Conclusions section in a long paper
- the introduction reviews a whole field's history instead of the work relevant to this paper
- application prospects crowding out the actual results

## Section-level

- abstract: opens with "In this paper" / "This paper"; contains display formulas or heavy notation; cites references as bare numbers ([10]); mixes first and third person; contains empty result sentences ("Some numerical experiments have been carried out")
- introduction: opens with a dump of symbols and definitions; opens with generic filler ("Polynomials are widely used ..."); buries the problem; self-praise or attacks on others
- body: display-equation chains of five or more lines with no intervening text; elementary derivations spelled out in full; "It is easy to see / It is trivial" claims a referee cannot quickly verify; figures and tables presented but never discussed
- conclusion: repeats the abstract/introduction word for word; introduces brand-new ideas; overclaims; apologizes
- references: inconsistent format; entries never cited in the text; non-alphabetical order in a math journal; missing fields

## Sentence-level

- sentences opening with a math symbol, especially right after a sentence ending in one
- formulas and text colliding without commas or intervening words ("If $x > \pi f(x) < 0$")
- article misuse: "the Schur decomposition" for a non-unique object, missing "a"/"the"
- Chinglish connectives: "Although ..., but ..."; "As far as ... is concerned"
- long single-sentence chains that separate subject and verb by a screenful of modifiers
- unnecessary abbreviation inflation (CS, LS, DS, SC, IE ...)

## Priority order

`paper type -> section job -> focus (one theme) -> theorem & proof discipline -> display & notation hygiene -> sentence polish`

Do not sentence-polish a draft whose section job or theorem architecture is wrong. Surface the structural problem first, then polish.
