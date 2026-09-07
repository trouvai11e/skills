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

Lesson: one style per manuscript, chosen by the target journal — never stack entries copied verbatim from different journals.
