# 🌌 Dynamics of Binary System around a Supermassive Black Hole: Binary Scattering and Eccentric vZLK Oscillations

**arxiv:** [2605.22525](https://arxiv.org/abs/2605.22525)
**Authors:** Kei-ichi Maeda, Hirotada Okawa
**Categories:** gr-qc, astro-ph.GA, astro-ph.HE

## TL;DR
Maeda & Okawa stitch together two regimes of a stellar-mass binary moving on an equatorial Kerr geodesic around a $10^{8}\,M_\odot$ SMBH: (i) single-passage scattering on parabolic/hyperbolic outer orbits, and (ii) the von Zeipel–Lidov–Kozai (vZLK) cycle on bound eccentric outer orbits. They classify scattering into four empirical "A/T/C/D" regimes (adiabatic, tidally-affected, chaotic, disruptive) parametrised by the binary semi-major axis $\mathfrak{a}_0$, and identify a new "scattering-type vZLK" regime in which the eccentricity evolves in step-like jumps at each periapsis passage, with $\Theta = \sqrt{1-e^{2}}\cos I$ conserved only in the mean. Useful catalogue, but heavily numerical and limited to equatorial geodesics, where the Kerr Riemann tensor degenerates to Schwarzschild — so Kerr-specific tidal physics is essentially absent.

## Summary
The motion is treated in a Fermi-normal/Fermi–Walker frame attached to the COM Kerr geodesic, with the binary governed by Newtonian gravity plus the leading tidal term $-\tfrac12\mu \bar{\mathcal R}_{\hat 0\hat k\hat 0\hat\ell}\,\mathsf r^{\hat k}\mathsf r^{\hat\ell}$ and a 0.5PN $R_{\hat 0\hat k\hat j\hat\ell}\dot{\mathsf r}^{\hat j}\mathsf r^{\hat k}\mathsf r^{\hat\ell}$ correction. Validity is set by $\ell_{\rm binary}\ll \ell_{\bar{\mathcal R}}\sim \mathfrak r_0(\mathfrak r_0/M)^{1/4}$, plus the Hills/Mardling stability $\ell_{\rm binary}\ll (m_{12}/M)^{1/3}\mathfrak r_0$.
- **Scattering** ($m_{1,2}=10\,M_\odot,M=10^{8}\,M_\odot,\mathfrak r_p=10M$): A at $\mathfrak a_0\lesssim 0.01M$, T at $\sim0.015$–$0.02M$, C up to $\mathfrak a_{\rm cr}\approx 0.099M$, D beyond. The Hills radius is $\mathfrak a_H\approx 0.0585M$; crucially $\mathfrak a_{\rm cr}>\mathfrak a_H$, i.e. some "super-Hills" binaries survive thanks to favourable $\omega_0$. Kerr spin enhances eccentricity excitation for prograde, suppresses it for retrograde; effect washes out for $e_0=0.5$.
- **Bound vZLK**: For eccentric outer orbits ($e_{\rm out}\in\{0.5,0.9\}$, $\mathfrak a_{\rm out}=10$–$50M$) the standard secular vZLK cycle is replaced by stepwise jumps at each periapsis (Fig. 14b, 15b). $\Theta$ deviates by up to $\sim10\%$ per passage but its mean is conserved. For softer binaries the cycle-to-cycle profile becomes irregular ("chaotic scattering vZLK"). Kerr rotation lengthens $P_{\rm vZLK}$ but does not change the qualitative picture — the authors explicitly note this is *because the equatorial Kerr Riemann tensor coincides with the Schwarzschild one*.

## Strengths
- Honest, transparent statement of validity conditions and the equatorial-Kerr Riemann degeneracy (Sec. II.5 and Summary).
- Useful unification of single-passage scattering and bound vZLK as two limits of "periapsis-driven tidal kicks" — the framing as a sequence of impulsive scatterings (Fig. 14b/15b) is pedagogically clean and quantitatively sharp.
- Identification of an empirical $\mathfrak a_{\rm cr}\approx 1.7\,\mathfrak a_H$ above the naive Hills criterion is a concrete, testable refinement.
- Uses Mino time and full analytic Kerr geodesics from Appendix A — cleanly done.

## Weaknesses / Skeptic's Attack
- **Kerr in name only.** Restriction to equatorial COM orbits means $\bar{\mathcal R}_{\hat 0\hat k\hat 0\hat\ell}$ on the COM worldline is identical to Schwarzschild; spin enters *only* through the COM geodesic and the 0.5PN $R_{0kj\ell}$ piece (which vanishes for equal masses, their nominal case $m_1=m_2$). So all "Kerr-vs-Schwarzschild" differences in Figs. 6, 20–22 are pure frame-dragging of the COM, not new tidal couplings — exactly what one would get by replacing Schwarzschild with a Newtonian Kerr COM trajectory. No new analytic Lidov-Kozai-in-Kerr insight.
- **"Four regimes" is phenomenology, not theory.** The A/T/C/D classification is read off from $\omega_0$-scans at four values of $\mathfrak a_0$; no analytic predictor of the A–T or T–C boundary is given. Boundaries are defined by a 5% deviation cut, and the C–D transition acknowledges possible fine-tuned survivors above $\mathfrak a_{\rm cr}$. This is qualitatively the same picture as Hills (1988)/Sari-Kobayashi-Rossi binary tidal disruption, Antognini-Perets single-flyby kicks, and Hayashi-Trani-Suto eccentric vZLK stability — none cited in the regime-discovery context, only as priors.
- **No dissipation.** No GW radiation reaction, no post-Newtonian inspiral feedback inside the binary. The chaos discussion is therefore purely conservative — relevant for orbit kicks per passage but not for actually predicting merger outcomes.
- **Validity in the soft regime.** In the C/D regimes $\mathfrak a_0$ approaches $\mathfrak a_H$, where the tidal expansion in Fermi coordinates becomes marginal. The truncation at $R \mathsf r\mathsf r$ + $R\mathsf r\mathsf r\dot{\mathsf r}$ is not stress-tested against a higher-order expansion or against geodesic-deviation control over many crossings.
- **No quantitative GW or LISA hook.** The summary mentions "implications for gravitational-wave astronomy" but no waveforms, no SNR, no b-EMRI rate, and the proposed follow-up (quadrupole formula for $\mathfrak r>10M$) is only flagged as "in progress."

## Relevance to Vojtěch's Research
Moderate. The b-EMRI/BBH-around-SMBH dynamical channel and the local-frame tidal description are squarely in Vojtěch's territory (three-body in Kerr, EMRI formation via dynamical capture, tidal effects). The step-like vZLK is a genuine reminder that the secular Lidov-Kozai approximation breaks down for eccentric outer orbits near the SMBH and should be replaced by an impulse-sum picture — useful framing. However, the absence of (a) genuine Kerr-tidal effects beyond the equator and (b) GW emission means the paper does not directly advance Vojtěch's interests in Kerr three-body or tidal resonance physics; it is upstream of, rather than within, the LISA EMRI observability problem.

## Quality Score
5.5 / 10

## Relevance Score
6 / 10

## Verdict
Worth-Skimming
