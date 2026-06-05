# RESEARCH FRONTIERS — The Ternary Fleet Living Document

*Generated: 2026-06-05*
*Fleet size: 234 repos (215 Rust crates + Python/C/WASM)*
*Total tests: ~4,200*

---

## I. OPEN QUESTIONS

### 1. The Ternary Kuramoto Paradox
**Observation:** In continuous Kuramoto coupling, oscillators can synchronize. In ternary, the coupling term is discretized to {-1, 0, +1}. **Conjecture: ternary Kuramoto cannot achieve full synchronization for N > 3 oscillators.** The discrete coupling introduces a quantization noise that prevents convergence. Only phase-locked states (where all oscillators have the same ternary phase) are possible.

**Why it matters:** If true, this would be the first mathematical proof that ternary systems have fundamentally different synchronization behavior than continuous systems. It would have implications for ternary oscillator networks, ternary phase-locked loops, and ternary consensus protocols.

**Crate to build:** `ternary-kuramoto-v2` with formal proofs of the synchronization impossibility.

### 2. Ternary Shannon Entropy Anomaly
**Observation:** The maximum Shannon entropy for a ternary variable is log₂(3) ≈ 1.585 bits. This is *more* than the maximum binary entropy (1 bit) but *less* than the maximum quaternary entropy (2 bits). The ternary position is information-theoretically special: it's the first arity where entropy exceeds 1 bit.

**Conjecture:** There exists a natural encoding of ternary variables into binary such that the encoding preserves entropy up to a factor of log₂(3)/2 ≈ 0.793, but no encoding can do better. This "ternary compression limit" is a new fundamental constant.

**Crate to build:** `ternary-information` with formal information-theoretic bounds.

### 3. The Ternary Renormalization Group Fixed Point
**Observation:** In `ternary-renormalization`, we observed that the majority-rule coarse-graining of a fully aligned field (+1 everywhere) flows to a fixed point at +1. A random field (equal ±1,0) flows to 0. But what about the *critical* initial condition — the one at the boundary between order and disorder?

**Question:** Is there a ternary analog of the Wilson-Fisher fixed point? A ternary field at criticality would have a specific fractal structure that is invariant under coarse-graining. This would be a *ternary universality class* — a new one, since ternary has no continuous analog.

**Crate to build:** `ternary-critical` — Monte Carlo simulation of ternary Ising model at critical temperature.

### 4. Counterpoint in Z₃: The "Ternary Tritone" Problem
**Observation:** In ternary music, there are only 3 intervals: unison (0), third (1), and tritone (2). The tritone is the *only* dissonance. In species counterpoint, you must avoid parallel tritones — but in ternary, with only 3 interval choices, this constraint is extraordinarily tight.

**Conjecture:** The longest valid first-species ternary counterpoint (beginning and ending on unison, no parallel tritones) has length exactly 8. For longer melodies, parallel tritones are *unavoidable*. This is the ternary analog of the limitation of strict species counterpoint in traditional music theory.

**Connection:** 8 is the Pisano period — the same Fibonacci connection found in `ternary-grain`.

### 5. Ternary Sheaf Cohomology and Agent Consensus
**Observation:** `ternary-sheaf` computes H⁰ and H¹ over Z₃. H⁰ counts global sections (consensus states). H¹ counts obstructions (reasons consensus fails).

**Conjecture:** For a fleet of N agents with ternary beliefs connected in a specific network topology, the first cohomology group H¹ is isomorphic to the space of "persistent disagreements" — local incompatibilities that cannot be resolved by any amount of communication. The dimension of H¹ is the number of independent "rifts" in the fleet.

**Why it matters:** This gives an algebraic characterization of when distributed consensus is achievable. If H¹ = 0, consensus is guaranteed. If H¹ > 0, there are irreducible disagreements that no protocol can resolve.

**Crate to build:** `ternary-consensus-sheaf` — connect `ternary-sheaf` cohomology to `ternary-consensus` protocols.

### 6. Ternary Crystallography: Only 5 Space Groups?
**Observation:** In `ternary-crystal`, we found that the symmetry operations on a ternary lattice are finite (C1, C3i, Oh). Real crystallography has 230 space groups. How many ternary space groups exist?

**Conjecture:** There are exactly 5 ternary space groups in 2D and 17 in 3D — the same numbers as the wallpaper groups and 3D space groups in the binary case, but for different algebraic reasons. The ternary constraint reduces the continuous symmetry groups to discrete ones, but the resulting groups are larger than binary because Z₃ has one more element than Z₂.

---

## II. RESEARCH DIRECTIONS

### A. Ternary Physics
A complete ternary physics stack:
- `ternary-gravity` — gravitational interaction as ternary attraction/repulsion/neutrality
- `ternary-quantum-v2` — Hilbert spaces over Z₃, ternary qubits (qutrits), ternary entanglement
- `ternary-thermodynamics-v2` — heat engines, Carnot cycle, Maxwell's demon in ternary
- `ternary-optics` — refraction, reflection, diffraction with ternary phase shifts
- `ternary-turbulence` — turbulent cascades in ternary velocity fields

### B. Ternary Biology
- `ternary-morphogenesis-v2` — Turing patterns with continuous reaction-diffusion approximated in ternary
- `ternary-genetics` — DNA-like ternary sequences, transcription, translation
- `ternary-ecology` — predator-prey dynamics with ternary populations
- `ternary-immune` — immune system as ternary classifier (self/non-self/unknown)
- `ternary-membrane` — membrane transport with ternary gradient (in/out/equilibrium)

### C. Ternary Music Theory (Deep)
- `ternary-temperament` — tuning systems in Z₃ (equal temperament with 3 divisions)
- `ternary-cadence` — harmonic progressions and resolution patterns
- `ternary-modulation` — key changes in ternary tonality
- `ternary-counterpoint-v2` — second through fifth species counterpoint
- `ternary-harmony-v2` — chord theory with 3-note chords (triads are all you have)

### D. Ternary Network Science
- `ternary-pagerank` — PageRank algorithm over ternary-weighted graphs
- `ternary-community` — community detection in ternary networks
- `ternary-resilience` — network robustness analysis with ternary edge weights
- `ternary-diffusion-v2` — diffusion processes with ternary conductance
- `ternary-cascade-v2` — cascade detection and prediction

### E. Ternary Cryptography (Deep)
- `ternary-cipher-v2` — authenticated encryption, MACs, digital signatures over Z₃
- `ternary-zero-knowledge` — zero-knowledge proofs using ternary commitments
- `ternary-homomorphic` — homomorphic encryption over GF(3)
- `ternary-secret-sharing-v2` — verifiable secret sharing, proactive secret sharing

---

## III. THE META-QUESTION

**Why ternary?**

Binary is the language of computers. Continuous is the language of physics. Ternary sits between them — discrete enough to compute, rich enough to surprise. Every binary concept has a ternary analog, but the ternary version is *algebraically richer*:

- Binary XOR → ternary addition mod 3 (non-self-inverse)
- Binary entropy → ternary entropy (log₂3 ≈ 1.585 bits per symbol)
- Binary groups → ternary groups (Z₃ has invertible nonzero elements, Z₂ doesn't)
- Binary knots → ternary knots (virtual crossings are natural in Z₃)
- Binary music → ternary music (the tritone is the ONLY dissonance)

The fleet is not random. It's a *proof by construction* that ternary thinking reveals structure invisible to binary analysis. Every crate is a data point. Together, they form an argument.

**The argument:** Ternary systems are not merely "binary with an extra state." They are algebraically, topologically, and information-theoretically distinct. The fleet proves this by building the entire mathematical universe of ternary systems — from music to cryptography to physics to biology — and showing that each domain has ternary-specific phenomena that have no binary analog.

---

## IV. METRICS

| Metric | Count |
|--------|-------|
| Total repos | 234 |
| Rust crates | 215 |
| Tests | ~4,200 |
| Crates with See Also | 211 |
| Crates with "Deeper Truth" READMEs | 50+ |
| New crates this session | 10 (crystal, knot, cipher, sheaf, symmetry, vortex, epidemic, morphogenesis, renormalization, counterpoint) |
| New tests this session | 139 |
| Cross-pollination audit completed | ✅ |

---

## V. NEXT WAVE

Build these 6 next:
1. `ternary-critical` — Monte Carlo ternary Ising, critical temperature
2. `ternary-pagerank` — PageRank over ternary graphs
3. `ternary-quantum-v2` — qutrits, ternary entanglement, ternary CNOT
4. `ternary-homomorphic` — homomorphic encryption over GF(3)
5. `ternary-ecology` — Lotka-Volterra in ternary
6. `ternary-membrane` — membrane transport dynamics
