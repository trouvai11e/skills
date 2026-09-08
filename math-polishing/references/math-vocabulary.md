# Math vocabulary and symbols (deep reference — load on demand)

Terminology lookup for polishing: the right English word for a Chinese math term, how a symbol is read or spelled out in prose, and context-dependent notation pitfalls. Use it to fix mistranslated terms and to write out a symbol in words at its first definition. For sentence patterns and connectives, use `math-phrasebook.md`.

## 1. General logic and proof terms

- Assert/reason: claim, assert, deduce, infer, imply, demonstrate.
- Proof types: direct proof, indirect proof, proof by exhaustion, mathematical induction, inductive hypothesis, inductive definition.
- Statement ladder: axiom, postulate, lemma, proposition, theorem, corollary, conjecture, counterexample.
- Conditions: hypothesis, assumption, premise, major (minor) premise, necessary condition, necessity, sufficiency.
- Linkers: namely, that is, i.e. (that is), e.g. (for example). Quality judgments: well defined, of universal validity, unsolvable.

## 2. Field vocabulary (mistranslation-prone terms)

- Algebra/arithmetic: division algorithm (辗转相除法 — not "division method"), greatest common factor, least common multiple, directly (inversely) proportional, like terms, undetermined coefficients, root of unity, multiplicity (重数).
- Geometry/trigonometry: hypotenuse (斜边), included angle (夹角), cyclic polygon (内接多边形), median line, centroid, frustum (圆台), generatrix (母线).
- Calculus/analysis: deleted neighborhood (去心邻域), nowhere dense, greatest lower bound / least upper bound, left (right) continuous, left (right) derivative, dominant (majorant) series (强级数), iterated (repeated) integral, function of bounded variation, almost everywhere, annihilator (零化子), equicontinuous, sequentially compact (列紧), weak solution, residual spectrum.
- Linear algebra: spanned by ... (由……张成), partition of unity, diagonally dominant matrix, ill-conditioned problem, generalized inverse, nilpotent, idempotent, doubly stochastic matrix.
- Number theory: mutually prime (coprime), sieve method, twin primes, overdetermined equation.
- Abstract algebra/topology: germ (芽), moving frame, stereographic projection, torsion-free, wedge product.
- Dynamical systems/PDE: well-posed (properly posed) problem, variation of parameters (参数变易法), first integral (首次积分), infinitesimal generator.
- Optimization: level set, slack variable, trust region method, semidefinite programming.
- Numerical analysis: round-off error, convergence order (收敛阶), grid point, step size, refinement.
- Probability/statistics: almost sure convergence (殆必收敛), convergence in measure, martingale (鞅), maximum likelihood.

## 3. Reading symbols aloud / writing them out (elementary)

Needed when prose must spell out a symbol (talks, definitions, accessibility) or when checking that a verbal description matches the formula.

- a + b "a plus b"; a/b "a over b"; a × b "a times b / a multiplied by b".
- a ≫ b "a is much greater than b"; a ≈ b "a is approximately equal to b"; a ∝ b "a is proportional to b"; a ≯ b "a is not greater than b"; a ≮ b "a is not less than b".
- a² "a squared"; aⁿ "a to the nth power"; a⁻ⁿ "a to the minus nth power"; ⁿ√a "the nth root of a".
- a_b "a sub b"; a^b "a super b / a superscript b"; a_b² "the square of a sub b".
- n! "n factorial"; m | n "m divides n / n is divisible by m"; [x] "the integral part of x"; log_b x "the logarithm of x to the base b"; arcsin x "arc sine x".
- ∑_{i=1}^n x_i "the summation of x sub i, with i running from 1 to n".

## 4. Advanced symbols (sets, limits, function spaces, measure)

- x ∈ A "x is a member of A / x belongs to A"; A ⊊ X "A is a proper subset of X"; A∖B "the complement of B relative to A"; ∅ "the empty set (null set)"; 2^X "the set of all subsets of X"; {x | P(x)} "the set of all x with the property P".
- [a, b) "the half-open interval (open at the right)".
- b = sup A "b is the least upper bound of A" (l.u.b.); a = inf A "the greatest lower bound" (g.l.b.); limsup/liminf "the upper (lower) limit"; f(a−) "the limit of f as x approaches a from the left".
- f(n) ~ log n "f(n)/log n approaches 1 as n goes to infinity"; O/o "big oh / little oh"; f(x) ↗ b "f(x) increases, approaching the limit b".
- C^k[a,b] "the class of functions having continuous kth derivatives on [a,b]"; C₀¹(Ω) "the space of continuously differentiable functions with compact support in Ω"; BV(0,1) "the functions of bounded variation on (0,1)"; B(X,Y) "the space of all bounded linear operators from X into Y".
- supp μ "the support of the measure μ"; dμ/dν "the derivative of μ with respect to ν"; ν ≪ μ "ν is absolutely continuous with respect to μ"; ν ⊥ μ "ν and μ are mutually singular".
- σ_p(T) "the point spectrum of T"; ρ(T) "the resolvent set of T"; R(λ,T) "the resolvent of T".
- ∇·v "the divergence of v"; ∇×v "the curl of v"; Δu "the Laplacian of u"; ∂(u,v)/∂(x,y) "the Jacobian of u and v"; ∮ "the line integral around a closed path".
- x ≡ y (mod p) "x is congruent to y modulo p"; g∘f "the composition of g and f"; A* "the adjoint (Hermitian conjugate) of A"; A^{1/2} "the square root of the positive semidefinite matrix A"; E(X | Y ≥ 1) "the conditional expectation of X given Y ≥ 1"; T_h "a triangulation with mesh size h".

## 5. Notation pitfalls: context-dependent symbols

The same symbol can mean different things in different fields, and the meaning is fixed by context. In general matrix theory A > 0 means the square matrix A is positive definite; in nonnegative-matrix theory A > 0 means every entry of A is positive. Likewise fⁿ (power vs. iterate) and (x, y) (point, inner product, gcd) shift with context.

Polishing consequence: check that every such symbol is defined at first use, and flag undefined ambiguous notation instead of guessing. When a draft writes out a symbol in words, verify the wording against the field's convention.

## Appendix A. A short history of notation (for introduction color, one line at most)

= (Recorde 1557); >, < (Harriot 1631); ∞ (Wallis 1655); d, ∫ (Leibniz 1675); π (Jones 1706); e, f(x), i, ∑ (Euler, 18th c.); n! (Kramp 1808); congruence notation (Gauss 1801); ∈, ∃ (Peano 1890s); O(·) (Bachmann 1894); ∅ (Weil 1939); ⌊x⌋, ⌈x⌉ (Iverson 1962); ■ end-of-proof (Halmos).
