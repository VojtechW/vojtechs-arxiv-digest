# 📐 Analytical Fluxes from Generic Schwarzschild Geodesics

**arXiv:** [2605.13847](https://arxiv.org/abs/2605.13847)
**Authors:** Majed Khalaf, Chris Kavanagh, Ofri Telem
**Categories:** gr-qc, hep-th
**Collaborator flags:** Chris Kavanagh (T2); Adam Pound, Leor Barack acknowledged

## Summary

The authors present an analytic algorithm to compute gravitational-wave flux Fourier coefficients (the Teukolsky $Z^{+}_{nlm}$ amplitudes) for bound Schwarzschild geodesics of arbitrary eccentricity, without expanding in eccentricity. The method writes each Schwarzschild Fourier element as a single closed-form linear operator $K_{nm}[f]$ acting on a function $f$, projected onto Keplerian Fourier coefficients that were previously derived in closed form via the authors' "Quantum Spectral Method". $K_{nm}[f]$ is expanded in a hybrid PN / Chebyshev / Gegenbauer basis chosen for uniform convergence on $r_p \leq r \leq r_a$. Benchmarks against BHPT numerics give $10^{-5}$ total-flux accuracy at $(p,e)=(12.5,0.5)$ and per-mode WRE below $10^{-6}$ for dominant modes at $(p,e)=(10,0.8)$.

## Key Results

- A clean identity reducing any Schwarzschild radial Fourier element to a Keplerian one with explicit kernels and a Kepler frequency-matching choice that aligns the turning points $(r_p, r_a)$ between the Schwarzschild and auxiliary Keplerian orbit. This is exact, not an eccentricity expansion.
- Closed-form Chebyshev/Bessel expansion of phase terms, supplemented by Chebyshev-U expansion of arctan-type functions and Gegenbauer expansion of $\log^k(r)$ terms. Square-root factors removed via integration by parts.
- Total-flux accuracy $10^{-5}$ at $(p,e)=(12.5,0.5)$; WRE below $10^{-6}$ per dominant mode at $(p,e)=(10,0.8)$ using 15-20PN expansion.
- Roadmap: direct extension to equatorial Kerr (and generic Kerr including inclination), plus analytic continuation to unbound/post-Minkowskian regimes.

## Strengths

- Genuinely solves the eccentricity-expansion bottleneck that has constrained analytic EMRI flux work. The method is structurally exact in $e$ for the orbit-dependent kernel.
- Mathematically clean: one linear operator + exact Keplerian-Fourier formula. Chebyshev/Gegenbauer choice is principled (uniform convergence on a closed interval).
- Nontrivial numerical benchmarks against BHPT at moderate $(p=12.5, e=0.5)$ and strong-field/high-eccentricity $(p=10, e=0.8)$ points with sensible weighted error metric.

## Weaknesses / Caveats

- Despite "Generic" in the title, the input Green's function is a 15PN expansion. Accuracy is ultimately bounded by the PN order of $R^{in}_{lm}$. Method is "analytic" in orbit eccentricity but still PN-truncated in the Teukolsky sector.
- Only $Z^{+}_{nlm}$ (infinity fluxes) computed; horizon fluxes deferred.
- Convergence claims rest on numerical benchmarks rather than rigorous bounds.
- "$O(1)$ faster than BHPT" performance claim is vague.
- Kerr extension repeatedly advertised but not done. Generic-inclination Kerr needs nontrivial adaptation.

## Novelty Assessment

The genuinely new ingredient is the explicit reduction of a Schwarzschild radial Fourier element to a Keplerian one with a controllable kernel, combined with a Chebyshev/Gegenbauer hybrid expansion well-adapted to the bounded interval $[r_p, r_a]$. The trick of choosing the Keplerian $\alpha$ and $L_K$ so that the auxiliary orbit shares $(r_p, r_a)$ with the Schwarzschild orbit is elegant. The hybrid PN+Chebyshev expansion (vs. the more conventional small-$e$ expansion) is the main practical step beyond Munna 2008.10622 / Sago-Fujita.

Self-assessment vs cited work checks out: prior analytic Schwarzschild eccentric-orbit flux work (Munna et al., Sago-Fujita) is genuinely small-$e$ expansion. Whittall-Barack-Long 2025 uses Gegenbauer reconstruction but for numerical self-force, not analytic fluxes. So the analytic-in-$e$ claim is real and the niche is not already filled.

## Relevance to Vojtěch

Highly relevant. This sits squarely in Schwarzschild Teukolsky-flux analytics with explicit eccentric-orbit Fourier-domain machinery, intersecting Vojtěch's interests in (i) analytic structure of perturbation theory for EMRIs, (ii) eccentric orbit treatment, (iii) PN/Kerr matching — the method is conceptually a Schwarzschild-Kepler matching at the Fourier-coefficient level. The flagged Kerr extension would touch his work on Kerr geodesic-resonance and orbital-resonance analytic structure.

## Scores

- **Quality:** 7.5/10
- **Relevance:** 8/10
- **Recommendation:** Should-Read
