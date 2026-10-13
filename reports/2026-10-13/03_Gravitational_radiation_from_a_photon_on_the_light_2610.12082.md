# 🎵 Gravitational radiation from a photon on the light ring: multipole fluxes and the logarithmic divergence

🌠 **Should-Read** · 🔬 Quality 7.5/10 · 🎯 Relevance 5.5/10

📎 **Citation:** Enrico Barausse, *Gravitational radiation from a photon on the light ring: multipole fluxes and the logarithmic divergence*, arXiv:[2610.12082](https://arxiv.org/abs/2610.12082) [gr-qc], submitted 08 Oct 2026.

> 💡 A massless particle circling a black hole on its unstable photon orbit radiates gravitational waves whose power per multipole falls only as one over the multipole number, so the total power diverges logarithmically; this paper derives the coefficient in closed form for any black-hole spin and finds a factor-of-four error in a classic 1973 formula.

## 🔍 Executive Summary

The paper treats a photon on the circular light ring of Schwarzschild and Kerr as a null point source for the Zerilli/Regge-Wheeler and Teukolsky equations and solves the large-l problem by matched asymptotics around the top of the potential barrier (parabolic-cylinder/Weber functions). It shows that the flux per multipole tends to g(a) kappa E^2/(M^2 l) both at infinity and at the horizon, with kappa = 0.063653 written as a rapidly converging sum over |m| = l - j, and a closed-form spin factor g = 27M^2(r0-M)/[r0^2(r0+3M)]. It attributes the slow 1/l falloff to two things: the source sits within a few damping widths of the eikonal quasinormal modes for every l (using an identity, vertical epicyclic frequency equals Lyapunov exponent, for all Kerr equatorial light rings), and the leading energy-density and pressure terms of the source cancel exactly because the momentum is null. Results are checked against direct numerical solutions up to l = 12800 (Schwarzschild) and l = 800 (Kerr), with agreement at the 1e-5 level. Along the way it computes the O(l^-1/2) asymmetry between horizon and infinity fluxes, shows how a massive particle's exponential cutoff emerges, and finds that the odd-parity geodesic-synchrotron formula of Breuer, Ruffini, Tiomno and Vishveshwara (1973) is too small by a factor of four.

## 📣 Claimed Contribution

An analytic proof, with the coefficient kappa in closed form, of the logarithmic divergence of the gravitational-wave flux from a photon on the light ring, which was previously established only numerically (Barausse et al. 2021). The paper explicitly lists four new items: (i) the odd-parity 1/l coefficient, four times larger than in the 1973 formulae; (ii) the explicit null limit, which gives kappa in closed form; (iii) the horizon flux for gravitational (rather than scalar) waves, including its O(l^-1/2) asymmetry with the flux to infinity; (iv) the exact normalization in Kerr, including the closed-form spin factor g(a), where the 1974 Chrzanowski-Misner WKB result agrees to 6% partly by accident. It also identifies the mechanism: near-resonance with quasinormal modes plus a cancellation in the source that only happens for null sources.

## ✅ Strengths

- Very strong validation: a fit of the numerical mean flux over 400 <= l <= 12800 gives 0.0318263 against the analytic 0.0318265; individual kappa_j are reproduced to 1e-3 to 2e-5, and the two separate contributions to the O(l^-1/2) horizon/infinity asymmetry are each checked numerically (1.0389 vs 1.0390). In Kerr, Richardson-extrapolated Teukolsky fluxes agree with the analytic values to 1.5e-5 at five spins.
- Gives a clear physical explanation of the 1/l law, correcting the earlier 'relativistic beaming' story: no exponential suppression because the source is near-resonant with the eikonal quasinormal modes at every l, and an l^2 suppression from the null-source cancellation of T_tt against T_phiphi.
- Clean closed forms in Kerr: the light ring parametrized by r0, the amplitude factor N = 16M^2/r0^6, the exact equality of horizon and infinity fluxes at leading order for all spins, and g(a). It also points out the identity Omega_theta = lambda_L, which makes the barrier parameter eta_j = j + 1/2 independent of spin.
- Concretely useful and checkable: it corrects a 1973 odd-parity formula by a factor of 4, demonstrated against exact Teukolsky fluxes for timelike orbits (ratio tends to 4.06/4.05). It also explains why Gundlach et al. (2012) found 42% rather than 50% horizon absorption, since the split approaches one half only logarithmically in the multipole cutoff, and why an earlier fitted cutoff exponent (0.42) differs from pi/6.
- Honest positioning against the 1970s geodesic-synchrotron literature: it says plainly that the even-parity formula, the horizon/infinity equality for scalars and the spin dependence were already present there. A public repository has the Mathematica notebook, a SymPy reproduction and the numerical data.

## ⚠️ Weaknesses

- The headline result is not new. The 1/l law, kappa = 0.064 +/- 0.001 and the equal split between horizon and infinity were already reported numerically by the same author and collaborators in 2021. The even-parity term follows by taking the null limit of the 1973 Breuer-Ruffini-Tiomno-Vishveshwara formula, which the paper itself shows reproduces kappa_0 exactly. The genuinely new analytic content is the factor-4 correction to the odd-parity term (about a 9% change in kappa), the gravitational-wave horizon flux with its l^-1/2 correction, and the exact Kerr normalization.
- The abstract presents the closed-form spin factor g(a) as a result 'we obtain'. Section 4, however, concedes that the null limit of Chrzanowski and Misner (1974), Eq. (4.28), has exactly the same spin dependence. Only the overall constant (6% off there) is new.
- The 'proof' is a matched-asymptotic (WKB/parabolic-cylinder) calculation, not a rigorous estimate. The O(l^-1/2) and O(l^-1) remainders are controlled by numerics, not bounds. For Kerr, the l^-1/2 horizon/infinity asymmetry is only computed numerically.
- The factor-of-four discrepancy with the 1973 odd-parity formula is not traced to a specific step in the original derivation. It is inferred from internal consistency and numerics (convincing, but stated as such).
- The near-extremal prograde regime is not really covered: as the barrier flattens, the asymptotic regime moves out to l >> 800 and no Kerr numerics were run at |a| = 0.99. The statement that g vanishes as a -> M is an order-of-limits result whose practical meaning is unclear.
- Limited physical stakes. A photon on the light ring is a toy problem, and the paper's own EHT estimate gives a fractional energy loss of about 1e-77 per orbit. The suggested applications (speeding up mode sums near the light ring, ultrarelativistic collisions, quadratic quasinormal modes, stable light rings in horizonless objects) are mentioned but not worked out.

## 🤔 Skeptic's Cross-Examination

This is a careful re-derivation of 1970s WKB results in the massless limit, applied to a problem whose answer (1/l, kappa ~ 0.064, equal split) the same author already had numerically. The only result that changes a number anyone used is the factor 4 in the odd-parity term, which shifts kappa by 9%. Since the photon-on-the-light-ring flux has essentially no astrophysical consequence, the value lies in pedagogy and in a correction to an old formula, not in new physics. The rebuttal is that the agreement with numerics to 1e-5 out to l = 12800 makes the corrected coefficients authoritative. The resonance-plus-cancellation explanation is also a real conceptual clarification, and the l^-1/2 corrections are practically useful for extrapolating slowly converging mode sums near the light ring.

## 🆕 Novelty in Context

The paper's self-positioning is mostly honest, but the abstract oversells it slightly. The closest prior work is (a) Barausse, Berti, Cardoso, Hughes and Khanna 2021 (arXiv:2106.09721, PRD 104, 064031), which found numerically up to l ~ 400 the same 1/l law, kappa ~ 0.064 and the equal horizon/infinity split; and (b) the 1972-75 geodesic-synchrotron literature (Breuer-Ruffini-Tiomno-Vishveshwara 1973, Breuer-Chrzanowski-Hughes-Misner 1973, Hughes 1973, Chrzanowski-Misner 1974). That literature already used the barrier-top quadratic approximation, had the even-parity flux in closed form, and had the omega^-1 spectrum up to a cutoff proportional to gamma^2, which implies the divergence in the massless limit at fixed energy. This paper takes that limit explicitly, and its own Section 5 shows that the 1973 even formula gives exactly kappa_0 in that limit. Section 4 shows that the Chrzanowski-Misner 1974 null limit already has exactly the g(a) spin dependence. So 'analytic proof of the divergence' and 'closed form for g(a)' are really 'explicit null limit of known WKB formulas, with corrected normalization'. That is a smaller claim than the abstract suggests. The corrections themselves are real and verified: the factor 4 in the odd-parity coefficient, the overall Kerr constant, and the gravitational-wave horizon flux with its l^-1/2 asymmetry. They also resolve two numerical puzzles in the literature: the 42% absorbed fraction of Gundlach-Akcay-Barack-Nagar 2012 (arXiv:1207.5167) and the fitted cutoff exponent of the 2021 paper. My own INSPIRE/ADS searches turned up no independent analytic treatment of the null-source light-ring flux after the 1970s; the citation search for the 2021 paper returned corrupted results, so very recent related work may have been missed. The identity Omega_theta = lambda_L for Kerr equatorial light rings is presented as a derived fact. It probably sits implicitly in the eikonal quasinormal-mode literature (Cardoso et al. 2009; Yang et al. 2012), and I did not verify whether it is stated there.

## 🎯 Relevance to Your Research

Moderately relevant for a black-hole-perturbation-theory and self-force reader. The paper is a clean, worked example of eikonal/barrier-top matched asymptotics for Teukolsky with a point source in Kerr, and it gives closed-form large-l tails (including l^-1/2 corrections) for mode sums near the light ring. That matters for anyone computing fluxes or self-force for highly relativistic or near-light-ring orbits, or plunges and scattering near the critical impact parameter. The exact Kerr light-ring closed forms and the identity Omega_theta = lambda_L are handy. It has no direct bearing on the EMRI inspiral regime, which stays far from the light ring, or on LISA waveform modeling.

📖 **Where to start:** Sec. 1 (last two paragraphs list exactly what is claimed as new); Sec. 3.3 (the large-l flux formula, kappa_j, and the l^-1/2 horizon/infinity asymmetry and the 42% explanation); Sec. 4 (Kerr: Omega_theta = lambda_L, amplitude factor N, closed-form g(a), and the comparison with Chrzanowski-Misner); Sec. 5 (the factor-4 odd-parity correction); Sec. 6.1 (massive particles and the origin of the exponential cutoff). Skip Sec. 2 unless you need the source conventions.

## Scores

- 🔬 **Quality:** 7.5/10
- 🎯 **Relevance:** 5.5/10
- 🌠 **Reading priority:** Should-Read (weighted score 5/10)

## 🚧 Caveats

- The 1/l law and kappa of about 0.064 were already known numerically (Barausse et al. 2021). What is new is the closed form and the corrections.
- The spin dependence g(a) already appears in the null limit of Chrzanowski and Misner (1974). Only the overall constant is new.
- This is a matched-asymptotics derivation backed by high-precision numerics, not a rigorous proof.
- Near-extremal prograde spins are not validated numerically: there the asymptotic regime sets in only well beyond l = 800.
- A toy problem with negligible astrophysical consequences, as the paper itself says (fractional energy loss of about 1e-77 per orbit for EHT photons).
- The author states that an AI assistant was used for calculations, code and drafting, with all results verified by the author. Companion code and data are public.

---

🔗 [Back to the weekly digest](../2026-10-13)
