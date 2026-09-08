# Worked examples (deep reference — load on demand)

Curated exemplars from published math papers and real revision cases. Use them as few-shot anchors when the user asks "show me an example", when a rule needs a concrete demonstration, or when drafting a section from scratch. Do not copy their sentences into the user's draft — adapt the pattern, not the words.

## 1. Titles

Good patterns:

- An algorithm for the machine calculation of complex Fourier series — the first FFT paper; names the contribution plainly (algorithm, machine computation, complex Fourier series).
- Viscosity solutions of Hamilton–Jacobi equations (Crandall–Lions) — object + problem class.
- Period three implies chaos (Li–Yorke) — the theorem itself as the title; works only for results that speak for themselves.
- Generation of finite difference formulas on arbitrarily spaced grids — "arbitrarily" is the load-bearing qualifier in a crowded field.
- Overcoming corner singularities using multigrid methods — gerund + using, acceptable shape.
- Can one hear the shape of a drum? (Kac) / One cannot hear the shape of a drum (Gordon et al., 26 years later) — question titles and their answers; expository flair, high memorability.
- Hilbert's tenth problem is unsolvable — a declarative sentence as title, for a definitive result.
- How long is the coast of Britain? (Mandelbrot, Science, 1967) / Can we make mathematics intelligible? (Boas, Amer. Math. Monthly, 1981) — more question titles; expository or field-defining papers only.
- Good approximation by splines with variable knots (de Boor, 1973) / Multi-level adaptive solutions to boundary-value problems (Brandt, 1977) / Boundary layer resolving pseudospectral methods for singular perturbation problems — crowded fields narrowed by load-bearing qualifiers ("variable", "multi-level adaptive", three keywords where each is indispensable).

Anti-patterns (too broad or empty — book titles, not paper titles):

- Computational methods for Euler equations / Numerical analysis for fluid mechanics.
- An efficient numerical method for solving a class of delay differential equations — "efficient" and "a class of" carry no information.
- A weakly and strongly convergent numerical algorithm for solving ... — logically redundant stack (strong implies weak); cut to "A strongly convergent ..." or "A convergent ...".

## 2. Abstracts

One-sentence abstract for a single-theorem paper (Proc. Amer. Math. Soc. style):

> A class of piecewise continuous, piecewise $C^1$ transformations on the interval $[0,1]$ is shown to have absolutely continuous invariant measures.

Structured pure-math abstract (Green–Tao, Annals of Mathematics, 2008): states the result, then enumerates the ingredients, marking which one is new:

> We prove that there are arbitrarily long arithmetic progressions of primes. There are three major ingredients. The first is Szemerédi's theorem ... The second, which is the main new ingredient of this paper, is a certain transference principle ... The third ingredient is a recent result of Goldston and Yıldırım. Using this, one may place the primes inside a pseudorandom set of "almost primes" with positive relative density.

Purpose -> result -> idea (a short note refining a definition):

> In this short note we suggest a refinement for the definition of viscosity solutions for parabolic equations. The new version of the definition is equivalent to the usual one and it better adapts to the properties of parabolic equations. The basic idea is to determine the admissibility of a test function based on its behavior prior to the given moment of time and ignore what happens at times after that.

Standard computational abstract (purpose -> method idea -> theory -> numerics -> extension), J. Comput. Phys., 1994:

> In this paper the authors discuss the applications of high-order compact finite difference methods for shock calculations. The main idea is the definition of a local mean that serves as a reference for introducing a local nonlinear limiting to control spurious numerical oscillations while keeping the formal accuracy of the scheme. For scalar conservation laws, the resulting schemes can be proven total variation stable in one-space dimension and maximum norm stable in multispace dimensions. Numerical examples are shown to verify accuracy and stability of such schemes for problems containing shocks. The idea in this paper can also be applied to other implicit schemes such as the continuous Galerkin finite element methods.

Abstract that must cite a specific predecessor — full citation, not a bare number (SIAM J. Numer. Anal., 1996):

> Saranen [Math. Comp., 48 (1987), pp. 485–502] proved local estimates in Sobolev norms for the Galerkin method applied to strongly elliptic equations on smooth closed curves in the plane. We extend his results to the case of open curves. ...

Avoiding display formulas by narration — instead of displaying the hyperbolic and viscous conservation laws and the error bound, write:

> It is proved that for scalar conservation laws, the viscous solution converges to the inviscid one with order 1/2. If the flux is strictly convex and the entropy solution is piecewise smooth, the order improves to 1.

Anti-pattern: "This paper develops an optimal-order multigrid method for the TRUNC plate element." — one bare sentence; the reader cannot tell the method, the difficulty, or the value.

Five-verb skeleton for a longer applied abstract (DiPerna–Lions, Annals of Mathematics, 1989): We study ... / We prove that ... / From this stability result we deduce global existence ... / Our method relies upon ... / It allows us to overcome ... — study -> prove -> deduce -> method -> overcome.

One-sentence abstract, active form (JAMS, 1996): "The main result characterizes small actions of surface groups on R-trees." — pair with the passive one-sentence form above; pick one voice.

Enumerating the selling points inside the abstract (SINUM, 1999): the scheme's two features are listed as (i) unconditionally stable for fixed physical parameters, and (ii) reducible to one-dimensional equations of optimal computational complexity — numbered highlights make the contribution quotable.

Self-citation in an abstract — full citation, "proposed by the authors" (SISC, 2001):

> This method is based on the random projection method proposed by the authors for general hyperbolic systems with stiff reaction terms [W. Bao and S. Jin, J. Comput. Phys., 163 (2000), pp. 216–248], where ...

Useful abstract verb strings (SINUM, 2000): is concerned with / differs in many aspects from / leads to / emphasis is on / results reported previously are not entirely satisfactory / provide sharper and more precise estimates. Note the diplomatic negation "not entirely satisfactory".

Anti-pattern, too thin (DCDS, 2001): "The method of generalized quasilinearization is extended to semilinear degenerate elliptic boundary value problems." — the reader cannot judge the method's value or the result's strength.

## 3. Introductions

Opening with a classical anchor, three sentences to the actual problem (Trans. Amer. Math. Soc., 2006):

> Edward Waring stated in 1770 that every integer is a sum of at most 9 positive integral cubes, also a sum of at most 19 biquadrates, and so on. Later on Jacobi and others considered the problem of finding all the decompositions of a given number into the least number of powers, [Di]. In this paper we are concerned with a similar question for general homogeneous forms.

Opening that states problem and difficulty at once (Computing, 1996):

> Among various techniques for solving partial differential equations, multigrid methods have proven to be one of the most efficient approaches. The efficiency of those methods, however, depends crucially on appropriate underlying multilevel structures. As such multilevel structures are not naturally available in most unstructured grids, multigrid methods are in general not easy to apply.

Opening with a concrete incident and a closing rhetorical question (BIT, 1983):

> The preparation of this note was prompted by the appearance, in the chemistry literature, of a 16-digit table of a Gaussian quadrature formula ..., a table which we suspected is accurate to only 1–2 decimal digits. How does one go about convincing a chemist, or anybody else for that matter, that his Gaussian quadrature formula is seriously defective?

Higham's delete-the-first-sentence compression:

> Before: Polynomials are widely used as approximating functions in many areas of mathematics and they can be expressed in various bases. We consider here how to choose the basis to minimize the error of evaluation in floating point arithmetic.
> After: In which basis should we express a polynomial to minimize the error of evaluation in floating point arithmetic?

Outline paragraph done well — one sentence per section, describing content, not repeating titles (Trans. Amer. Math. Soc., 2005, shortened):

> We devote Section 2 to a discussion of those aspects of warped products and model spaces which will be instrumental for our comparison analysis. The general setup for the comparison techniques is then constructed in Section 3. ... The local version of our main result is then established in Section 7. Finally the proofs of Theorem A and its corollaries are presented in Sections 8 and 9, respectively.

Anti-pattern: an intro paragraph of universally known facts that can be deleted wholesale:

> As everyone knows, a large number of the operators which arise naturally in applications (e.g., mathematical physics, quantum mechanics and partial differential equations) are unbounded [18]. However, many of these unbounded operators have bounded inverses ... — every sentence deletable; nothing about this paper.

One line of simple notation, then straight to the problem (Math. Comp., 1979) — the exception done right:

> Let A be a positive definite matrix of order n with eigenvalues $\lambda_1 \geq \cdots \geq \lambda_n > 0$ ... In some applications, one must obtain an estimate of $\lambda_1$ without going to the expense of computing the complete eigensystem of $A$. A simple technique ... is the power method.

One glanceable symbol line is allowed; a dump of definitions is not. The problem arrives in sentence two.

Objectivity anti-patterns (never write these):

- Self-praise: "Our new result is extremely important toward the proof of von Neumann's conjecture." — 文章在自己,评价在别人.
- Putting others down: "The result of this paper is most general, a trivial consequence of which is the main result of [3]." — imagine [3] is your own paper.
- Strident correction: "The conclusion of the main theorem of [3] is completely wrong, because the key inequality in the proof is unfortunately not correct." — even a genuine error is pointed out gently.

Middle moves (published patterns):

- Purpose -> history -> question -> answer (Proc. Amer. Math. Soc., 2006): "The main purpose of this paper is to prove ... (see [9, Ch. 5] for the classical ...)" -> "In analogy with ... we ask whether ..." -> "It turns out that the answer is yes, and ... we obtain more quantitative estimates." The suspense-and-reveal "It turns out that the answer is yes" is a legitimate rhetorical move.
- Giving the reason (boundary-element paper): "This gives a simpler set of equations on the boundary and hence a more efficient starting point ... than the direct formulation ... used in previous studies. More importantly, this will allow us to ..."

Outline variants beyond "This paper is organized as follows":

- "The present paper is built up as follows. The physical, mathematical and numerical aspects of ... are treated in Section 2, while ..." (an outline that also covers Appendices A and B).
- "Results ... are summarized in Section 3, which can be read without knowledge of the details of our numerical method presented in Section 4." — annotating a skip-reading route for the reader.

## 4. Conclusions

Three-paragraph shape: short summary -> consequence of the study -> extension/future work (J. Comput. Chem., 1993, abridged):

> The first conclusion to be drawn from the numerical evidence presented earlier is that the multigrid method is the most efficient method for the two test problems ... Secondly, the advantage of multigrid grows with the problem size ...
> A point that should be stressed is that the SOR and CG results reported here are based on highly optimized codes ... the results presented here for the multigrid method are conservative ...
> Finally, while we have considered only the LPBE in this paper, the multigrid method can be extended to nonlinear problems through ... and their application to the NPBE will be investigated in a future paper.

Two-sentence minimal conclusion with a sequel announcement (use only with real certainty):

> What we have seen from the above is the convergence of a piecewise linear approximation method for the class of Li–Wang piecewise monotone mappings of the unit interval. A different technique can be used to prove the convergence of the algorithm for the class of piecewise convex mappings of an interval, and the resulting paper will be published elsewhere.

## 5. Acknowledgments

- The financial support of the Natural Sciences and Engineering Research Council of Canada (NSERC) is gratefully acknowledged.
- The author gratefully acknowledges the support of the National Science Foundation under grant number DMS1234567.
- This work was supported in part by the National Natural Science Foundation of China (Grant No. 12345678).
- We are grateful to the two anonymous referees for useful comments and suggestions.
- The author is indebted to Dr. J. Smith for many helpful discussions, and to Dr. S. Fisher for correcting two errors in an earlier version of the paper.
- Part of this work was carried out while this author was visiting Peking University.
- This work was supported by the US Department of Energy under Contract # ... (agency + contract number pattern).
- We thank Dr. Smith for valuable comments, and the Nanjing University Research Fund as well as the US National Science Foundation for the financial support. (person and two agencies in one sentence — note the repeated "for")

Revision case — telegraphic to standard:

> Before: Supported by the National Natural Science Foundation of China (No. 88886666) and Key Laboratory of Education Ministry.
> After: The research was supported by the National Natural Science Foundation of China (No. 88886666) and the Key Laboratory of the Ministry of Education.

## 6. Revision before/after (structural cosmetics)

Abstract — cut filler, person consistency, no repetition:

> Before: In this paper we consider the approximate eigenvalues and approximate eigenspaces for generalized Rayleigh quotient, and present some residual bounds. Our bounds will improve the corresponding ones.
> After: We consider approximate eigenvalues and eigenspaces for generalized Rayleigh quotients and present some residual bounds which improve the existing ones.

Intro opening — symbols-first dump compressed into problem-first (note the set definition gets its own display):

> Before: Throughout this paper $\|A\|_2$ stands for the Euclidean norm of a real-valued matrix A and $A^\dagger$ denotes the Moore–Penrose generalized inverse of A. We define the set $M_k = \{B \in \mathbb{R}^{n\times n}: \operatorname{rank} B = k\}$ for each $k = 1,\dots,n$. Given $A \in \mathbb{R}^{n\times n}$ of full rank and a positive integer $k < n$ we are interested in the best approximation problem $\min\{\|A-B\|_2 : B \in M_k\}$.
> After: We are interested in the best approximation problem
> $$\min\{\|A-B\|_2 : B \in M_k\}$$
> where $A \in \mathbb{R}^{n\times n}$ has rank $n$ and $k < n$,
> $$M_k = \{B \in \mathbb{R}^{n\times n} : \operatorname{rank} B = k\},$$
> and $\|A\|_2$ is the Euclidean norm.

Comma-splice and broken agreement in a results sentence:

> Before: Extensive simulations are performed, as a result, the finite difference WENO schemes with multilevel time discretization have higher accuracy maintain nonoscillatory properties and more cost effective than WENO scheme with Runge-Kutta time discretization.
> After: Extensive simulations are performed, which indicates that the finite difference WENO schemes with the multilevel time discretization can achieve a higher accuracy and are more cost effective than the WENO scheme with the Runge-Kutta time discretization, while still maintaining nonoscillatory properties.

The 60-word single sentence split into three:

> Before: In this section a new three-dimensional autonomous nonlinear dynamical system with only two quadratic terms but can generate a chaotic attractor bridging the gap between the Lorenz system and the Chen system which can be described by a system of ordinary differential equations is introduced, as follows.
> After: In this section a new three-dimensional autonomous nonlinear dynamical system is introduced. This system has only two quadratic terms but can generate a chaotic attractor bridging the gap between the Lorenz system and the Chen system. The system can be described by a system of ordinary differential equations, as follows.

## 7. Reference entries — same paper, six publisher styles

C. Shannon, "A mathematical theory of communication", Bell Syst. Tech. J. 27 (1948), 379–423:

- AMS: C. Shannon, A mathematical theory of communication. Bell Syst. Tech. J. 27 (1948), 379–423.
- Elsevier: C. Shannon, A mathematical theory of communication, Bell Syst. Tech. J. 27: 379–423 (1948).
- IMA: Shannon, C. 1948 A mathematical theory of communication. Bell Syst. Tech. J. 27, 379–423.
- SIAM: C. Shannon, A mathematical theory of communication, Bell Syst. Tech. J. 27 (1948), pp. 379–423.
- Springer-Verlag: Shannon, C. (1948) A mathematical theory of communication. Bell Syst. Tech. J. 27, 379–423.
- World Scientific: C. Shannon, A mathematical theory of communication, Bell Syst. Tech. J. 27 (1948), 379–423.

Lesson: one style per manuscript, chosen by the target journal — never stack entries copied verbatim from different journals.

## 8. Body: introducing the governing equations

Name the equation's meaning through its parameters, not just its symbols:

> The Poisson–Boltzmann equation, characterized by a Debye screening parameter $\kappa$, has the form [formula], where $y = ze\psi/(k_B T)$ is the scaled nondimensional potential.

> The Perron–Frobenius operator is defined via [formula] for all $f \in L^1$.

Pattern: state the equation, then a "where"-clause that explains each unknown function and parameter's physical meaning.

## 9. Paragraph-level exemplars (reusable skeletons)

- "Why the method matters" paragraph (discontinuous Galerkin): locate the method first ("somewhere between a finite element and a finite volume method"), list the advantages, then draw the boundary with its closest relative: "An important distinction between ... is that ...". Skeleton: locate -> frame value -> scenarios -> distinction from the nearest method.
- Survey motivation paragraph (Budd–Huang–Russell, Acta Numerica, 2009): plain words, full precision. Chain: phenomena (interfaces, shocks, singularities ...) -> standard practice ("it is typical to impose some form of spatial mesh") -> where it fails ("this strategy may not be effective in the case of ...") -> the proposal's benefit and cost ("Mesh adaptation should thus be used with care").
- Chronicle of a method's history (van Leer, CiCP, 2006): dash entries of "Name, year" (Godunov, 1959 / Fromm, 1968 / Wesseling, 1973 ...), one sentence of contribution and one of significance each; close with the open challenge ("The price one has to pay for all this goodness is ..."). The template for a history-of-the-field paragraph.

## 10. Sentence-level graded comparisons (bad / fair / good)

1. Conditionals. Bad: "If $x > \pi f(x) < 0$" (symbols collide, no punctuation). Fair: "$f(x) < 0$ if $x > \pi$." Good: "If $x > \pi$, then $f(x) < 0$." — front the if-clause.
2. Multiple conditions. Bad: "Let $x \neq 0, y \geq 1$. Then $f(x,y) \leq -1.$" Fair: "$x \neq 0$ and $y \geq 1$ imply $f(x,y) \leq -1$." Good: "If $x \neq 0$ and $y \geq 1$, then $f(x,y) \leq -1$." — join conditions with and, not a comma.
3. Symbol-dense causality. Bad: "Since $p^{-1}+q^{-1}=1$, $\|\cdot\|_p, \|\cdot\|_q$ are dual norms." Good: "Since $p^{-1}+q^{-1}=1$, the norms $\|\cdot\|_p$ and $\|\cdot\|_q$ are dual." Better: "The norms $\|\cdot\|_p$ and $\|\cdot\|_q$ are dual since $p^{-1}+q^{-1}=1$." — give symbols a noun label; link symbol pairs with and.
4. Quantifier scope position. Bad: "It suffices to show that $\|H\|_p = n^{1/p}$, $1 \leq p \leq 2$." Bad: "... that for $1 \leq p \leq 2$, $\|H\|_p = n^{1/p}$." Fair: parenthesized "($1 \leq p \leq 2$)". Good: "It suffices to show that $\|H\|_p = n^{1/p}$ for $1 \leq p \leq 2$" or "... that if $1 \leq p \leq 2$, then $\|H\|_p = n^{1/p}$."
5. Citation comma. Bad: "For $n = r$ (1.2) holds with $\delta_r = 0$." Good: "For $n = r$, (1.2) holds with $\delta_r = 0$" or "Inequality (1.2) holds with $\delta_r = 0$ for $n = r$."
6. Category statements drop the article. Bad: "The stationary densities are the fixed points of the Markov operators." Good: "Stationary densities are fixed points of Markov operators" / "A stationary density is a fixed point of Markov operators."
7. Symbol-opening rescue. Bad: "From the above formula we have $\int f(t)\,dt = e$. $f(s) \geq e$ for at least one $s \in [0,1]$ since $f$ is not a constant function." Good: "We have $\int_0^1 f(t)\,dt = e$ from the above formula. The inequality $f(s) \geq e$ is valid for at least one $s \in [0,1]$ since $f$ is not a constant function."

## 11. Where to find model prose

Not every published paper is well written — learn from established venues, and beware of profit-driven new journals. Reliable hunting grounds: Amer. Math. Monthly, Math. Intelligencer, Notices of the AMS, SIAM Review (general); Annals of Mathematics, Inventiones, JAMS, Trans. AMS (top research); Math. Comp., Numer. Math., SIAM J. Numer. Anal., SIAM J. Sci. Comput., J. Sci. Comput. (computational); CPAM, SIAM J. Appl. Math., SIAM J. Math. Anal. (applied); Math. Program., SIAM J. Optim., SIAM J. Control Optim. (optimization); J. Comput. Phys., CiCP (computational physics). Award-winning expository prose: Lester R. Ford Award (MAA), SIAM Outstanding Paper Prizes, AMS Steele Prize for mathematical exposition, AMS Levi L. Conant Prize.
