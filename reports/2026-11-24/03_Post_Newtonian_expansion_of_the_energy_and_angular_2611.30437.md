# ♻️ Post-Newtonian expansion of the energy and angular momentum flux radiated to infinity: Eccentric-equatorial orbits about a Kerr black hole

🌟 **Must-Read** · 🔬 Quality 6.5/10 · 🎯 Relevance 7/10

📎 **Citation:** Jezreel C. Castillo, Christopher Munna, Zachary Nasipak, J. David Brown, Charles R. Evans, *Post-Newtonian expansion of the energy and angular momentum flux radiated to infinity: Eccentric-equatorial orbits about a Kerr black hole*, arXiv:[2611.30437](https://arxiv.org/abs/2611.30437) [gr-qc, astro-ph.HE], submitted 23 Nov 2026.

> 💡 Closed-form weak-field formulas for the energy and angular momentum that gravitational waves carry away from a small body on an eccentric orbit in the equatorial plane of a spinning black hole are pushed to much higher order than before, and at large separations they match numerical results well enough to stand in for the numerical tables.

## 🔍 Executive Summary

The authors use the Mano-Suzuki-Takasugi analytic solutions of the Teukolsky equation, expanded symbolically in Mathematica, to compute the orbit-averaged energy and angular momentum fluxes to infinity for a point mass on an eccentric-equatorial Kerr geodesic. The results are a double series to 10PN in 1/p and to e^20 in eccentricity, and they are exact in the spin a. Two independent codes (s=+2 and s=-2) agree through 8PN and e^20, and the results reduce correctly to earlier Schwarzschild and circular-equatorial results. They find that the leading-spin (q^n) coefficients resum to closed forms in e up to 6PN in the energy flux and nearly through 10PN in the angular momentum flux. Against pybhpt Teukolsky data at a=0.9M, the 10PN energy flux reaches relative error ~1e-7 (the accuracy of the FastEMRIWaveforms flux grid) for p of about 20 at e=0.1, about 35 at e=0.5 and about 75 at e=0.7. Beyond that point the e^20 truncation, not the PN order, limits the accuracy.

## 📣 Claimed Contribution

First analytic PN flux expansions for eccentric-equatorial Kerr orbits to 10PN and e^20, exact in spin. The paper describes this as going beyond the previous 6PN/e^16 state of the art for generic Kerr orbits. Other claims: closed-form eccentricity resummations of the leading-spin flux coefficients, identification of identically vanishing terms (A_i^{S(i-1)}=0 for even i) and of where non-polynomial spin dependence first appears (6.5PN), and a mapped-out region of (p,e) where the PN fluxes can replace interpolated Teukolsky flux grids.

## ✅ Strengths

- Independent cross-check: two separate Mathematica codes built on opposite-spin-weight Teukolsky functions agree exactly through 8PN and e^20, and the results recover the Schwarzschild and circular-equatorial limits.
- The validation is honest and quantitative. It compares against both the interpolated FastEMRIWaveforms grid and higher-accuracy discrete pybhpt data (agreement ~1e-13 at p=200, e=0.1), and it separates PN truncation error from eccentricity truncation error, including an explicit fitted error model at e=0.9.
- Practically useful: it states where in (p,e) the series beats current flux-grid accuracy, and the full expressions are released in public repositories (Black Hole Perturbation Toolkit and others).
- Exact in spin, which makes it more useful than small-spin expansions for rapidly rotating primaries.
- The paper is clearly written and does not oversell; it states plainly that the series degrades at high eccentricity and at small p.

## ⚠️ Weaknesses

- Methodologically incremental. It applies the symbolic MST pipeline of Munna 2020 (Schwarzschild, also 10PN/e^20) and Castillo et al. 2025 (inclined-spherical Kerr) to a new orbit family that the same group already handled for the redshift invariant (Munna 2023). The method contains nothing new beyond speed-up tricks (Coulomb-wave representation, amplitude rescaling).
- Infinity-side fluxes only. The horizon fluxes are deferred, so the claim that the series 'could replace Teukolsky-code results' in adiabatic inspirals is not yet usable: at a=0.9 the horizon flux is suppressed only by about 2.5PN relative to the infinity flux, which is far above 1e-7 at p~20.
- Restricted to equatorial orbits, whereas Sago et al. 2026 already give generic (eccentric and inclined) Kerr results to 6PN/e^16. The gain is depth in PN order and eccentricity within a subcase, not new orbital coverage.
- Numerical validation covers essentially a single spin value (a=0.9M). Retrograde orbits and near-extremal spins, where the PN series converges worst, are not tested.
- The e^20 truncation makes the series unreliable for e of about 0.7 and above, which is exactly where EMRIs may live. A 3PN spin-dependent term without a known closed form controls the error at e=0.9.
- The physics insight is modest: resummation patterns of leading-spin terms are noted, but whether they can be derived from full PN theory is left open.

## 🤔 Skeptic's Cross-Examination

This is a bigger table from a known pipeline, for a subcase of orbits already covered at 6PN by another group. Without horizon fluxes it cannot replace anything in a real adiabatic inspiral at a=0.9. Where it would matter most (high eccentricity, small p, near-extremal spin), the e^20 truncation and the asymptotic PN series fail, so the regime where it 'replaces' Teukolsky data is the regime where Teukolsky data are already cheap.

## 🆕 Novelty in Context

The introduction positions the work honestly. It extends the group's Schwarzschild eccentric flux series (Forseth-Evans-Hopper 2016, Munna et al. 2020, Munna 2020, which already reached 10PN/e^20) and their inclined-spherical Kerr fluxes (Castillo et al. 2025, arXiv:2411.09700) to eccentric-equatorial Kerr. It uses the same machinery previously applied to the redshift invariant on these orbits (Munna 2023). The relevant competing result is Sago, Fujita, Isoyama and Nakano 2026 (arXiv:2603.27941), which gives secular changes of E, L and Q for fully generic Kerr orbits to 6PN and e^16 with numerical Teukolsky validation. That paper already covers the equatorial eccentric case at lower order. So the actual contribution is four more PN orders and four more eccentricity orders, exact in spin, for the equatorial subcase, plus the resummation observations. 'Extending beyond prior 6PN and e^16 results available for generic orbits' is accurate, but it is a depth extension, not a new capability. The authors themselves point to Khalvati-Kavanagh et al. 2026, which avoids the eccentricity expansion entirely in Schwarzschild, as the likely better route at high e. That suggests the e-expanded approach used here may already be heading toward obsolescence.

## 🎯 Relevance to Your Research

Directly relevant to EMRI modelling and self-force/PN overlap work. It gives high-order analytic Kerr eccentric fluxes, usable for checking Teukolsky codes, for filling flux grids at large p (once horizon fluxes appear), and as input to effective-one-body or hybrid models. It is a reference and data product rather than a conceptual advance. Read it if you build or validate adiabatic eccentric Kerr inspirals; skim it otherwise.

📖 **Where to start:** Introduction (positioning and the two-code cross-check); Sec. III.A (structure and spin decomposition of the flux); Sec. III.C (leading-spin resummations); Sec. III.D (numerical comparison: the error-versus-p figures and the e=0.9 error model are the most useful parts); Conclusion.

## Scores

- 🔬 **Quality:** 6.5/10
- 🎯 **Relevance:** 7/10
- 🌟 **Reading priority:** Must-Read (weighted score 6.7/10)

## 🚧 Caveats

- Fluxes to infinity only; horizon fluxes are not included, so these cannot yet replace full Teukolsky fluxes in an inspiral.
- Equatorial orbits only; generic Kerr orbits are already known to 6PN and e^16 from another group.
- Numerically validated essentially only at spin a=0.9M.
- For eccentricity around 0.7 and above, the e^20 truncation, not the PN order, limits accuracy; it is unreliable close to the separatrix.
- Only spin-dependent terms through 5PN are printed; the full 10PN expressions are in online repositories.

## In Network

- 🚩 Jezreel Castillo — extended-network collaborator
- 🚩 Zachary Nasipak — extended-network collaborator

---

🔗 [Back to the weekly digest](../2026-11-24)
