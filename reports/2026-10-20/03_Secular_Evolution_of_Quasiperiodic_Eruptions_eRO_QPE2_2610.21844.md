# 💡 Secular Evolution of Quasiperiodic Eruptions: eRO-QPE2

🌠 **Should-Read** · 🔬 Quality 5/10 · 🎯 Relevance 8/10

📎 **Citation:** Zirui Zhang, Cong Zhou, Zhen Pan, *Secular Evolution of Quasiperiodic Eruptions: eRO-QPE2*, arXiv:[2610.21844](https://arxiv.org/abs/2610.21844) [astro-ph.HE], submitted 15 Oct 2026.

> 💡 Four years of X-ray monitoring of the repeating flares from the galaxy nucleus eRO-QPE2 show no hidden faint flares between the bright ones and a slowly shrinking flare period, which the authors read as a small body on a nearly circular orbit hitting a tilting gas disk twice per orbit.

## 🔍 Executive Summary

The authors reanalyse all 11 XMM-Newton observations of eRO-QPE2 (August 2020 to December 2024). They find that the eruption peak count rate stays roughly constant while the quiescent flux falls, with deviations from a linear decline that they attribute to disk precession. Stacking all eruptions, they find no secondary flare between consecutive eruptions, with a 95% upper limit of 0.56% on its counts relative to a normal eruption. Combined with a Roche-lobe argument and published star-disk collision simulations, they use this to argue against the one-eruption-per-orbit interpretation. They then fit the flare start times with their existing Kerr EMRI plus precessing-disk timing model, using an osculating (forced) trajectory with a constant period derivative, fitting epochs 1-4 and 4-11 separately. The results are e < 0.026 and e < 0.033 (95%), an orbital period of about 17.4 ks decreasing at dT_obt/dt of about -1.1e-5, and essentially unconstrained black-hole mass, spin and disk parameters.

## 📣 Claimed Contribution

(1) The first analysis of the full 11-epoch XMM-Newton data set of eRO-QPE2 covering both quiescent and eruption emission, with a constant eruption peak rate and a declining, non-linear quiescent rate. (2) A stacked search for secondary flares giving N_small/N_large < 0.56% (95%), which together with tidal-stability and simulation arguments 'strongly disfavors' one eruption per orbit and makes existing one-eruption interpretations 'ungrounded'. (3) A Bayesian forced-trajectory timing analysis over 4.33 yr giving e < 0.033 and dT_rec/dt of about -5e-6, consistent with an EMRI crossing a precessing disk twice per orbit.

## ✅ Strengths

- The secondary-flare upper limit (0.56% of the normal eruption counts, from stacking all 11 epochs) is a concrete new empirical number that bears directly on the one versus two eruptions per orbit debate for this source.
- Uses the full public XMM baseline (4.33 yr). The timing likelihood marginalises over unknown cycle counts across observing gaps, and an explicit systematic-timing term absorbs flare-shape variability (measured intrinsic scatter of t_peak - t_start is 171 s).
- Section 3 gives a clear analytic catalogue of which mechanisms produce in-phase versus anti-phase odd/even recurrence-time modulation (apsidal precession, disk precession, light-travel geometry, Lense-Thirring coupled to viewing angle, companion black hole), with order-of-magnitude amplitudes. This is useful intuition for anyone fitting QPE timing.
- Section 4.1 gives a simple, explicit validity criterion for when a pure geodesic timing model breaks down because of period decay (span under about 6.5 d for eRO-QPE2 parameters).

## ⚠️ Weaknesses

- Incremental relative to the authors' own recent work. The osculating/forced-trajectory timing machinery and an eRO-QPE2 fit on a subset of these data are in Zhou, Zeng & Pan (2411.18046). The companion note Zhou et al. (2605.29382) already concluded that eRO-QPE2 is 'well described by a near-circular EMRI and a precessing disk'. The genuinely new pieces are the stacked secondary-flare limit and the extension to 11 epochs.
- The 0.56% limit is on 0.2-2 keV counts, but the simulation asymmetries it is compared against (luminosity ratios of about 10-50 at peak, energy ratios E_back/E_for > 3%) are bolometric. A cooler or more obscured backward flare could fall out of the band, so the step from 'no faint flare in counts' to 'two eruptions per orbit' is weaker than the 'leave no room' language suggests.
- The stacking aligns on flare peaks across epochs whose long-short contrast varies from about 650 s to about 100 s. Under the one-eruption hypothesis on an eccentric or precessing orbit, a putative second-crossing flare would not sit at a fixed phase, so the stacked limit depends on an assumed location and shape for the secondary. In the sections read, how robust the limit is to this is not shown.
- The 'large-amplitude oscillation' in the quiescent flux in the abstract is, in the text, 11 points that 'cannot be well fitted by a linear trend', e.g. epoch 3 lies below it. No periodicity is fitted, and the quiescent variation is not quantitatively tied to the disk precession period inferred from timing. Here the precession interpretation is a plausibility argument, not a result.
- The timing fit is split into epochs 1-4 and 4-11 rather than fitted globally. The two dT_obt/dt values (-1.10e-5 versus -0.40e-5 with a broad, oddly signed asymmetric interval) are called 'consistent', but the secular claim effectively rests on comparing two period measurements 3.3 yr apart. Black-hole mass, spin, orbit size and disk parameters are essentially unconstrained.
- The low-eccentricity result is model-dependent: in Fit 1 the early-epoch long-short contrast (about 650 s) is attributed mostly (about 500 s) to light-travel geometry rather than eccentricity. This is a degeneracy the fit is free to exploit with a 14-parameter model on sparse data, and the 95% upper limit on e inherits it.
- In the sections read, there is no direct engagement with the main competing analysis, Arcodia et al. 2026 (2604.09788). That analysis used a denser month-long multi-mission campaign, found |dP/dt| < 2e-6 at 3 sigma and correlated odd/even timing, and favoured one observed eruption per orbit. Those data are not included here, and the 'ungrounded' dismissal of one-eruption interpretations is argued only indirectly.
- Minor inconsistencies: the prior table lists sin(theta_min) as uniform but the table note says cos(theta_min). The Fit 2 period-derivative interval is written in a way that crosses zero despite a prior fixing the sign.

## 🤔 Skeptic's Cross-Examination

The headline exclusion of one eruption per orbit rests on a soft X-ray count ratio compared with bolometric simulation asymmetries for a small set of star-disk setups. A colder or more obscured backward flare, a stripped star, or a compact object with asymmetric ejecta could evade a 0.56% count limit. Meanwhile the two-eruption timing fit, with 14 free parameters, splits the data into two windows and leaves mass, spin and disk parameters unconstrained. So the fit demonstrates that the precessing-disk model can describe the data, not that it is required.

## 🆕 Novelty in Context

The paper presents itself as settling the one versus two eruptions per orbit question for eRO-QPE2 and measuring its secular evolution. The literature check shows the timing framework, including the osculating-trajectory treatment of disk-induced period decay, comes from Zhou, Zeng & Pan (2411.18046). That paper already fitted eRO-QPE2 on a data subset. The group's own note 2605.29382 (May 2026) already concluded that eRO-QPE2 timing is 'well described by a near-circular EMRI and a precessing disk'. Period decrease in eRO-QPE2 was previously reported by Arcodia et al. 2024 (2406.17020) and Pasham et al. 2024 (2411.00289), which the paper acknowledges. The direct opposing analysis, Arcodia et al. 2026 (2604.09788), argues from correlated odd/even timing in a month-long campaign that only one crossing per orbit is observed, and finds no period derivative on that short baseline. The present paper does not address that analysis head-on in the sections read; the 'ungrounded' verdict on one-eruption models is reached through the flare-stacking limit and simulation literature. The honest framing is therefore: an extension of the group's existing eRO-QPE2 fit to the full XMM baseline, plus one genuinely new observational constraint (the stacked secondary-flare upper limit). It is not a first measurement of the secular evolution or a first EMRI-plus-precessing-disk fit for this source.

## 🎯 Relevance to Your Research

Directly relevant: the reader co-authored the 3.5-year eRO-QPE2 timing paper (Pasham et al. 2024) and works on EMRI-disk QPE timing models. This paper takes a firm side in the current dispute over eRO-QPE2 (two eruptions per orbit plus a precessing disk, versus one eruption per orbit plus apsidal precession or a hierarchical triple, as in Arcodia et al. 2026). It also supplies a new empirical upper limit on faint intermediate flares that any one-eruption model must now satisfy. The timing machinery is the authors' established Kerr osculating-orbit code, so for the reader the value is the observational constraints and the modulation taxonomy, not the method.

📖 **Where to start:** Section 2.2 (secondary-flare stacking and the one-versus-two-eruption argument; the main new content), Section 3 (analytic in-phase versus anti-phase modulation taxonomy, a useful reference), and Section 4.3 (timing posteriors, especially the split into a geometric versus eccentric long-short contrast). Sections 2.1 and 4.2 can be skimmed.

## Scores

- 🔬 **Quality:** 5/10
- 🎯 **Relevance:** 8/10
- 🌠 **Reading priority:** Should-Read (weighted score 5.5/10)

## 🚧 Caveats

- Mostly an update of the same group's earlier eRO-QPE2 fits (2411.18046, 2605.29382) to all 11 XMM epochs; the stacked secondary-flare limit is the main new result.
- The 0.56% secondary-flare limit is in 0.2-2 keV counts, while the simulation asymmetries it is compared with are bolometric.
- The 'oscillation' in quiescent flux is a deviation of a few points from a linear trend, not a detected period.
- Eccentricity limit e < 0.033 depends on the model attributing most of the early long-short timing contrast to light-travel geometry; mass, spin and disk parameters are unconstrained.
- Does not use the denser 2026 multi-mission campaign data, and does not directly rebut the competing analysis that found no period decay over a month (|dP/dt| < 2e-6).

---

🔗 [Back to the weekly digest](../2026-10-20)
