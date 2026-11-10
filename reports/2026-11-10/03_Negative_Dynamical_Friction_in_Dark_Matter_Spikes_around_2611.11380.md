# ☁️ Negative Dynamical Friction in Dark Matter Spikes around Rotating Black Holes

🌠 **Should-Read** · 🔬 Quality 5.5/10 · 🎯 Relevance 7/10

📎 **Citation:** Wei Xiong, Peng-Cheng Li, Bin Chen, *Negative Dynamical Friction in Dark Matter Spikes around Rotating Black Holes*, arXiv:[2611.11380](https://arxiv.org/abs/2611.11380) [gr-qc], submitted 08 Nov 2026.

> 💡 Close to a spinning giant black hole, a dense dark matter cloud can push a small orbiting black hole forward and add to its orbital energy, instead of slowing it down as usual.

## 🔍 Executive Summary

The paper extends the relativistic local momentum-exchange model for a small black hole moving through collisionless dark matter (Vicente, Karydas and Bertone 2025) from a non-spinning to a spinning (Kerr) central black hole. The dark matter spike is built by adiabatically growing a Kerr black hole inside a Hernquist (or isochrone) halo, following Ferrer, da Rosa and Will. The paper also solves the linearised Einstein equations spectrally for the spike's own effect on the metric. On stable prograde circular orbits, Kerr capture and binding conditions allow more particles that overtake the companion in azimuth than particles that trail it, and scattering at low relative speed dominates. Above a spin threshold, the net friction therefore adds orbital energy between the innermost stable circular orbit and a few gravitational radii (for spin 0.65, from 3.6M to about 4.9M). For a Milky Way-like halo, mass ratio 1e-5 and a four-year inspiral, the abstract reports about 100 radians of dephasing from friction, plus a redshift correction from the metric response that is comparable in size to, and opposite in sign from, the first-order conservative self-force.

## 📣 Claimed Contribution

The paper shows that dark matter spikes around rotating massive black holes can drive negative dynamical friction, supplying orbital energy to secondaries on stable prograde circular orbits beyond the ISCO once the spin exceeds a model-dependent threshold. It says this is driven by asymmetric Kerr orbital support combined with velocity-dependent scattering, is robust to finite changes in the occupation and to the scattering cutoff, and appears for both cusped and cored progenitor halos. It also claims that the environmental conservative metric response, constructed for Kerr, is comparable to the first-order conservative self-force, so both energy exchange and metric response are needed for precision EMRI modelling.

## ✅ Strengths

- The mechanism is isolated cleanly in the Supplemental Material. Pairing opposite azimuthal velocities shows that the sign comes only from the support difference Delta-chi and from the occupation difference, and a constant-occupation benchmark separates the orbital-support effect from the kernel effect (R_1 = 0.61 net loss vs R_W = 2.22 net gain).
- A simple, rigorous sufficient bound (eta < D_0) shows that the energy gain survives pointwise occupation perturbations of up to about 38% at r=4M and 17% at r=4.5M, so the result does not hinge on a fine-tuned distribution function.
- The sign is checked against the scattering cutoff (b_max varied from half to twice the Hill-type value) and against quadrature refinement, with quoted error estimates well below the margins.
- The paper splits the friction into its scattering and accretion parts: scattering supplies the energy and accretion removes it, and scattering wins by a factor of about 42 for the Hernquist spike. This is a useful physical diagnostic.
- As far as the literature check shows, this is the first Kerr-background implementation of the Vicente-Karydas-Bertone fully relativistic collisionless-environment formalism. It also includes a spectral solution for the stationary metric response of the spike.

## ⚠️ Weaknesses

- The main letter text could not be retrieved with the available tools. Only the End Matter and Supplemental Material were read. The headline numbers (about 100 radians of dephasing, the redshift correction versus first-order conservative self-force, the spin threshold) could not be checked against the actual inspiral and waveform calculation. The quality assessment rests on the mechanism sections.
- Energy gain is confined to a narrow radial window close to the ISCO (3.6M to about 4.9M at spin 0.65 for the constant-occupation benchmark). Most of a four-year inspiral is spent outside it. The abstract's 100-radian figure is for the total friction contribution, which is probably dominated by ordinary positive friction at larger radii, so the headline 'negative friction' may contribute only a small part of the dephasing.
- The physics is less surprising than the title suggests. A body moving more slowly than the local population that overtakes it is known to gain energy from friction; this is standard in rotating stellar systems and gas flows, and Gruzinov, Levin and Matzner (2019) already use the term 'negative dynamical friction' for gas. What is new is that the Kerr capture and binding conditions produce such a population around a circular orbiter. This is a narrower contribution than a new type of friction.
- The interaction kernel uses Schwarzschild cross sections for the companion in its local frame with a hand-chosen maximum impact parameter. This local, Chandrasekhar-like prescription ignores the global wake and resonant response of the spike. Near the ISCO, where tidal and Kerr frame-dragging scales are not well separated from the interaction scale, that is exactly where the approximation is weakest.
- The spike is the idealised adiabatic-growth (Gondolo-Silk-type) profile. Its survival in a Milky Way-like nucleus is doubtful, and the companion's feedback on the spike (phase-space depletion) is not included in the parts read. The absolute dephasing is therefore close to an optimistic upper bound.
- The LaTeX source contains comments stating that the supplemental numerical diagnostics were 'independently recomputed' without running the authors' production code, plus leftover red-text editorial macros. Together these suggest the supplemental numbers and the main-text pipeline may not come from the same code.

## 🤔 Skeptic's Cross-Examination

The sign reversal lives in a radial band of about one gravitational radius next to the ISCO. It is computed with a local, Schwarzschild-kernel friction prescription that is least reliable there, using a spike density profile that probably does not survive in real nuclei and ignoring how the companion depletes the spike. Integrated over a realistic four-year inspiral, the negative-friction part is probably a small correction to an already model-dependent total dephasing, so the headline is a qualitative curiosity rather than a waveform-level effect.

## 🆕 Novelty in Context

The paper builds directly on Vicente, Karydas and Bertone (arXiv:2505.09715, PRL 2025), which introduced the fully relativistic local momentum-exchange formalism for collisionless environments on Schwarzschild. It also builds on Ferrer, da Rosa and Will (2017) for adiabatically grown Kerr spikes. Searches of InspireHEP and ADS found no prior Kerr implementation of the friction formalism. Follow-ups by the same group (2510.13604 on companion spin evolution, 2610.37638) stay with non-spinning hosts, so the Kerr extension and the near-ISCO sign reversal appear new. The phrase 'negative dynamical friction' is not new: Gruzinov, Levin and Matzner (MNRAS 2020) used it for compact objects in dense gas. More generally, acceleration by an overtaking population is textbook physics in rotating systems. The honest claim is 'the Kerr capture and binding structure produces an overtaking population large enough to reverse the sign of collisionless friction near the ISCO'. That is a solid but incremental result, not a new kind of friction. The self-force comparison could not be checked against the main text.

## 🎯 Relevance to Your Research

This is directly relevant to environmental effects in extreme-mass-ratio inspirals and to how environmental corrections compare in size with self-force corrections. It is the first Kerr extension of the fully relativistic collisionless friction model now being built into FastEMRIWaveforms-style pipelines. The claim that the metric-response redshift correction rivals the first-order conservative self-force is the part most worth checking for anyone doing self-force or waveform work. Treat the negative-friction sign as a near-ISCO detail, not as something that changes the inspiral.

📖 **Where to start:** Supplemental Material Sec. I (Energy-supply mechanism), which has the paired-velocity argument and the R_1 vs R_W benchmark, and Sec. II (Robustness under occupation perturbations), which has the D_0 margin and the radial extent table. In the main letter, read the inspiral and dephasing figure and the paragraph comparing the redshift correction with the first-order conservative self-force. End Matter C covers the spectral metric-response construction and its boundary conditions (fixed horizon angular velocity).

## Scores

- 🔬 **Quality:** 5.5/10
- 🎯 **Relevance:** 7/10
- 🌠 **Reading priority:** Should-Read (weighted score 5.2/10)

## 🚧 Caveats

- Negative friction only operates in a thin band just outside the innermost stable circular orbit (about 3.6M to 4.9M at spin 0.65), and only above a spin threshold.
- The 100-radian dephasing is for the total friction, which is most likely dominated by ordinary drag, and assumes an idealised adiabatically grown dark matter spike.
- The friction is a local Chandrasekhar-style prescription using Schwarzschild cross sections and a chosen impact-parameter cutoff. It does not include a self-consistent wake or feedback from the companion on the spike.
- The concept of 'negative dynamical friction' predates this paper; what is new is how it arises from Kerr orbital support.
- The source comments say the supplemental diagnostics were recomputed outside the authors' production code.

---

🔗 [Back to the weekly digest](../2026-11-10)
