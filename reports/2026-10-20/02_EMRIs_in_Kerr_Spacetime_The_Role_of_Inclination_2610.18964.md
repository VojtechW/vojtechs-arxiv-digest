# 💫 EMRIs in Kerr Spacetime: The Role of Inclination Diffusion

🌠 **Should-Read** · 🔬 Quality 5/10 · 🎯 Relevance 5/10

📎 **Citation:** Yael Alush, Nicholas C. Stone, Scott A. Hughes, *EMRIs in Kerr Spacetime: The Role of Inclination Diffusion*, arXiv:[2610.18964](https://arxiv.org/abs/2610.18964) [astro-ph.GA, astro-ph.HE, gr-qc], submitted 13 Oct 2026.

> 💡 Simulations that let random stellar encounters keep tilting a compact object's orbit around a spinning giant black hole find that rapid spin roughly doubles the rate of slow gravitational-wave inspirals relative to direct plunges, and that these inspirals end up strongly biased toward orbits that co-rotate with the black hole.

## 🔍 Executive Summary

The authors write diffusion coefficients for energy, the axial angular momentum and the Carter constant from two-body scattering. They then average them over Kerr geodesics and run orbit-averaged Langevin Monte Carlo simulations, with gravitational-wave losses taken from the Gair-Glampedakis numerical kludge. They compute the fraction of captures that become inspirals rather than plunges, plus differential rates and inclination and eccentricity distributions, for 10^4 and 10^6 solar-mass black holes and 1.4, 10 and 50 solar-mass compact objects. For a 10^6 solar-mass black hole and 10 solar-mass objects, the integrated rate goes from 7.2e-9 per year (Keplerian orbits) to 1.3e-8 (Schwarzschild geodesics) to 2.8e-8 (spin 0.9), and saturates near spin 0.99. Over all semimajor axes, the inclination distribution is close to the earlier fixed-inclination prediction. Letting inclination evolve mainly suppresses retrograde inspirals that form at large semimajor axes (about a factor of 5) and erases an initially anisotropic distribution of orbit orientations.

## 📣 Claimed Contribution

A framework for inclination diffusion driven by two-body encounters for orbits on Kerr geodesics: local diffusion coefficients in energy, axial angular momentum and Carter constant, averaged over the orbital torus, used in 3D Monte Carlo simulations that go beyond the fixed-inclination approximation of Amaro-Seoane et al. 2013. The paper also claims that substantial spin enhances the inspiral rate by about 2.5, and that geodesic rather than Newtonian orbits raise it by a similar factor even without spin. It also claims a prograde-biased inclination distribution that could help pick out loss-cone inspirals in future samples, plus a Teukolsky-based error estimate (with fitted correction factors) for the Gair-Glampedakis kludge fluxes.

## ✅ Strengths

- To my knowledge, the first loss-cone Monte Carlo for inspirals around spinning black holes in which inclination evolves under scattering instead of being frozen. That makes it a real, if incremental, step past Amaro-Seoane et al. 2013 and the 2026 fixed-inclination follow-ups.
- Honest check of the gravitational-wave flux model: Gair-Glampedakis kludge fluxes are compared with Teukolsky fluxes from the Hughes code. Errors are under 10% at pericentre at or beyond 10 gravitational radii, about 50% at 3, and about a factor of 2 at 2. The paper gives power-law correction fits.
- Sensible internal checks: the 3D code at spin 0.001 reproduces the 2D geodesic results, and the diffusion coefficients reduce to the standard 2D ones in the non-spinning limit.
- Useful output for people building waveform and population models: inclination-eccentricity distributions at fixed orbital frequency, broken down by initial semimajor axis (Figs. 8-10).
- The limitations section is unusually candid: it lists neglected resonant relaxation, isotropic field stars, torus averaging, loss-cone shielding and the use of a single-mass population.

## ⚠️ Weaknesses

- The 'Kerr' diffusion coefficients are Newtonian. The local coefficients drop all spin terms and use Newtonian integrals of motion, so the Carter-constant coefficient is just Newtonian diffusion of total angular momentum minus its axial part. Diffusion coefficients for the axial angular momentum were already in Merritt 2013 and Einsel & Spurzem 1999. The only relativistic ingredient is the averaging weight along geodesics, and the appendix itself reports that a Newtonian weight gives only small deviations. The paper concedes that Xin 2026 already derived the equivalent inclination-diffusion coefficients.
- The headline effect of inclination diffusion is never isolated in a controlled experiment. The 'fixed-inclination' comparison does not rerun the 3D code with inclination frozen. Instead it rescales the 2D geodesic success-fraction curves with the analytic Amaro-Seoane scaling for the critical semimajor axis and then averages over inclination. The difference between live and fixed inclination therefore mixes real dynamics with the error of that analytic scaling.
- On the paper's own fiducial model, the inclination distribution summed over all semimajor axes is 'quite close' to the fixed-inclination prediction. The titular effect mostly survives as retrograde suppression at large semimajor axes and as erasure of initial anisotropy.
- The factor of about 2.5 from 'geodesics versus Newtonian orbits' is largely a statement about where the plunge boundary sits. The Keplerian runs use a minimum pericentre of 8 gravitational radii, a convention the paper itself calls ambiguous, and Peters fluxes are applied on geodesics with no clear pericentre mapping. Mancieri et al. had already shown that more relativistic orbit treatments raise the inspiral fraction.
- The spin enhancement in the paper's own Table 1 is 2.1 to 2.2 over Schwarzschild geodesics for 1.4 and 10 solar-mass objects, about 1 for 50 solar-mass objects, and 1.0 for a 10^4 solar-mass black hole. 'A factor of about 2.5' is a generous summary, and it is in line with the 'modest when inclination-averaged' result of Zhang & Amaro-Seoane 2026.
- The kludge underestimates fluxes by up to a factor of 2 at pericentres of about 2 to 3 gravitational radii. That is exactly the prograde, high-spin regime that drives the spin effect, yet the paper does not apply its own correction fits.
- Trajectories that wander below eccentricity about 0.98 (for 10 solar-mass objects) are terminated. How they enter the success-fraction denominator, and how sensitive the results are to this cut, is not shown.
- Absolute rates of about 1e-8 per year for a Milky-Way-like nucleus sit well below the usual 1e-7 to 1e-6 estimates and are not discussed. Only the ratios are interpretable.
- The arXiv LaTeX source contains tracked-change markup, with old (red) and replacement (blue) text side by side, plus inline co-author comments. Depending on how the macros render, the PDF may show duplicated or contradictory passages, for example two different correction fits for the kludge fluxes.

## 🤔 Skeptic's Cross-Examination

Strip away the geodesic averaging, which the authors admit barely matters, and this is Newtonian 3D angular-momentum diffusion with a spin-dependent plunge boundary. The rate gain from spin is the long-known asymmetry of that boundary. The effect of inclination diffusion is measured against an analytic rescaling rather than a frozen-inclination run of the same code, and on the integrated distribution it mostly cancels anyway. The 'geodesics give 2.5 times more inspirals' headline is a statement about the 8 gravitational-radius Keplerian convention, not new physics.

## 🆕 Novelty in Context

The paper positions itself against Amaro-Seoane, Sopuerta & Freitag 2013 (arXiv:1205.4713), which works at fixed inclination and finds up to a factor of about 30 enhancement for specific prograde inclinations, and against more recent fixed-inclination Kerr work (Vazquez-Aceves et al. 2022, Sun et al. 2026, Zhang & Amaro-Seoane 2026). The latter already found that the inclination-averaged spin enhancement is modest. This paper's factor of about 2 confirms that rather than overturning it. A co-author comment in the source shows a 'first ever' claim was deliberately removed, which is appropriate. Xin 2026 (arXiv:2606.18050) already formulated a 2D Fokker-Planck equation for diffusion in the size and orientation of angular momentum, with spin-dependent loss-cone boundaries, for tidal disruptions; the authors themselves say his coefficients are 'equivalent to the Newtonian limit' of theirs. Since their own local coefficients are Newtonian, the formalism is new only in averaging over geodesics and in its application to inspirals with a live Monte Carlo. The geodesic-versus-Keplerian enhancement extends the Newtonian-to-post-Newtonian trend of Mancieri et al. 2025 (arXiv:2409.09122, 2509.02394). The real contribution is narrower than the abstract suggests: the first inspiral Monte Carlo around spinning black holes with live inclination, plus a Teukolsky check of the kludge fluxes. It is not a new relativistic diffusion theory.

## 🎯 Relevance to Your Research

Moderately relevant to an extreme-mass-ratio theorist as astrophysical input rather than as gravitational physics. It gives expected inclination and eccentricity distributions for loss-cone inspirals around spinning black holes, which matter for which parts of generic-orbit Kerr parameter space waveform and self-force models must cover, and it flags high-eccentricity, prograde, strong-field pericentres. The Teukolsky-versus-kludge flux comparison (Sec. 3, Fig. 1) is a small, reusable quantitative result. There is no new two-body or perturbation theory content.

📖 **Where to start:** Sec. 3 (kludge versus Teukolsky flux errors, Fig. 1); Sec. 5, Table 1 and Figs. 8-10 (integrated rates and inclination-eccentricity distributions); Sec. 6.2 (summary and honest list of approximations). Skip Sec. 2.2 unless you need the coefficients: they are Newtonian.

## Scores

- 🔬 **Quality:** 5/10
- 🎯 **Relevance:** 5/10
- 🌠 **Reading priority:** Should-Read (weighted score 5.2/10)

## 🚧 Caveats

- The diffusion coefficients are Newtonian; 'Kerr' enters only through the plunge boundary and the averaging along geodesics, which the authors say barely matters.
- The live-versus-fixed-inclination comparison uses an analytic rescaling, not the same code with inclination frozen; summed over all orbits, the inclination distribution matches the old fixed-inclination prediction.
- The spin enhancement in the paper's own table is about 2 and vanishes for 50 solar-mass objects or 10^4 solar-mass black holes; 'about 2.5' is generous.
- The gravitational-wave fluxes come from a kludge that underestimates them by up to a factor of 2 in the strong-field prograde regime that drives the result; the paper's correction fits are not applied.
- The arXiv source still carries tracked-change markup and co-author comments; parts of the PDF may read as duplicated or inconsistent.

## In Network

- 🚩 Scott Hughes — extended-network collaborator

---

🔗 [Back to the weekly digest](../2026-10-20)
