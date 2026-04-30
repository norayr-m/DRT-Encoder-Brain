# DRT Encoder Brain — index of demos

> This is an amateur engineering project. We are not HPC professionals and make no competitive claims. Errors likely.

A single repository that bundles several browser demos exploring the Distributed Reconstruction framework — the cellular biology layer (HPA axis), the harmonic solver, the generator/scanner pair, the pipeline, the supernova solver, the rank-sphere viewer, and a city/grid-DRT pair. One repo, many small standalone HTMLs.

**[Live landing page →](https://norayr-m.github.io/DRT-Encoder-Brain/)**

## What it does

Open the landing page and pick a demo. Each is a self-contained HTML file with no build step, no server, no external dependencies beyond a modern browser. The demos:

- **Cellular Graph Simulator** — small cells on a non-grid graph, each with local rules, scored by Bach BWV 847; emerges into HPA-axis-flavoured visuals.
- **Generator (7-Column Signal QED)** — a discrete pipeline (rotating clock → lookup table → routing matrix → weighted nodes) shown side-by-side with the equivalent deep-graph unification.
- **Scanner (7-Column Signal QED)** — the dual of the generator: signal flows from a master back through the columns, used for inspecting reconstruction quality.
- **Harmonic Solver** — a small multi-agent debate visualization.
- **Pipeline (BWV 847)** — a composer/decomposer pair running in parallel on the C-minor fugue.
- **Supernova / Orbital Solver** — observers on orbital paths, with reconstruction at convergence points.
- **CityDRT, GridDRT, GridDRT-Demo** — early sketches of the framework on city / power-grid topologies.
- **rank-sphere v05 / v06 / `rank-sphere.html`** — the rank-by-rank navigable sphere used by the decoder.

The repository is, in effect, the early sandbox where the framework was first explored visually before the v0.1 paper.

## Why it matters (DRT angle)

This is the **explorer's index**. Each demo is one slice of the same underlying question: what happens when many partial observers, each with a small projection of the global state and a learned "completion" back to it, are aggregated. The demos are deliberately small and visual rather than rigorous.

The honest current claim from v0.1 is conditional: under four explicit hypotheses and a bounded computational budget, the aggregate exposes structure not accessible from the original signal alone within the same budget. The earlier "norm-growth" framing seen in some demo prose has been retracted; the present claim is about computational accessibility, not about norms. Read the demos in that light.

## How to run

Clone, then open whichever demo HTML you want directly in a browser.

```
git clone https://github.com/norayr-m/DRT-Encoder-Brain.git
open DRT-Encoder-Brain/index.html
```

Each demo is a single HTML file in the repository root. No dependencies. Audio is opt-in where present.

## File map

- `index.html` — landing
- `2026-03-23_-cell_simulator-NM_v01.html`
- `2026-03-23_-generator-NM_v01.html`
- `2026-03-23_-harmonic_solver-NM_v01.html`
- `2026-03-23_-pipeline-NM_v01.html`
- `2026-03-23_-scanner-NM_v01.html`
- `2026-03-23_-supernova_solver-NM_v01.html`
- `CityDRT_2026-03-23_NM_v01.html`
- `GridDRT_2026-03-23_NM_v01.java` — Java sketch
- `GridDRT-Demo_2026-03-23_NM_v01.html`
- `rank-sphere.html`, `rank-sphere_2026-03-01_NM_v05.html`, `rank-sphere_2026-03-01_NM_v06.html`

## References

- Distributed Reconstruction work — v0.1 in preparation, N. Matevosyan and A. Petrosyan.
- Bach, BWV 847 — *The Well-Tempered Clavier*, Book I (1722).

Visualizations co-authored with Claude (Anthropic).

## Author

Norayr Matevosyan

## License

GPLv3
