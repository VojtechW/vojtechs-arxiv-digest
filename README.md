# 📜 Vojtěch's arXiv Digest

**Live site:** [vojtechw.github.io/vojtechs-arxiv-digest](https://vojtechw.github.io/vojtechs-arxiv-digest/)

Every Tuesday morning, a scheduled task in [Claude Cowork](https://claude.ai) pulls the week's arxiv notification emails, parses several hundred papers across gr-qc, astro-ph.HE, hep-th, and related categories, and produces a curated digest published here on GitHub Pages. I also get an email with a link so I can skim it from my phone over coffee.

## What it does

The pipeline fetches my arxiv mailing-list notifications from Gmail, scores papers by keyword relevance and author proximity, selects roughly ten candidates, then downloads and critically reads each one before deciding which survive. The output is a tiered weekly report (Must-Read / Should-Read / Worth-Skimming) with individual write-ups for every paper that passes review, plus a list of papers that failed and why. Updated versions of older papers are tracked separately in a Notable Updates section.

## Selection philosophy

Papers are evaluated along two axes. The first is direct research relevance — anything touching EMRIs, gravitational self-force, black hole perturbation theory, spinning-particle dynamics, post-Newtonian methods, or QPEs gets flagged automatically. The second axis is broader: papers anywhere in black hole or gravitational-wave physics that demonstrate genuine originality, technical depth, or exploration of uncharted territory. A paper does not need to be about my own research topics to make the cut — it just has to be good.

The default assumption is that every paper is low-quality until proven otherwise. The review checks what is genuinely new, whether claims are backed by real calculations rather than speculation, and whether a skeptic would find the result convincing. Formulaic exercises (yet another QNM computation on an exotic metric, routine GR-consistency tests with null results, conference proceedings rehashing published work) are filtered out.

## Repository structure

```
index.md                              — landing page with links to all weekly digests
reports/
  YYYY-MM-DD.md                       — weekly summary for the digest published on that date
  YYYY-MM-DD/
    01_Author_et_al_short_title.md    — individual paper report
    02_Author_et_al_short_title.md
    ...
```

Each weekly summary contains the tiered reading list, failed-paper explanations, a short thematic-trends section, and any notable updates by collaborators.

## About

I'm a gravitational physicist working mainly on extreme mass-ratio inspirals, spinning particles in Kerr spacetime, and black hole perturbation theory. Feel free to browse the digests — if you work in a neighbouring area, you might find them useful too.
