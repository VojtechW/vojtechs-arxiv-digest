# 🌊 Orbital Evolution of Asymmetric Binaries Within Accreting Environments

**arXiv:** [2606.18341](https://arxiv.org/abs/2606.18341)
**Authors:** Albert Radulea, Marcelo E. Rubio, Konstantinos Kritos, Andrea Maselli
**Categories:** gr-qc, astro-ph.HE
**Comments:** 14 pages, 7 figures

---

## Summary

Extends the Spieksma-Cannizzaro (2504.08033) Keplerian disk-crossing EMRI model to **bound Kerr geodesics**, integrated analytically between impulsive Ostriker-DF and Bondi-Hoyle-Lyttleton accretion kicks at each disk crossing. The authors report a generic **two-stage evolution**: rapid alignment of the orbital plane with the disk, followed by slower eccentricity damping. They also claim a Kepler-vs-Kerr divergence visible already at a ∼ 10⁶ M (i.e., before the strong-field regime).

## What's genuinely new

- **Kerr-geodesic backbone** in place of the Keplerian one used in Spieksma-Cannizzaro 2504.08033 — incremental but technically clean.
- Quantitative comparison of relativistic vs Keplerian trajectories under repeated disk-crossing dissipation.

## Strengths

- The Kerr-geodesic integration between impulsive disk kicks is technically solid.
- Clean parameter-space scan in (inclination, eccentricity, disk-density profile).

## Weaknesses

- **Disk-crossing physics is Newtonian.** The dynamical friction uses Ostriker's log Λ hardcoded to 3; the accretion uses BHL with a singular v_z denominator that doesn't gracefully handle perpendicular crossings.
- **The two-timescale (alignment → circularization) hierarchy is not new.** Syer-Clarke-Rees 1991 established this decades ago for satellite-disk interactions. The paper frames it as a "finding" rather than a confirmation.
- **The Kepler-vs-Kerr "divergence" at a ∼ 10⁶ M is suspicious.** It is plausibly a phase-decoherence artifact of accumulated periastron precession (which differs between Kepler and Kerr by O(M/a) per orbit) rather than a genuine relativistic disk-coupling effect. The authors do not properly diagnose this.
- **The bibliography misses the entire stellar-transit / disk-crossing lineage.** No citation to Witzany 2017/2019 (stellar transits, secular evolution through tori), Šubr-Karas (debris from disk crossings), Suková-Zajaček (QPEs from disk-crossing stars), Pasham 2024 (GSN 069 disk crossings), Speri (relativistic disk-crossing dynamics), or any of the work establishing how the hydrodynamics and observational phenomenology actually work. This is exactly the literature a paper on EMRI-in-disk should engage with.
- The paper is essentially an upgrade of one model (Spieksma-Cannizzaro) without engaging with the parallel literature on the same problem.

## Relevance to Vojtěch

**Direct overlap with Vojtěch's own line of work on stellar transits through accretion tori and disk-crossing dynamics, and with QPE phenomenology.** The fact that the paper completely misses his lineage is itself worth flagging — both as a literature gap to fix and as a signal of how isolated different communities working on the same problem can be. Reading this critically is more useful than reading it as a primary reference.

## Scores

- **Quality: 5/10**
- **Relevance: 9/10**
- **Verdict: Should-Read (critically)** — useful as a benchmark of what the EMRI-in-disk community thinks they are doing, but the disk-crossing physics is significantly under-developed and the literature engagement is poor.
