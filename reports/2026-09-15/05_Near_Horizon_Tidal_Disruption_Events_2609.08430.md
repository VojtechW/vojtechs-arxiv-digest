# 🍴 Near-Horizon Tidal Disruption Events

🔦 **Worth-Skimming** · 🔬 Quality 6/10 · 🎯 Relevance 5/10

📎 **Citation:** Yang Yang, Xian Chen, *Near-Horizon Tidal Disruption Events*, arXiv:[2609.08430](https://arxiv.org/abs/2609.08430) [astro-ph.HE, gr-qc], submitted 08 Sep 2026.

> 💡 A semi-analytic calculation shows that when a star is torn apart just outside the horizon of a very massive, rapidly spinning black hole, most of the stellar debris is swallowed at once or thrown away, so the resulting flare is faster and dimmer than standard theory predicts.

## 🔍 Executive Summary

The authors study tidal disruptions in the regime where the tidal radius, the pericentre and the gravitational radius are all comparable, which requires black holes of about 10^8-10^9 solar masses spinning near extremally. Using Fermi normal coordinates along the stellar centre-of-mass geodesic, they map the finite-size spread of the debris onto the equatorial Kerr energy-angular momentum plane, where it forms an ellipse whose intersections with the separatrix (plunge boundary) and with the E = c^2 escape line determine analytically how much debris is promptly lost. For nearly parabolic orbits at the marginally bound orbit they find 90-95% of the debris is lost to plunge or escape, while bound centre-of-mass orbits on the innermost-stable-bound-orbit branch retain far more and give peak fallback rates about 10^3 times higher with correspondingly shorter decay times. They combine the short timescale with the plunge-induced mass deficit to fit the light curve of ASASSN-15lh, and propose a peak-rate versus decay-time plane as a diagnostic for other high-mass tidal disruption candidates.

## 📣 Claimed Contribution

Identification and naming of a distinct class of 'near-horizon TDEs' (r_t ~ r_p ~ r_g around M > 10^8 solar-mass, near-extremal black holes); a framework mapping the debris energy-angular momentum distribution onto the Kerr orbital classification, yielding analytic boundaries for complete disruption, partial mass loss and total mass loss; quantification of a 'plunge-induced mass deficit' with no Newtonian counterpart; relativistic fallback rates for bound as well as parabolic stellar orbits; and an explanation of the overluminous, fast-declining transient ASASSN-15lh plus a proposed observational diagnostic for finding massive, rapidly spinning black holes.

## ✅ Strengths

- The central construction is clean and genuinely useful: because the tidal energy and angular momentum offsets are linear in the displacement from the centre of mass, the star maps to an ellipse in the (E, L) plane, and the fraction of debris lost to plunge or escape follows from elementary geometry against the Kerr separatrix. This gives analytic boundaries (L_TDE, L_loss, complete-loss) rather than a black-box numerical result.
- The regime is genuinely underexplored: existing relativistic hydrodynamic simulations of main-sequence disruptions sit at 10^6-10^7 solar masses with pericentres above ~4 r_g, and the paper is explicit and accurate about that gap.
- The qualitative result that near-horizon disruptions on parabolic loss-cone orbits lose 90-95% of the debris is a concrete, checkable statement with a real consequence: the most relativistic disruptions should be the dimmest, not the brightest.
- The peak-fallback-rate versus half-decay-time plane (Figure 7) is a falsifiable prediction that can be confronted with samples of high-mass candidates, and the standard Rees/Lodato model is plotted on the same axes for comparison.
- The paper is honest about what it cannot do: circularization, hydrodynamics, inclined orbits and repeated tidal forcing during the whirl phase are all flagged as omitted, and the prior-work attribution for the debris-capture effect (Kobayashi 2004, Kesden 2012, Tejeda 2017, Ryu 2023) is fair rather than inflated.

## ⚠️ Weaknesses

- Methodologically this is Kesden (2012, PRD 86, 064026) re-run in a new corner of parameter space: the same Fermi-normal-coordinate tidal spread, the same 'frozen-in' debris released on geodesics, the same fallback integral. The new ingredients are bound centre-of-mass orbits on the innermost-stable-bound-orbit branch, higher black hole masses, and the explicit plunge-boundary bookkeeping. That is an increment, not a new method.
- Restriction to equatorial orbits with vanishing Carter constant is a step backwards in generality relative to Kesden 2012, which already handled inclined orbits. Since stars arrive at the loss cone with roughly isotropic inclinations, and the near-horizon window depends on prograde alignment with a near-extremal spin, the fraction of real disruptions that land in the quoted parameter space is never estimated.
- No event rate anywhere in the paper. The favoured explanation of ASASSN-15lh requires a star on a bound orbit delivered by tidal capture or the Hills mechanism to within roughly a gravitational radius of a 6.3x10^8 solar-mass, a = 0.998 black hole. The claim that such configurations are 'not expected to be rare' is asserted, not calculated.
- The ASASSN-15lh fit has two free dimensionless orbital parameters plus an assumed black hole mass and a maximal spin, tuned against essentially two numbers (peak rate and decay time). The paper itself states that near the plunge boundary the debris distribution becomes nearly one-dimensional and parallel to the separatrix, so the peak rate swings by orders of magnitude under tiny changes in the angular momentum parameter. That sensitivity makes the fit cheap rather than impressive.
- The light-curve comparison assumes luminosity is proportional to fallback rate with a constant efficiency (circularization 0.15 times reprocessing 0.25), the reprocessing factor borrowed from work in the conventional regime. Section 2 argues that the usual single-stream self-intersection circularization picture is inapplicable during the whirl phase and that quantifying it needs hydrodynamics; the light-curve section then proceeds as if the efficiency were known.
- The favoured ASASSN-15lh solution has the angular momentum parameter negative, meaning the stellar centre of mass is itself inside the separatrix and destined to plunge. The whole surviving-debris budget then hinges on where along that plunging trajectory the star is assumed to be instantaneously disrupted, which the frozen-in prescription fixes by hand at the tidal radius.
- The observational sections leave out the features of ASASSN-15lh that made it controversial in the first place (the ultraviolet rebrightening, the late-time plateau, the X-ray behaviour); only the first peak and decline are addressed.

## 🤔 Skeptic's Cross-Examination

The paper's own analysis shows that in the near-horizon limit the debris distribution collapses onto a line nearly parallel to the plunge boundary, so the surviving mass fraction varies by orders of magnitude for infinitesimal changes in the stellar orbit. A model with that property can reproduce almost any peak-rate/decay-time pair, and that is exactly what is done for ASASSN-15lh. Without an event-rate calculation showing that the required fine-tuned orbits are actually populated, and without hydrodynamics validating the instantaneous-disruption-plus-geodesics prescription for a star whirling at the separatrix, the observational claim is a plausibility argument dressed as a fit.

## 🆕 Novelty in Context

The paper coins 'near-horizon TDE' but does not claim to have invented the machinery, and the literature check bears that out. Kesden (arXiv:1207.6401) already built the Fermi-normal-coordinate debris spread in Kerr, computed relativistic fallback rates down to the marginally bound pericentre for both equatorial and inclined orbits, and flagged the frozen-in approximation's limits; the present paper reuses that framework essentially verbatim (its own equations cite Kesden for the energy and angular momentum deviations). Prompt capture of debris by the horizon was likewise noted earlier (Kobayashi 2004, Tejeda 2017, Ryu 2023), and the paper cites those works when introducing the effect, which is honest. The maximum black hole mass for disruption outside the horizon as a function of spin is prior work too (Kesden 2012, Mummery 2024 and, closely related, Huang & Lu 2023 on horizon suppression of disruption rates). That the higher peak rate and faster decline of bound-star disruptions is known from the eccentric-TDE literature (Hayasaki, Park, Cufari et al.), which the paper cites but does not credit prominently when quoting the factor of 10^3. What is new is the combination: restricting the centre of mass to the innermost-stable-bound-orbit branch at masses near the maximum, deriving analytic thresholds for partial and complete debris loss from the geometry of the debris ellipse against the separatrix, and using the resulting mass deficit as an observational diagnostic. A Kerr-black-hole interpretation of ASASSN-15lh was already proposed by Leloudas et al. (2016); this paper adds a specific dynamical mechanism to it rather than proposing the interpretation itself. The correct reading is therefore a solid incremental extension with one new geometric construction, not the opening of a new field.

## 🎯 Relevance to Your Research

The physics content is Kerr geodesic dynamics near the separatrix plus a Fermi-normal-coordinate tidal expansion: the same toolkit used for near-separatrix inspiral orbits and tidal forcing in extreme-mass-ratio problems, here put to astrophysical use. Anyone comfortable with the (E, L) orbital classification and whirl orbits will read Sections 3.1-3.3 quickly and may find the ellipse-versus-separatrix geometry a reusable trick for other finite-size or fragmentation problems near the plunge boundary. The astrophysical payload (fallback light curves, ASASSN-15lh) is peripheral to strong-field gravitational dynamics and is the weaker half of the paper.

📖 **Where to start:** Section 3.1 (equatorial Kerr orbit classification and why the innermost-stable-bound-orbit branch is selected) and Section 3.2 (the Fermi-normal-coordinate mapping of the star onto an ellipse in the energy-angular momentum plane) are the substance; Section 3.3 with Figure 5b gives the surviving-mass diagnostic plane. Skim Section 4 and read Figure 7 for the falsifiable prediction, but treat the ASASSN-15lh numbers in Section 4.1 with caution.

## Scores

- 🔬 **Quality:** 6/10
- 🎯 **Relevance:** 5/10
- 🔦 **Reading priority:** Worth-Skimming (weighted score 4.3/10)

## 🚧 Caveats

- Method is Kesden-style frozen-in debris on Kerr geodesics; the novelty is the regime (bound orbits near the separatrix, r_t ~ r_p ~ r_g) and the explicit plunge-boundary bookkeeping, not a new technique.
- Equatorial orbits only, vanishing Carter constant, no hydrodynamics, no partial disruption, no self-gravity of the debris.
- No event-rate estimate: how often stars actually reach these orbits around near-extremal 10^8-10^9 solar-mass black holes is never computed.
- The ASASSN-15lh explanation is a two-parameter fit in a regime the authors themselves show is extremely sensitive to those parameters; the light curve to fallback rate conversion uses a fixed efficiency that the paper elsewhere argues cannot yet be computed.
- The late-time plateau and ultraviolet rebrightening of ASASSN-15lh are explicitly left unexplained.

---

🔗 [Back to the weekly digest](../2026-09-15)
