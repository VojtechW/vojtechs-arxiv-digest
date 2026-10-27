# ♻️ PSR J0653+0443: An Eclipsing Millisecond Pulsar in an Extremely Eccentric Double Neutron Star System

🔦 **Worth-Skimming** · 🔬 Quality 6/10 · 🎯 Relevance 3.5/10

📎 **Citation:** Z. L. Yang, J. L. Han, L. G. Hou, Z. W. Chen, Y. G. Gong, Y. L. Guo, Y. J. Lu, C. Zhang, K. Y. Song, B. Liu, D. Lai, C. Wang, W. Q. Su, P. F. Wang, X. P. You, N. N. Cai, Q. Gao, W. C. Jing, B. Wang, H. G. Wang, T. Wang, J. Xu, Y. Yan, D. J. Zhou, *PSR J0653+0443: An Eclipsing Millisecond Pulsar in an Extremely Eccentric Double Neutron Star System*, arXiv:[2610.29838](https://arxiv.org/abs/2610.29838) [astro-ph.HE], submitted 21 Oct 2026.

> 💡 Radio astronomers using the Chinese FAST telescope have found a pair of neutron stars on the most elongated orbit ever measured for any binary star, swinging from far apart to less than a solar radius apart once every 79 days, and briefly hiding one star behind the other.

## 🔍 Executive Summary

The paper reports the FAST discovery and two years of timing of PSR J0653+0443, a 47.5 ms partially recycled pulsar in a 79.08-day double neutron star orbit with eccentricity 0.99238692, the highest measured for any stellar binary. Periastron advance gives a total mass of 2.814 solar masses, and a weak Shapiro-delay constraint splits this into about 1.38 and 1.44 solar masses with inclination 76 (+8/-15) degrees. One periastron observation shows an 85-second eclipse near superior conjunction, which the authors attribute to the companion's magnetosphere. The paper also fits the orbital-phase-dependent part of the relativistic periastron shift (a millisecond-level timing signature) to bound any non-relativistic precession, runs a population synthesis arguing such systems are rare, and computes the burst-like gravitational-wave signal, which LISA cannot detect (signal-to-noise about 0.1) but which proposed larger detectors might.

## 📣 Claimed Contribution

Discovery of a Galactic-field double neutron star with record orbital period and eccentricity; the second double neutron star seen to eclipse, after the double pulsar; the largest timing modulation from orbit-phase-dependent periastron advance in any such system, used to constrain a non-relativistic precession rate more tightly than for the double pulsar; a reparametrised Keplerian timing model (DDe/DDeGR) that removes the near-degeneracy of x, omega and e at high eccentricity; a population-synthesis claim that the system challenges standard binary evolution; and a prediction that its periodic gravitational-wave bursts, peaking near 0.36 mHz, are detectable by LISAmax-class missions.

## ✅ Strengths

- A genuinely new and extreme object: e = 0.99238692 +/- 5e-8 from a dedicated two-hour FAST track through periastron, with a phase-connected solution over more than two years.
- Pragmatic and well-motivated timing reparametrisation (zeta_1, zeta_2, sqrt(1-e^2)) that cuts parameter correlations from |r| about 0.999 to about 0.1-0.3; useful for other very eccentric binaries.
- The total mass from periastron advance is robust (2.814 +0.018/-0.021 solar masses), and the companion mass bound (at least 1.38 solar masses) makes the double-neutron-star identification secure.
- The gravitational-wave section is honest about LISA: it states an expected signal-to-noise of about 0.11 instead of claiming detectability by the funded mission.
- The quoted merger time (2.54 Gyr) agrees with a quick Peters-formula estimate (about 3 Gyr).

## ⚠️ Weaknesses

- The relativistic content is textbook: the phase-dependent periastron shift is the Damour-Deruelle 1985/86 k-term, and the idea of separating relativistic from non-relativistic precession through their different orbital-phase dependence comes from Damour-Deruelle 1986, as the paper itself acknowledges. The new part is the size of the effect in this system, not the method.
- The headline non-relativistic precession 'measurement', -1.5 (+0.9/-0.8) x 10^-4 deg/yr, is about a 1.7-sigma deviation from zero. The authors admit it is consistent with zero at 95 percent, yet it appears in the abstract as if it were a result.
- Inclination is presented inconsistently. The main text says sin i >~ 0.98 and that the eclipse 'confirms' an edge-on orbit, but the timing fit gives i = 76 (+8/-15) degrees, the Shapiro-only fit gives sin i = 0.93(10), and explaining the eclipse at i = 76 needs a companion spin period of about 35 s with the double-pulsar magnetosphere scaling. The eclipse comes from one 85-second event in a single observation, and the paper discusses no alternative explanations.
- Sloppy numbers: the total periastron advance is quoted as 0.017791 deg/yr in the main text and 0.017785(11) in Methods; the general-relativistic part is written as 0.1790(10) deg/yr, which is off by a factor of ten; velocity units are given as km s^-3. Large commented-out blocks and revision markup remain in the source, which suggests the manuscript was not finalised.
- The binary-evolution claim ('challenges current understanding', probability <~5e-3) is undercut by a companion paper from overlapping authors (arXiv:2610.31583). Once survey selection effects are included, it finds such systems 'compatible with standard binary evolution', with about 0.3 expected detections in the survey.
- The gravitational-wave section only applies Peters-Mathews and quadrupole formulae; the detectability claims rest on proposed concept missions (Folkner, LISAmax), not funded ones.
- The Einstein delay (about 45 ms) is not measured; it is fixed from the general-relativistic mass solution because it is degenerate with zeta_2. Only two post-Keplerian parameters are effectively constrained, and the Shapiro delay only marginally, so no meaningful test of general relativity is possible yet.

## 🤔 Skeptic's Cross-Examination

Take away the record numbers and what remains is a standard binary-pulsar timing solution with one well-measured post-Keplerian parameter (periastron advance), a marginal Shapiro delay, an unmeasured Einstein delay, a 1.7-sigma 'non-relativistic precession', and a single 85-second signal drop interpreted as a magnetospheric eclipse that requires a roughly 35-second companion at the best-fit inclination. The 'challenge to binary evolution' disappears once selection effects are included, by the authors' own companion paper, and the gravitational-wave signal is undetectable by any approved mission. The object is remarkable; the physics extracted from it so far is thin.

## 🆕 Novelty in Context

The discovery itself is new. INSPIRE returns only this paper and a follow-up population-synthesis letter (Chen, Zhang, Lu, arXiv:2610.31583) for this pulsar, and the eccentricity beats the previous stellar-binary record (0.985) and every known double neutron star, all of which have e below about 0.8. The secondary novelty claims are smaller than presented. (i) The orbit-phase-dependent periastron advance and the separation of relativistic from non-relativistic precession are from Damour-Deruelle (1985, 1986), and Damour-Taylor (1992) applied them to B1913+16; the paper says 'as proposed in Damour-Deruelle 1986', so the real claim is only 'largest such modulation observed'. (ii) The 'more precise than the double pulsar' bound on non-relativistic precession is a 1.7-sigma number, not a detection. (iii) The tension with binary evolution is contradicted by the companion letter, which includes survey selection effects. (iv) Eclipses in double neutron stars were previously seen only in J0737-3039A/B, so 'second eclipsing double neutron star' is correct if the eclipse interpretation holds. (v) The DDe/DDeGR reparametrisation is an ELL1-style change of variables for e close to 1. It is useful but incremental, and I did not check whether similar high-eccentricity parametrisations already exist in the timing literature.

## 🎯 Relevance to Your Research

Peripheral to self-force and extreme-mass-ratio inspiral work. The physics is 1PN Damour-Deruelle timing plus Newtonian-order quadrupole radiation. The interest for a relativist is the object itself: a Galactic binary in the near-parabolic regime that emits gravitational waves as periodic periastron bursts, with power peaking near the 2440th harmonic. That is a concrete real-world example for eccentric-burst waveform and frequency-domain harmonic-sum methods, and possibly a future source for a sub-mHz detector. Worth knowing the object exists. There is little to learn from the methods.

📖 **Where to start:** Main-text sections 'Pulsar J0653+0443 and its extraordinary orbit' and 'The relativistic effects' (about 10 minutes, all the key numbers). Methods 'Keplerian parameters and modified timing models' if you care about timing near-parabolic orbits. Methods 'GW emission and future evolution' for the burst waveform and characteristic-strain figure. Skip the population synthesis and read arXiv:2610.31583 instead.

## Scores

- 🔬 **Quality:** 6/10
- 🎯 **Relevance:** 3.5/10
- 🔦 **Reading priority:** Worth-Skimming (weighted score 3.5/10)

## 🚧 Caveats

- The relativistic timing physics is standard Damour-Deruelle; the novelty is the object, not the method.
- The headline 'non-relativistic periastron advance' is a 1.7-sigma result that is consistent with zero.
- The eclipse is one 85-second event; the timing inclination (76 degrees) sits awkwardly with the 'edge-on confirmed' wording.
- Not detectable by LISA (signal-to-noise about 0.1); detectability claims refer to proposed missions only.
- A companion paper by overlapping authors (arXiv:2610.31583) finds the system compatible with standard binary evolution, contrary to this paper's framing.
- Several numerical typos and inconsistencies (periastron advance values, units).

---

🔗 [Back to the weekly digest](../2026-10-27)
