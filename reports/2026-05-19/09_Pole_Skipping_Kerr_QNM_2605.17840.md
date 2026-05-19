# 🔮 Pole Skipping, Avoided Crossing, and Resonant Excitation in Kerr Quasinormal Modes near Algebraically Special Frequencies

**arXiv:** [2605.17840](https://arxiv.org/abs/2605.17840)
**Authors:** Kei-ichiro Kubota, Hayato Motohashi
**Categories:** gr-qc, astro-ph.HE, cond-mat.stat-mech, hep-th
**Collaborator flags:** Motohashi co-authors with Panosso Macedo (T2) on the closely-related update 2512.02110 ("Exceptional Points and Resonance in Black Hole Ringdown")

## Summary

The authors address a long-standing puzzle in Kerr quasinormal mode theory: near the algebraically special frequencies, Kerr QNM trajectories in the complex plane exhibit anomalous behavior — apparent bifurcation, disappearance, and a non-smooth connection to the Schwarzschild limit — that has resisted clean physical interpretation since the work of Maassen van den Brink in the early 2000s. By tracking the poles and zeros of Green-function building blocks across different Riemann sheets, they identify the bifurcation as an avoided crossing accompanied by resonant excitation, and the disappearance as pole skipping caused by cancellation between a QNM pole and a Matsubara-mode zero.

## Key Results

- Identification of an avoided crossing between two Riemann-sheet pole trajectories as the origin of the apparent QNM bifurcation near algebraically special frequencies.
- Demonstration that "disappearing" QNMs are not actually missing but are removed from the physical sheet by exact cancellation against a Matsubara-mode zero — i.e., a pole-skipping mechanism.
- Resonant-excitation accompaniment of the avoided crossing, suggesting that this region of parameter space should produce enhanced QNM amplitudes in ringdown signals (potentially observable).
- Clean unification of disparate observed anomalies under a single Green-function analytic-structure framework.

## Strengths

- The pole-skipping language imported from holography (where it has a clear physical meaning in finite-temperature CFT) is mapped non-trivially onto Kerr ringdown — this is a genuine cross-pollination between hep-th and gr-qc.
- Resolves a specific, well-defined puzzle that has been on the books for ~20 years.
- The avoided-crossing + resonant-excitation prediction is, in principle, observationally relevant for high-SNR ringdown spectroscopy.
- Tracks the underlying analytic structure (Riemann sheets, pole/zero cancellations) rather than just fitting numerical mode trajectories.

## Weaknesses / Caveats

- The 4-page PRL-style format means many calculations are sketched rather than fully exposed; verification requires recomputing the Green-function building blocks.
- The connection between "Matsubara-mode zeros" in this context and the standard finite-temperature Matsubara construction is nontrivial — readers unfamiliar with the holographic pole-skipping literature may find the framework opaque.
- Algebraically special frequencies sit at imaginary values; whether the resonant-excitation enhancement is large enough to actually matter for ringdown spectroscopy is not quantified.
- Co-author Motohashi has a closely-related update (2512.02110) with Panosso Macedo on "exceptional points" in BH ringdown that should be read alongside this paper.

## Novelty Assessment

This is a structural/conceptual contribution rather than a routine QNM-on-exotic-metric paper. The author's preferences explicitly caution against "QNM/greybody/shadow computations on exotic backgrounds" — but this paper is not in that category. It addresses a long-standing analytic-structure puzzle in the Kerr QNM spectrum itself, using techniques (pole skipping, Matsubara modes) that have meaningful physical content in adjacent fields. The "novel" claim — that the QNM disappearance and bifurcation are organized by avoided crossing + pole skipping — is a real structural insight if the analysis holds up.

Compared to Maassen van den Brink's foundational work and the Berti-Cardoso analyses of algebraically special modes, this paper provides a new mechanism rather than a re-derivation. The follow-up with Panosso Macedo (2512.02110, currently a replacement) appears to extend the same framework to exceptional points more broadly.

## Relevance to Vojtěch

Highly relevant to the analytical-structure side of Vojtěch's interests. The algebraically special frequencies, Riemann-sheet analysis, and pole-zero structure of Kerr Green's functions are exactly the kind of "non-trivial integrability and analytical structure in GR" that Vojtěch's preferences explicitly flag as qualifying for the broader-net axis. The resolution of a long-standing puzzle via pole-skipping is a clean structural insight, not an exotic-background QNM exercise. The connection to ringdown spectroscopy adds observational relevance.

## Scores

- **Quality:** 7.5/10
- **Relevance:** 7/10
- **Recommendation:** Should-Read
