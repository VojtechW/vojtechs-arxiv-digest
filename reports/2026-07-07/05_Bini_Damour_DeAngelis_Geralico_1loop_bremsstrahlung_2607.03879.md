# 🌊 Radiated Energy Spectrum, Radiated Angular Distribution and Non-linear Memory from the One-loop Gravitational Bremsstrahlung Waveform

**Authors:** Donato Bini, Thibault Damour (T3), Stefano De Angelis, Andrea Geralico
**arXiv:** [2607.03879](https://arxiv.org/abs/2607.03879) · gr-qc · 23 pp
**Submitted:** 4 Jul 2026

## Summary
Building on the one-loop (G³) two-body scattering waveform (Brandhuber et al. 2303.06111; Herderschee–Roiban–Teng 2303.06112; Georgoudis et al. 2303.07006), the authors extract three derived observables at G⁴/G⁵: the spectral radiance dE/(dω dΩ), the frequency spectrum dE/dω, and the angular distribution dE/dΩ, and from the last of these the multipole decomposition of the non-linear memory up to G⁵. Everything is worked in the CoM frame and expanded to fractional 7.5PN (p_∞¹⁵ beyond LO). Ancillary Mathematica files (`spectrum_l_m.m`, `memory_l_m.m`) provide multipole tables up to ℓ ≈ 17.

## Genuinely New?
Modestly. The one-loop waveform itself is *not* new — De Angelis is a co-author on Brandhuber et al. 2023, and Heissenberg 2025 already pushed its PN expansion to 5PN. The extraction of dE/dω and dE/dΩ by squaring the waveform, and the well-known Blanchet–Damour 1989/1992 identity mapping the angular energy distribution to non-linear memory multipoles, are essentially mechanical. The real new content is: (i) pushing the PN expansion of the 1-loop waveform from 5PN → 7.5PN in the CoM frame, and (ii) explicit tables of non-linear memory multipole coefficients at G⁴/G⁵. The authors' framing — "To our knowledge, such a result is new" — is technically correct but understates how derivative the setup is; concurrent Heissenberg–Russo (2511.13835) and Giacomo–De Angelis–Kosower (2511.05412) papers on the same object are cited.

## Strengths
- Legitimate consistency checks: total energy/momentum losses reduce to Herrmann et al. 2104.03957 (G³) and Dlapa et al. 2210.05541 (G⁴); the ν→0 limit reproduces the rest-frame memory of Georgoudis et al. 2506.20733.
- Ancillary files make results usable — the multipole tables are the tangible deliverable.
- Technically clean high-PN expansion of Bessel-K + exponential structures, nontrivial in practice.

## Weaknesses
- The 7.5PN claim is a fractional PM-expansion statement, *not* an independent 7.5PN scattering-mode cross-check — only the LO G³/G⁴ totals are compared to bona fide PN results. So "7.5PN accuracy" is really "PN-expanded 1-loop PM waveform to p_∞¹⁵" and only the low-order slice is externally verified.
- Overlap with Heissenberg–Russo and Giacomo–De Angelis–Kosower is real; competitive pressure with the Parra-Martinez group is explicit in the acknowledgments.
- The paper is bulky (dominated by coefficient tables) and reads as an inevitable follow-up to prior Bini–Damour output (Bini:2026dvn on quadrupolar 3.5PN memory is the direct precursor).

## Relevance to Vojtěch
Directly useful. PN-expanded PM memory multipoles in the CoM frame are exactly the sort of object that feeds into PN-to-Kerr matching cross-checks: they provide analytic velocity-expanded scattering-mode data that can be re-analytically-continued to bound orbits and compared against BHPT/Teukolsky output. The ancillary `memory_l_m.m` file is worth grabbing.

## Scores
- **Quality: 7/10** — solid, competent, well cross-checked at leading PM orders; not a conceptual advance, an extension riding on a waveform other people (partly) computed. Unusually well cross-checked and produces machine-readable output.
- **Relevance: 7/10** — direct value for PN-to-Kerr matching.
- **Verdict: Should-Read.** Read the intro and Section III.1 (checks), then download the ancillary `.m` files. Do *not* invest time reading the coefficient tables in-paper — treat this as a reference table.

## Collaborator flags
Thibault Damour (T3).
