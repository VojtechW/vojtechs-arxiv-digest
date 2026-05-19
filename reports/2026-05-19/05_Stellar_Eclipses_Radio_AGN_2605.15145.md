# 🌑 Eclipses of Nearby Radio-Loud Galactic Nuclei by Stars in Nuclear Star Clusters

**arXiv:** [2605.15145](https://arxiv.org/abs/2605.15145)
**Authors:** Michal Zajaček
**Categories:** astro-ph.GA, astro-ph.HE
**Collaborator flags:** Zajaček (T2)

## Summary

Zajaček proposes that evolved giant/supergiant stars ($R_* \sim 500$-$2000\,R_\odot$) in nuclear star clusters can occult the millimeter radio cores of nearby ($z\sim0.001$) radio-loud AGN, producing detectable dips of $\sim10\%$ depth with durations of $\sim10$ days and recurrence timescales of $\sim10$ years. The key physical reason is that at 230-345 GHz, core-shift effects shrink the radio "photosphere" of the jet base down to $\sim1000$-$2000\,R_\odot$ ($\sim10$-$20\,r_g$ for a $5\times10^7\,M_\odot$ SMBH), making it geometrically comparable to evolved stellar radii. The paper derives a transit-style SMBH mass relation, discusses microlensing/occultation boundaries, and applies it to the PKS 1413+135 ESE case.

## Key Results

- At $z=0.001$, $\nu=230$ GHz the mm radio core is $R_c \sim 2000\,R_\odot \approx 19\,r_g$ for $M=5\times10^7\,M_\odot$, so giants/supergiants can produce 6-25% dips.
- Recurrence timescale $\tau_{\rm rec} \sim 419\,{\rm yr}\,(r/0.1\,{\rm pc})^{3/2}\,(M/5\times10^7)^{-1/2}$; reaching $\sim10$ yr forces orbits to $r\sim 0.01$ pc, dangerously close to the red-giant tidal radius.
- A clean SMBH-mass formula combining $\tau_{\rm rec}$ and $\tau_{\rm dur}$ is derived; applied to PKS 1413+135 gives $M_{\rm BH}\sim 6.6\times10^{17}\,M_\odot$, ruling out bound-star origin.
- Occultation duration $\sim10$ days at 230 GHz with characteristic chromatic signature ($\tau_{\rm dur}\propto\lambda$, $\Delta F/F\propto\lambda^{-2}$).
- Number of expected occulting evolved stars within $r_{\rm SI}$ is $\sim 0.07$-$0.1$ for standard NSC parameters; reaching unity requires steep cusps $\gamma\to 2$.

## Strengths

- Clean, well-organized order-of-magnitude/analytical study that exploits an underexploited window (the mm/VLBI core size matching evolved-star radii in nearby AGN).
- Actionable observational predictions (depths, frequency-dependent chromatic profile) that can be confronted with EHT/ngEHT, ALMA, NOEMA light curves.
- Distinguishes occultation vs. microlensing regimes self-consistently via $R_*/R_E$.
- SMBH-mass formula and negative application to PKS 1413+135 already extracts something quantitative from existing data.

## Weaknesses / Caveats

- The most "interesting" repeating-eclipse regime sits at $r\sim 0.01$ pc, essentially coinciding with the tidal radius of giants/supergiants — acknowledged but not quantitatively folded into the rate estimate.
- The model assumes uniform circular-disk emission; real VLBI mm cores are often elongated jet bases with substructure.
- Core-shift scaling taken as a single power law; significant source-to-source scatter.
- No mention of variability confounders: AGN intrinsic stochastic variability at mm wavelengths can mimic a single 10% dip.
- No actual target list of nearby radio AGN beyond Cen A.

## Novelty Assessment

The proposal builds on the well-established Béky & Kocsis (2013) stellar-transit-in-AGN framework but extends it to a genuinely new observational window. The core insight — that mm/VLBI radio cores at $z\sim 0.001$ shrink to $\sim1000$-$2000\,R_\odot$, geometrically matching evolved-star radii — is correct and, as far as I can tell, has not been spelled out in this form. The link to EHT/ngEHT visibility/imaging artifacts is also noted.

The work is incremental rather than revolutionary: the formalism is standard transit geometry, microlensing dividing line, Bahcall-Wolf cusp number counts. The novelty lies in the synthesis and the specific identification of the mm window as the right place to look. More of a "proposal/concept" paper than a quantitative population study.

## Relevance to Vojtěch

Highly relevant. Vojtěch works on EMRIs and stellar transits across accretion disks as EM counterparts; this paper covers exactly the adjacent geometric-transit signal (stars eclipsing the jet base / synchrotron photosphere) and uses the same NSC/galactic-center machinery. The $M_{\rm BH}$-from-transit formula is conceptually parallel to inferring orbital parameters from disk-crossing flares in QPE-like contexts, and the PKS 1413+135 connection ties into recurring-dip phenomenology adjacent to QPE territory. Zajaček is a Tier-2 collaborator.

## Scores

- **Quality:** 6.5/10
- **Relevance:** 8/10
- **Recommendation:** Should-Read
