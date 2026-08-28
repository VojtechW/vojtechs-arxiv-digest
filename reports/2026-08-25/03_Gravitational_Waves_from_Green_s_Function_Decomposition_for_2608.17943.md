# 🎵 Gravitational Waves from Green's Function Decomposition for a Kerr black hole: I. Equatorial ISCO Plunge

**Citation:** Junquan Su, Neev Khera, Abhishek Chowdhuri, Marc Casals, Huan Yang, *Gravitational Waves from Green's Function Decomposition for a Kerr black hole: I. Equatorial ISCO Plunge*, arXiv:[2608.17943](https://arxiv.org/abs/2608.17943) [gr-qc], submitted 18 Aug 2026.

**In one sentence:** The authors split the response of a spinning black hole into a prompt part, a ringing part and a slowly fading part, and use it to separate the wave emitted by a small body falling into the hole, while finding that the spin introduces a new mathematical obstruction that prevents them from pinning down exactly when one part ends and the next begins.

## Executive Summary

The paper carries the authors' own Schwarzschild G+/G- Green's-function decomposition over to the Teukolsky equation on Kerr, building the radial Green's function from MST and Jaffe series at high precision and analytically continuing the spin-weighted spheroidal harmonics in the complex frequency plane. They find a genuinely new structural feature absent in Schwarzschild: the spheroidal eigenvalue produces angular branch cuts, so the causal split time for an isolated (l,m) mode is not fixed by the analysis and is instead set operationally to the Schwarzschild value |r_*| + |r'_*|, with an unresolved window of width O(a) around it. Fixed-source kernels built from the direct-part contour plus 42 QNM poles are compared with an independent 2+1 time-domain Teukolsky evolution at a = 0.4M and track it away from the causal fronts. The headline application, the (2,2) waveform of a finite-start equatorial ISCO plunge at a/M = 0.1, 0.4, 0.7, is not actually computed from the contour decomposition: it is a real-frequency inverse Fourier transform that is then time-windowed by causal indicators, yielding a direct-part contribution that terminates exactly at the retarded time at which the particle crosses r'_* = 0.

## Claimed Contribution

Extension of the frequency-domain Green's-function split (branch-cut direct part, quasinormal-mode sum, late-time tail) from Schwarzschild to Kerr in the time domain, validated against time-domain Teukolsky simulations, plus what the paper calls the first numerical extraction of the branch-cut direct part in Kerr and its application to the leading-order-in-mass-ratio ringdown of an equatorial ISCO plunge.

## Strengths

- The Kerr angular branch cuts are a real structural discovery, not a bookkeeping detail: because the spheroidal eigenvalue depends on a*omega, the mode-by-mode causality argument that works in Schwarzschild simply fails, and the paper says so explicitly rather than papering over it.
- Serious numerical machinery, not hand-waving: 160-bit MST with 400 series terms, 8000 Jaffe terms, a Riccati/Sasaki-Nakamura handoff above M*omega = 0.4 with an explicit overlap-band cross-check, Planck-tapered nonuniform frequency grids and degree-11 Hermite panels with analytically integrated oscillatory phases.
- The QNM pole sum goes past the published Cook et al. Kerr datasets (n > 32 obtained by their own root tracking), and they note the n = 8 label carries two distinct roots under continuous tracking in spin - the kind of detail that only shows up if the calculation was really done.
- Independent validation channel: the fixed-source contour reconstruction is compared against a separate compactified 2+1 time-domain Teukolsky solver, at future null infinity, not just against another frequency-domain calculation.
- The direct-part termination time has a clean, checkable derivation (u_D,end = sup over r'_* > 0 of t_p(r') + r'_*) and matching numbers to six digits at three spins; the claim that the direct part vanishes by loss of causal support rather than by damping is a falsifiable statement.
- Useful negative result for the community: the 'direct wave' of Oshita et al. is explicitly plotted alongside and shown to be a different object from the branch-cut direct part, which should stop a terminological confusion before it spreads.

## Weaknesses

- The abstract's claim that 'the split times are determined by the black hole spin and positions of the emitter and receiver' is contradicted by the paper's own introduction, which states that within a window of width O(a) the large-arc contribution is not understood, that the split time is set 'operationally' to the Schwarzschild value, and that the exact split time is left to future studies.
- The abstract says 'excellent agreement' with the time-domain simulations; the introduction of the same paper says 'qualitative agreement', and Sec. 5 says the curves are 'visually indistinguishable on the scale of the lower panel'. No quantitative error metric against the time-domain code appears anywhere - the only stated tolerances (1e-7, 1e-8) are internal chirp-z versus panel-sum consistency checks of the same integral.
- The headline plunge waveform does not use the decomposed Green's function. It is a full real-axis inverse transform multiplied by causal indicator functions. Since the validity of exactly those indicators for an isolated (l,m) mode in Kerr is what the angular cuts call into question, the labelled 'direct part' and 'QNM part' are assumed rather than derived, with no error budget on the assumption.
- The tail is never computed. 'QNM+Tail' is an honest label for an unevaluated object: neither the radial branch-cut integral nor the angular-cut jump integrals are evaluated anywhere in the paper, and any signal falling outside the two indicator supports is assigned to neither sector and simply called an approximation.
- Truncating the direct-part contour produces a spurious front spike about 3e5 times the physical peak. The paper diagnoses this correctly as nonuniform convergence, but the response is to abandon the contour method for production runs, which is precisely an admission that the advertised technique is not yet usable for waveforms.
- Narrow scope: one mode (s, l, m) = (-2, 2, 2), one trajectory family, three moderate spins (0.1, 0.4, 0.7), observer at future null infinity only. Nothing near high spin, where the angular cuts, QNM branching and overtone convergence problems are sharpest and where the method would actually be tested.
- The manuscript is visibly unfinished: live \draftgraphic placeholders, \blue/\green/\rev revision markers in the typeset text, abandoned draft paragraphs with empty \cite{} commands, and unresolved co-author dialogue left in the source - including a comment from one author objecting that the text 'sounds as though we get the plunge waveform from a direct part+QNM calculation but we don't'.

## Skeptic's Cross-Examination

If the causal-support prescription used for the plunge is exactly correct, then the 'decomposition' of the plunge waveform contains no information beyond the ordinary waveform plus the trivial statement 'cut it at u = t_p(r') +/- r'_*', and the Green's-function apparatus is decoration. If it is not exactly correct - which the paper's own angular-cut discussion says it may not be for an isolated (l,m) mode in Kerr - then the direct-part and QNM curves in the money figure carry an unquantified systematic error, and no bound on it is given. The paper never resolves which of these two it is, and that is precisely the question the title promises to answer.

## Novelty in Context

The G+/G- split, the branch-cut reformulation of Leaver's problematic large-arc term, and the phrase 'branch-cut direct part' are all from this same group's Schwarzschild paper (Su, Khera, Casals, Ma, Chowdhuri, Yang, arXiv:2601.22015, PRD 113, 104013), seven months earlier; related contemporaneous work includes De Amicis et al. arXiv:2506.21668 on dynamical QNM excitation and Aruquipa & Casals arXiv:2603.07747 on Regge-Wheeler and Teukolsky Green functions in Schwarzschild. So the conceptual framework is not new here. Casals and collaborators have also computed Schwarzschild QNM-plus-branch-cut Green functions for over a decade (Casals & Ottewill 2013; Casals, Dolan, Ottewill & Wardell 2013), and no comparable Kerr branch-cut calculation turns up in the literature, so 'first numerical extraction of the branch-cut direct part in Kerr' is plausible as stated. But that claim should be read narrowly: what is new is the Kerr/Teukolsky implementation and the identification of the angular cuts, not the decomposition idea. And the correspondingly bigger-sounding abstract claims - that split times are determined by spin and positions, and that the decomposed Green's function is what produces the plunge waveform - are both walked back in the body.

## Relevance to Your Research

Directly adjacent to Kerr perturbation-theory infrastructure: MST and Jaffe radial solutions, analytic continuation of spin-weighted spheroidal harmonics in a*omega, high-overtone Kerr QNM root tracking, and the retarded Green function whose branch cut is the same object that matters for the method of matched expansions in self-force. The angular-cut discussion is the part most likely to change how someone thinks about the analytic structure of the Kerr Teukolsky Green function, and it is not something you would get from the Schwarzschild literature. Less useful if the interest is waveform accuracy - as production waveform technology this is not yet competitive with anything.

**Where to start:** Sec. 3.2 and Appendix on the angular cuts and the large-frequency split time in Kerr (the actual new structure); the split-time paragraphs of the Introduction, which contain the honest version of the abstract's claim; Sec. 4.3 and Sec. 5, especially Eq. (real-axis-time-split), for what the 'decomposition' of the plunge waveform actually is; Sec. 6.2 for the direct-part termination time. Sec. 3.5 and the appendices on MST/Jaffe implementation are worth skimming for numerical technique.

## Scores

- **Quality:** 6/10
- **Relevance:** 6.5/10
- **Reading priority:** 🌟 Must-Read

## Caveats

- The abstract says the split times 'are determined by the black hole spin and positions'; the body says the opposite - in Kerr the split time is set by hand to the Schwarzschild value, with an O(a)-wide window where the analysis breaks down.
- The plunge waveform is not computed from the decomposed Green's function. It is a real-frequency inverse Fourier transform, cut into pieces by causal indicator functions whose validity for a single (l,m) mode in Kerr is exactly what the paper leaves open.
- 'Excellent agreement' with the time-domain code is asserted but never quantified; elsewhere the same comparison is described as qualitative and visual.
- The late-time tail is never evaluated, and neither are the angular-cut jump integrals; 'QNM+Tail' means 'whatever is left after the front'.
- One mode, one trajectory family, three moderate spins, no high-spin case.
- This is a v1 with draft figure placeholders, revision-colour markup and internal co-author comments still in the source; expect the text to change.

## In Network

- 🚩 Huan Yang — notable author

---

[Back to the weekly digest](../2026-08-25)
