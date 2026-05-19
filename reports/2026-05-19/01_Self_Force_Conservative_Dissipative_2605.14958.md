# ⚖️ Conservative and dissipative sectors in a nonlinear scalar model for the gravitational self-force problem

**arXiv:** [2605.14958](https://arxiv.org/abs/2605.14958)
**Authors:** Francisco M. Blanco, Éanna É. Flanagan, Abraham I. Harte
**Categories:** gr-qc, astro-ph.SR
**Collaborator flags:** Éanna Flanagan (T3), Francisco Blanco (T2), Abraham Harte (T2); Adam Pound and Leor Barack acknowledged

## Summary

The authors study how to split the second-order self-force into conservative and dissipative sectors using a nonlinear scalar toy model on a fixed background as a stand-in for the gravitational self-force. They combine Harte's earlier nonlocal field-transformation ("dressing") formulation of self-force with his recent result that broad classes of perturbatively nonlocal-in-time dynamics admit Hamiltonian descriptions. Three candidate prescriptions for the conservative sector are constructed (iterated time-even, time-even, symmetric), Hamiltonians and symplectic forms are written down, and the iterated-time-even definition is shown to be IR-divergent in a cubic toy model. Results are restricted to scattering trajectories because the symmetric Green's-function-squared structure diverges for bound orbits.

## Key Results

- Three candidate "conservative second-order self-force" prescriptions are identified; each admits a Hamiltonian formulation through Harte's nonlocal-to-local framework.
- Demonstration (Appendix C) that the iterated-time-even prescription is IR-divergent in a cubic scalar field model; symmetric and time-even prescriptions remain finite for scattering orbits.
- Argument that, for LISA EMRI waveforms at post-1-adiabatic order, the symmetric prescription is the most efficient because fully-symmetric 3-point functions vanish under phase-space averaging (except on resonances), so only the dissipative sector contributes to the orbit-averaged secular evolution.

## Strengths

- Honest acknowledgement that no unique "preferred" definition exists; framed as a calculational/pragmatic choice rather than dressed up as a discovery.
- Clean technical execution combining two pre-existing frameworks into a single coherent prescription, with explicit Hamiltonians/symplectic forms.
- Useful discussion linking SF ambiguities to current divergent results in PM/PN tail-of-tail computations (Porto-Riva-Yang et al.).

## Weaknesses / Caveats

- Bound orbits are excluded due to IR divergences — exactly the regime relevant to EMRIs and LISA. Framed as "future work" but is the central physical case.
- Existence of the required fully-symmetric singular 3-point function $G_3^S$ is *assumed*, never constructed; the whole edifice rests on this conjecture.
- A scalar toy model on a fixed background — the actual gravitational extension is left for future work.
- Adds a third option without resolving anything; risks proliferating definitions rather than converging.

## Novelty Assessment

The genuinely new content is the assembly of two recent results (Harte's nonlinear self-force formulation and Harte's nonlocal-Hamiltonian theorem) into the first explicit Hamiltonian description for a second-order scalar self-force, plus the systematic enumeration of three candidate conservative-dissipative splits using projection operators on n-point functions. The Appendix C demonstration that the iterated-time-even prescription is IR-divergent is a concrete (if narrow) technical result. The authors are openly self-aware that conservative/dissipative splits beyond first order are well-trodden ground.

What is *not* new: the field-mapping/dressing technology, the basic time-even vs. retarded/advanced split, and the observation that Hamiltonian conservative dynamics is desirable. The paper is more "structural clarification" than breakthrough; useful as a clean rederivation that other workers in PM/SF tail-of-tail debates may cite, but no quantitative observables are produced.

## Relevance to Vojtěch

Hits self-force foundations, Hamiltonian/symplectic structure of EMRI dynamics, action-angle/resonance language (Mino and Hinderer/Flanagan cited for phase-space averaging arguments), and PN-to-SF matching discussions. Vojtěch's 2019 spinning-particle Hamiltonian paper (Witzany-Steinhoff-Lukes-Gerakopoulos) is cited as motivation for Hamiltonian formulations of spin-corrected geodesic motion. The discussion of orbit-averaging vanishing for symmetric 3-point functions (with the footnote "except on resonances") directly touches his resonance interests. The bound-orbit IR obstruction is the operationally relevant limitation for EMRIs.

## Scores

- **Quality:** 7/10
- **Relevance:** 7/10
- **Recommendation:** Should-Read
