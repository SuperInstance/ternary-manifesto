# ternary-manifesto

[![SuperInstance](https://img.shields.io/badge/part%20of-SuperInstance-purple.svg)](https://github.com/SuperInstance)

Research documents for the SuperInstance ternary fleet — open questions, research directions, and the cross-pollination audit of 211+ crates.

## What's Here

This repo is the research spine of the SuperInstance ecosystem. It contains two documents:

- **CROSS_POLLINATION_AUDIT.md** — A structural analysis of all 211 ternary crates, their thematic clusters, and missing cross-links between them
- **RESEARCH_FRONTIERS.md** — Open mathematical conjectures and research directions for ternary systems

## CROSS_POLLINATION_AUDIT.md

An audit of the entire fleet's internal documentation links. Key findings:

- **211 crates** audited (215 Rust + Python/C/WASM)
- **76 crates** have `See Also` sections linking to other ternary crates
- **135 crates** have zero outbound links — isolated from their neighbors
- Crates grouped into **13 thematic clusters**: Audio, Grid/CA, Agent Coordination, Evolution, Perception/AI, Math, Compiler, Storage, Games, Visualization, Core, Experiment, and Fleet Orchestration (nautical metaphors)

The audit identifies specific missing links for each isolated crate, ranking them by thematic adjacency. Example: `ternary-adversarial` should link to `ternary-arena`, `ternary-agent`, `ternary-failure`, and `ternary-noise` — but currently links to none of them.

### Thematic Clusters

| Cluster | Size | Example Crates |
|---------|------|----------------|
| Audio / Music | 24 | `bite`, `echo`, `harmonic`, `muse`, `sampler`, `wave` |
| Grid / Cellular Automata | 14 | `life`, `collatz`, `sandpile`, `ising`, `automata` |
| Agent Coordination / Fleet | 36 | `bus`, `sync`, `captain`, `consensus`, `constellation`, `harbor` |
| Evolution / Genetics | 13 | `ga`, `genome`, `fitness`, `swarm`, `symbiont` |
| Perception / AI | 16 | `attention`, `bayesian`, `cortex`, `oracle`, `rl` |
| Math / Complexity | 20 | `entropy`, `tensor`, `topology`, `quantum`, `chaos` |
| Storage / Infrastructure | 19 | `database`, `archive`, `foundry`, `shipyard` |
| Fleet Orchestration (nautical) | 33 | `anchor`, `beacon`, `helm`, `lighthouse`, `voyage` |

## RESEARCH_FRONTIERS.md

Six open mathematical conjectures and four research direction categories:

### Open Conjectures

1. **Ternary Kuramoto Paradox** — Ternary coupling {-1, 0, +1} cannot achieve full synchronization for N > 3 oscillators. The discrete coupling introduces quantization noise that prevents convergence.

2. **Ternary Shannon Entropy Anomaly** — Maximum ternary entropy is log₂(3) ≈ 1.585 bits — the first arity exceeding 1 bit. There exists a "ternary compression limit" of log₂(3)/2 ≈ 0.793 as a fundamental constant.

3. **Ternary Renormalization Group Fixed Point** — Is there a ternary analog of the Wilson-Fisher fixed point? A ternary field at criticality with invariant fractal structure under coarse-graining would define a new universality class.

4. **Counterpoint in Z₃: The "Ternary Tritone" Problem** — The longest valid first-species ternary counterpoint (beginning/ending on unison, no parallel tritones) has length exactly 8 — the Pisano period.

5. **Ternary Sheaf Cohomology and Agent Consensus** — For N agents with ternary beliefs, H¹ counts irreducible "rifts" — persistent disagreements no protocol can resolve. H¹ = 0 guarantees consensus.

6. **Ternary Crystallography** — Exactly 5 ternary space groups in 2D and 17 in 3D, paralleling wallpaper and space groups but for different algebraic reasons (Z₃ vs continuous symmetry).

### Research Directions

| Direction | Proposed Crates |
|-----------|----------------|
| Ternary Physics | `ternary-gravity`, `ternary-quantum-v2`, `ternary-thermodynamics-v2`, `ternary-optics` |
| Ternary Biology | `ternary-genetics`, `ternary-ecology`, `ternary-immune`, `ternary-membrane` |
| Ternary Music (Deep) | `ternary-temperament`, `ternary-cadence`, `ternary-counterpoint-v2` |
| Ternary Networks | `ternary-pagerank`, `ternary-small-world`, `ternary-scale-free` |

### The Conservation Law γ + η = C

Both documents reference the ternary conservation law: in any ternary system, the sum of productive energy γ and dissipation η is bounded by a constant C. This is not a metaphor — it's the mathematical relationship between structure and noise in ternary algebra, and it appears in fleet dynamics, cellular automata, musical counterpoint, and cohomology.

## Related Repositories (SuperInstance Ecosystem)

- **ternary-mud** — Ternary algebra MUD rooms with Hodge lostness detection
- **symplectic-fleet** — Hamiltonian fleet dynamics with Noether conservation
- **meta-agent** — Multi-agent task coordination and simulation
- **forgemaster** — GPU fleet orchestration
- **license-compliance** — License compatibility checking for the fleet
