# 📈 Time-frequency analysis for LISA: Fast waveform templates

🌠 **Should-Read** · 🔬 Quality 6/10 · 🎯 Relevance 6/10

📎 **Citation:** Neil J. Cornish, *Time-frequency analysis for LISA: Fast waveform templates*, arXiv:[2609.28316](https://arxiv.org/abs/2609.28316) [gr-qc], submitted 23 Sep 2026.

> 💡 A single toolkit builds LISA signal templates for galactic binaries, merging massive black holes and extreme-mass-ratio inspirals directly as sparse time-frequency maps, without ever computing the full year-long waveform, and in one precessing black-hole test it is about two thousand times faster than the direct calculation with essentially no loss of accuracy.

## 🔍 Executive Summary

The paper describes how to generate LISA templates directly in the orthogonal Wilson-Daubechies-Meyer time-frequency basis. The source model supplies only slowly sampled amplitudes and phases along each harmonic, and the detector response comes from an improved version of the author's 'TDI on the fly' sparse-response method. The main trick is that shifting a signal in frequency by an even number of wavelet layers leaves the transform unchanged, so each harmonic can be shifted down to near zero frequency and handled with small FFT blocks or a chirplet lookup table. Merger, plunge and turning points in frequency get short direct-evaluation segments, joined on with a partition of unity. A second scheme, 'TDI Tapestry', transforms the two polarizations first and then applies the detector response pixel by pixel, keeping both wavelet quadratures and a first-order frequency correction; this is meant for waveforms with many harmonics, such as EMRIs. The one fully quantified test is a precessing IMRPhenomTPHM binary: matches of 0.99998 in each TDI channel, and a roughly 2000-fold speedup on one CPU core.

## 📣 Claimed Contribution

A unified family of 'templates without waveforms' algorithms for three LISA source classes (galactic binaries, massive black-hole binaries including precessing IMRPhenomTPHM, and FEW EMRIs), built from sparse carrier tracks. Specific new pieces: a complex heterodyne that shifts by an even number of wavelet layers, replacing the earlier real heterodyne; a forward-marching adaptive grid for TDI-on-the-fly that no longer needs seeding at merger; splining the TDI modulation in Cartesian form, so no inverse tangents or phase unwrapping are needed; source-dependent endpoint handling for mergers, plunges and EMRI frequency turnovers; and 'TDI Tapestry', which applies the detector response after the polarizations have been transformed to the wavelet basis.

## ✅ Strengths

- One carrier-based interface covers galactic binaries, higher-mode and precessing massive black-hole binaries, and many-harmonic EMRIs, including EMRI harmonics whose frequency turns over and binaries whose frequency decreases because of mass transfer.
- TDI Tapestry is a new and sensible reordering for many-harmonic signals. The paper gives a clear argument that the real Wilson transform alone cannot carry the complex response, so both quadratures must be kept. A first-order frequency correction reportedly cuts the mismatch from about 1e-3 to about 1e-5.
- Careful practical engineering: continuous bracket refinement avoids template jumps under tiny parameter changes, the Cartesian spline stays regular through response nulls, the three time stamps (barycentric, guiding-center, per-link retarded) are kept separate, and partition-of-unity joins replace hard switch-overs.
- The precessing massive black-hole test is concrete: X, Y and Z matches of 0.999985, 0.999993 and 0.999985 without maximization, and over 99.99997% of the reference power inside the sparse support.
- Memory is small and the per-pixel kernels are highly regular, which makes the method a good candidate for GPU likelihoods in a LISA global fit.

## ⚠️ Weaknesses

- Validation is thin and anecdotal. The only fully quantified accuracy and timing test is one precessing massive black-hole binary. For EMRIs the paper gives no match against a direct TDI plus wavelet reference in the sections read, only that the FFT and lookup methods have 'similar CPU costs' and that the FFT path is 'currently' more accurate.
- The roughly 2000-fold speedup is measured against the author's own unoptimized direct pipeline. A commented-out passage in the LaTeX source concedes that the baseline 'is not a fully optimized dense-waveform baseline'. There is no timing comparison with existing frequency-domain or GPU LISA response codes.
- The Tapestry accuracy figure (mismatch from 1e-3 to 1e-5) is stated 'in the tests performed here', with no description of the parameter range, sources or number of cases.
- The EMRI plunge is closed with an ad hoc C^1 attachment of a Kerr quasinormal-mode ringdown to each FEW mode. Its only purpose is to suppress spectral leakage, and its effect on template accuracy, or on biases near plunge, is not quantified.
- The grid tolerances were 'arrived at by testing across a wide range of source parameters', but the testing is not shown. There is no systematic study of mismatch as a function of parameters, observation length or signal-to-noise ratio.
- No public code is mentioned, so the algorithms are hard to reproduce from a short methods note that mostly describes rather than demonstrates.
- Much of the text is implementation bookkeeping (figure descriptions, knot placement, handoff rules), while the error analysis is qualitative.

## 🤔 Skeptic's Cross-Examination

This is an engineering description of one author's in-house code, and the numbers do not show it is ready for production. The single end-to-end benchmark is a massive black-hole binary compared against a deliberately unoptimized baseline. The EMRI case, the one most relevant to a many-harmonic Tapestry argument, has no quantified accuracy or speed comparison against FEW with its GPU response, and its plunge relies on an unphysical quasinormal-mode patch. Until the paper shows systematic mismatches over EMRI parameter space and wall-clock comparisons with existing GPU pipelines, the claim of 'fast templates' for EMRIs is a plausible design, not a demonstrated result.

## 🆕 Novelty in Context

The groundwork is the author's own. Cornish 2020 (arXiv:2009.00043) already introduced fast wavelet-domain templates built from local amplitude, phase, frequency and frequency derivative, including the lookup-table idea; the paper says so itself ('introduced in Ref. Cornish:2020odn'). Cornish and Littenberg 2025 (arXiv:2506.08093) introduced TDI on the fly, with a claimed ten-thousand-fold response speedup. So the headline 'templates without waveforms' is not new. The incremental contributions are the complex even-layer heterodyne, the general forward adaptive grid, the Cartesian response spline, and the endpoint and turnover machinery. The one conceptually new element is TDI Tapestry: applying the frequency- and time-dependent response after the wavelet transform, using both quadratures and a first-order frequency expansion. The paper is honest about its lineage and does not overclaim priority. An INSPIRE search for recent time-frequency LISA work found search pipelines (cWB-space, excess-power premerger detection, stellar-mass black-hole searches) but no competing wavelet-domain template generator for EMRIs. The extension to FEW EMRIs therefore looks new, though it is presented with little quantitative support. The paper does not compare against the established frequency-domain or GPU response codes (for example the Marsat-Baker style Fourier-domain response, or the GPU LISA response used with FEW). The speed claim is measured against the author's own unoptimized direct baseline, not the current state of the art.

## 🎯 Relevance to Your Research

Moderately relevant to EMRI data-analysis readers. It is a concrete proposal for producing FEW-style EMRI templates in a wavelet basis that handles nonstationary noise and data gaps natively. It also flags practical EMRI issues: harmonics turning over before plunge, abrupt waveform termination causing spectral leakage, and the cost of dozens of harmonics. Of limited direct interest to self-force or waveform-theory work; the value lies in understanding what a LISA global-fit pipeline will require of EMRI waveform outputs (slowly sampled amplitude and phase per harmonic, plus a clean plunge termination).

📖 **Where to start:** Section II.D (sparse Meyer-Wilson transform and the even-layer complex heterodyne), Section II.E (source-dependent endpoints: EMRI turnovers and the quasinormal-mode plunge patch), Section II.F (templates without waveforms: partitioned FFT versus lookup table), Section III (TDI Tapestry). Section II.G has the only quantified benchmark.

## Scores

- 🔬 **Quality:** 6/10
- 🎯 **Relevance:** 6/10
- 🌠 **Reading priority:** Should-Read (weighted score 4.8/10)

## 🚧 Caveats

- The only quantified accuracy and speed benchmark is one precessing massive black-hole binary; the EMRI claims come without matches or timings.
- The roughly 2000-fold speedup is measured against the author's own unoptimized direct code, not against existing GPU or frequency-domain LISA response codes.
- The EMRI plunge uses an ad hoc quasinormal-mode ringdown attached to each FEW mode, only to suppress spectral leakage.
- The heterodyned wavelet templates and TDI on the fly come from the author's 2020 and 2025 papers; the new parts are TDI Tapestry and a set of refinements.
- No code release is mentioned.

---

🔗 [Back to the weekly digest](../2026-09-29)
