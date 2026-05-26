# 📜 Convergence of post-Newtonian for quasi-circular non-precessing comparable mass ratios BBHs

**arxiv:** [2605.20562](https://arxiv.org/abs/2605.20562)
**Authors:** Dongze Sun, Béatrice Bonga, Leo C. Stein, Guido Da Re
**Categories:** gr-qc
**Collaborator flag:** 🌟 Leo Stein (Tier 1), Béatrice Bonga (Tier 2)

## TL;DR
The authors benchmark the convergence of the post-Newtonian (PN) energy-flux series against a long, high-accuracy SXS Cauchy-characteristic-evolution (CCE) waveform for a q = 3 non-spinning quasi-circular BBH (SXS:BBH:2265, 60+ orbits). Working at scri after fixing both NR and PN into a common BMS frame and fitting only (M, q), they find that PN improvement persists through (incomplete) 6PN for orbital velocities v ≲ 0.45, but non-monotonically — with local extrema near 2.5PN and 4PN — which directly refutes the Yunes–Berti prescription of stopping at the first local minimum. Near v ~ 0.47 (ICO) all PN orders cluster: PN loses convergence.

## Summary
The paper is essentially the comparable-mass analogue of the Sago–Fujita–Nakano / Yunes–Berti PN-vs-perturbation-theory comparisons, but now using a full NR simulation as the "exact" answer. Methodology:

- **NR side:** SpEC Cauchy evolution + SpECTRE CCE for waveform extraction at ℐ⁺, providing strain, Bondi news, and Weyl scalars directly without extrapolation. Energy flux computed as ∮r²/(16π)|ḣ|² dΩ via the `scri` package.
- **PN side:** TaylorT1 with non-spinning flux complete through 4.5PN, supplemented by EMRI-limit terms (Fujita) up to 6PN; horizon flux to 4PN (Alvi). Strain modes complete to 3.5PN (4PN for the (2,2) mode), m=0 modes to 3PN.
- **Gauge-consistent comparison:** They use Mitman/Stein/Bonga-style BMS frame fixing: a boost to map COM charge, a supertranslation to map the Moreschi supermomentum onto the analytically-known PN supermomentum. They fit the PN intrinsic parameters (M, q) plus the usual gauge offsets by minimizing the fractional L² mismatch over a 5-orbit early-inspiral window.
- **Key results:**
  1. For v ≲ 0.45, ΔĖ decreases roughly as v^(10+2N+1), confirming asymptotic behavior at the expected order; 6PN gives the best agreement.
  2. The decrease in ΔĖ vs PN order is **non-monotonic**, with bumps at 2.5PN and 4PN. This is the headline negative result against Yunes & Berti's "first local minimum = optimal truncation" recipe.
  3. At v ≈ 0.5 (ICO), all PN orders pile up — clean signal of asymptotic divergence near merger.
  4. At v ≲ 0.32 (~5 orbits before merger), the 6PN error already drops below NR truncation error. Extrapolating, at v = 0.2 the 6PN flux is accurate at ~10⁻¹⁵, i.e. at double precision — meaning further PN improvement would require NR codes that don't exist.
  5. Practical implication: pushing the non-spinning PN flux beyond 6PN buys nothing; the win is in spinning/eccentric extensions.
- **Robustness checks:** Variations of the 5-orbit matching window position and width (3 vs 5 orbits) give consistent results. A 15-orbit window biases the comparison because v drifts non-negligibly during matching — a clean physical explanation.

## Strengths
- The methodology is technically clean: doing the BMS frame fixing properly (boost + supertranslation via Moreschi supermomentum) is *the* right way to make PN/NR flux comparisons gauge-invariant, and they explicitly fit only physical (M, q), letting gauge degrees of freedom soak up the rest.
- Use of CCE rather than extrapolation eliminates one of the main concerns of older Boyle et al. (2007) PN–NR comparisons.
- The fitted power-law slopes log ΔĖ vs log v match the analytic v^(2N+11) prediction quite well, providing a non-trivial consistency check that they really are probing PN truncation error and not gauge artifacts.
- The Yunes–Berti "first local minimum" rebuttal is well-supported and useful: the 2.5PN/4PN extrema are visible in their Fig. 2 and clearly demonstrate that the simple monotonic-approach-to-optimum picture is wrong.
- Honest about limitations: they note the strain is only 4PN-complete so >4PN flux comparisons are slightly inconsistent (using Trestini-style arguments that strain truncation has subdominant impact).
- The "you'd need 10⁻¹⁵ NR to test 6PN at v = 0.2" observation is striking and has clear practical consequence for waveform-model strategy.

## Weaknesses / Skeptic's Attack
- **Single configuration.** Everything rests on one SXS run, q = 3, non-spinning, non-precessing. Calling this "the convergence of PN for comparable-mass BBHs" is overselling — it's the convergence for *this one orbit*. Equal-mass behavior could differ in detail (the asymptotic-series coefficients carry ν-dependent symmetric structure), and the conclusion that 6PN is "good enough" might be q-dependent. The title is broader than the analysis.
- **6PN is incomplete and EMR-derived.** The headline 6PN curve uses only the v^(2N) terms known in the test-particle limit; the comparable-mass corrections at 5, 5.5, 6PN are missing. The footnote acknowledges that incompleteness could reverse trends. The "extrapolation" to predict 10⁻¹⁵ accuracy at v = 0.2 is a stretch — the fitted slope is much larger than the expected 2N+11 = 23, which the authors themselves note "suggests that the missing higher order PN terms become dominant." If unknown terms dominate the residual in the fit region, the extrapolation to v = 0.2 is not bounding the *true* 6PN error, it is bounding "incomplete 6PN as the authors define it." This caveat is admitted but then largely waved through in the discussion.
- **Strain truncated at 4PN.** Frame-fixing and parameter-fitting depend on the strain, which is only complete to 4PN. They cite [32] (Trestini) to argue strain inaccuracies are subdominant, but this is hand-waved rather than quantified directly for their setup.
- **2.5PN/4PN non-monotonicity vs. Yunes–Berti.** While the result is genuine, it is a fairly modest update to existing literature. EMRI-limit work (Sago–Fujita–Nakano, and beyond) already showed PN coefficients grow oscillatorily, so non-monotonic decrease of residuals at comparable mass is plausible rather than surprising. The "first local minimum" recipe was always crude — slaying it is a small giant.
- **Parameter fit overfitting concern.** They fit (M, q) plus a boost, time shift, rotation, spatial translation, and 77 supertranslation modes. They argue these are "mostly gauge", but the COM boost in particular can absorb some monopole/dipole flux features. Their counter — that the flux comparison is over a wide v range — is reasonable but does not formally exclude bias. This is the kind of place a future "first-principle parameter mapping" (their own Future Work bullet) would matter.
- **Single eccentricity, no spins.** The title says "BBHs" but the analysis cannot distinguish convergence behavior driven by mass-ratio dependence from convergence driven by spin or eccentricity. The Future Work section honestly admits this.

## Relevance to Vojtěch's Research
Directly relevant. This paper is the natural comparable-mass extension of the EMRI-limit PN convergence studies (Sago, Fujita, Nakano [40]; Yunes & Berti [52]; Simone–Poisson–Will [43]) that Vojtěch has worked alongside. The methodological lessons — gauge-invariant comparison via BMS frame fixing, the (M, q) parameter mapping, the v^(2N+11) error scaling diagnostic — port directly to PN-to-self-force matching projects. The negative result about Yunes–Berti's "first local minimum" criterion is something Vojtěch should know about before quoting that recipe. Stein and Bonga have been pushing the BMS-frame fixing program for a while; this is its first really clean application to a convergence statement. The Future Work direction on first-principle PN-mass vs NR-horizon-mass mapping (citing [45]) is the kind of body-zone-asymptotic-matching work that overlaps Vojtěch's PN-to-Kerr matching interests.

## Quality Score
7.5 / 10

## Relevance Score
8 / 10

## Verdict
Should-Read

## Reading Notes (optional)
- Fig. 1 / Fig. 2 are the key plots. Fig. 2 (ΔĖ vs PN order at fixed v) is where the non-monotonic 2.5PN/4PN structure is visible — worth eyeballing before quoting any "PN converges through Nth order" statement.
- The footnote on tidal-deformability degeneracy with unknown point-mass 5PN terms is a tidy practical point worth filing for NS-BH discussions.
- They explicitly note the distinction between x = (MΩ)^(2/3) and y = (Mω)^(2/3) at 4PN — relevant for anyone doing PN-EMRI matching where conventions matter.
- The 10⁻¹⁵ accuracy claim at v = 0.2 is fragile (uses an extrapolated slope much larger than asymptotic), but the qualitative point — that NR is already the bottleneck — is solid.
- Worth comparing the published 2.5PN and 4PN "bumps" to those seen in EMRI-limit convergence plots (Sago–Fujita–Nakano) to see if they share an origin.
