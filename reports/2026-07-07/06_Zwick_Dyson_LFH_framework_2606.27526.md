# 🌌 Dynamics of Relativistic Binaries in Structured and Stochastic Environments: A Lagrange-Fourier-Hansen Framework

**Authors:** Lorenz Zwick, **Conor Dyson** (T2), Brian C. Seymour, János Takátsy, Johan Samsing
**arXiv:** [2606.27526](https://arxiv.org/abs/2606.27526) · gr-qc, astro-ph.GA, astro-ph.HE
**Submitted:** 25 Jun 2026

## Summary
A framework paper claiming a unified formalism (Lagrange planetary equations + Fourier decomposition of external forces + Hansen coefficients) for treating non-vacuum perturbations of GW-driven binaries. Reduces smooth, structured, or stochastic environments to a "resonant spectral projection" on a rolling averaging window, yielding coupled ODEs for orbital elements that capture epi-cyclic, apsidal, and nodal resonances alongside radiation reaction. Two applications: compact binary in a variable tidal field, and EMRI in an accretion disk.

## Genuinely New?
Skeptical. The direct precursor 2506.09140 (same lead team) already implements exactly this construction in Newtonian osculating elements with a Fourier expansion of the perturbing force and orbit-averaged secular ODEs — including "epi-cyclic resonances" as commensurabilities of external Fourier modes with equation-of-center harmonics. That paper does not name Hansen coefficients nor cite the century-old astrodynamics literature (Brouwer, Kaula, Wisdom) or the Kerr action-angle EMRI resonance literature (Hinderer–Flanagan, Fujita–Hikida, Flanagan–Hughes–Ruangsri). The present paper's real novelty appears to be: (i) branding — explicitly identifying the equation-of-center expansion coefficients as Hansen coefficients (standard since Hansen 1855); (ii) generalizing to structured/stochastic perturbations with a rolling averaging window; (iii) apparently adding apsidal/nodal resonances (3D + relativistic precession, hence Dyson/Seymour). Whether items (ii)–(iii) are substantive or cosmetic requires close reading of the actual text; the abstract's framing suggests reformulation rather than new physics.

## Strengths
- Unifying a scattered set of environmental-effect dephasing prescriptions used by the Zwick/Samsing program (2505.09513, 2506.09140, 2508.17348, 2511.04540) into one coherent framework has real value for the LISA/eccentric-binary community.
- Adding Dyson (analytic Kerr geodesics, spiral density waves in Kerr) and Seymour (GR inspiral tests) plausibly injects proper relativistic content that was absent from the strictly Newtonian precursor.
- The "rolling averaging window" for stochastic perturbations is a nontrivial extension of orbit averaging.

## Weaknesses
- "Lagrange–Fourier–Hansen" is a rebranding of standard secular perturbation theory used in celestial mechanics for ~170 years. Naming it a "framework" risks overclaiming.
- The precursor's citation hygiene omits the entire astrodynamics genealogy and the Kerr AA/self-force literature — if this pattern persists, positioning against prior art will be weak.
- Given the precursor is fully Newtonian and explicitly punts on PN precession and mixing ("only at 5PN or 6PN"), any "relativistic" content here is likely bolted-on osculating-element approximations to Kerr rather than a genuinely covariant/AA treatment.

**Caveat:** the full-text PDF could not be retrieved during evaluation (network restrictions on newly-processed arxiv). This assessment leans on the abstract, the precursor 2506.09140, and Dyson/Seymour's prior work. Recommend a full-text pass on Sec. II and the intro's positioning paragraph.

## Relevance to Vojtěch
Moderate–high. Directly overlaps his orbital-resonance and environmental-effects-on-EMRIs interests, and Dyson is a T2 collaborator. But methodologically it is orthogonal to his AA/Hamilton-Jacobi program: this is 3D osculating-element astrodynamics for stellar-mass binaries in disks/tidal fields, not covariant Kerr AA with self-force. Worth reading to check whether the "apsidal/nodal resonance" treatment overlaps or conflicts with Flanagan–Hughes–Ruangsri-style Kerr resonances.

## Scores
- **Quality: 6/10** (tentative — pending full-text confirmation of claimed novelty).
- **Relevance: 6/10.**
- **Verdict: Worth-Skimming.** Read Sec. II (framework construction) and the novelty paragraph carefully; the two example applications are almost certainly demonstrations rather than new physical results.

## Collaborator flags
Conor Dyson (T2).
