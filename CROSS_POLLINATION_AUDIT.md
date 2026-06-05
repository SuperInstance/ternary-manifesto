# Cross-Pollination Audit — SuperInstance Ternary Fleet

**Generated:** 2026-06-05  
**Fleet size:** 211 crates  
**Crates with any See Also links:** 76  
**Crates with zero See Also links:** 135  

---

## Methodology

1. Listed all `ternary-*` directories under `~/repos/`
2. Read the first 3 lines of each README.md to extract functionality descriptions
3. Grepped each README.md for "See Also" / "Related" sections, extracting all `ternary-*` references
4. Counted unique outbound links per crate (excluding self-references)
5. Grouped crates into thematic clusters by functionality
6. For each crate, identified thematically adjacent crates not currently linked
7. Ranked crates by isolation (fewest outbound links + most thematic relevance to unlinked neighbors)

---

## Thematic Clusters

### 🎵 Audio / Music
`bite`, `echo`, `envelope`, `grain`, `harmonic`, `loop`, `mixer`, `muse`, `music`, `pan`, `polyrhythm`, `rack`, `rhythm`, `sampler`, `tempo`, `wave`, `crossfader`, `gate`, `vu`, `needledrop`, `jam`, `ear`, `resonance`, `phase`

### 🧮 Grid / Cellular Automata
`life`, `collatz`, `sandpile`, `ising`, `percolation`, `minority`, `drift`, `fire`, `morph`, `field`, `lattice`, `irradiate`, `automata`, `shield`

### 🤖 Agent Coordination / Fleet
`bus`, `sync`, `speculate`, `predict`, `signaling`, `steward`, `room`, `consensus`, `trust`, `quorum`, `beacon`, `captain`, `channel`, `navigator`, `protocol`, `platoon`, `mesh`, `anchor`, `helm`, `voyage`, `constellation`, `harbor`, `reef`, `ensign`, `bridge`, `cargo`, `current`, `conduct`, `lighthouse`, `tidelight`, `cartograph`, `pilgrim`, `frontier`, `weather`, `observatory`, `event`

### 🧬 Evolution / Genetics
`ga`, `genome`, `fitness`, `evolution-advanced`, `popgen`, `swarm`, `symbiont`, `seed`, `gradient`, `curriculum`, `transfer`, `federated`, `ensemble`

### 🧠 Perception / AI
`attention`, `bayesian`, `cortex`, `predict`, `sensor`, `oracle`, `agent`, `classifier`, `explain`, `inference`, `som`, `reservoir`, `rl`, `language-model`, `kalman`, `prophet`

### 📐 Math / Complexity
`complexity`, `mutual-info`, `fib`, `kuramoto`, `entropy`, `ring`, `matrix`, `tensor`, `tuple`, `permutation`, `pca`, `projection`, `geometry`, `topology`, `codes`, `quantum`, `chaos`, `thermodynamics`, `energy`, `fuzzy`

### 💻 Compiler / Language / Data
`compiler`, `compiler-v2`, `compiler-optimizer`, `compiler-python`, `grammar`, `language`, `language-evolution`, `language-model`, `regex`, `diff`, `hash`, `steganography`, `codes`

### 🗃️ Storage / Infrastructure
`database`, `archive`, `memory`, `registry`, `registry-v2`, `compression`, `compression-v2`, `streaming`, `pipeline`, `benchmark`, `metrics`, `validation`, `replay`, `foundry`, `shipyard`, `dockyard`, `sandbox`, `locks`, `inventory`

### 🎮 Games / Decision Theory
`games`, `game-theory`, `auction`, `market`, `econ`, `voting`, `dice`, `pareto`, `scoring`, `arena`

### 📊 Visualization / Rendering
`visualization`, `visualizer`, `color`, `wave` (overlaps with audio)

### 🔧 Core / Low-Level
`hardware`, `esp32-firmware`, `cell`, `circuit`, `logic`, `wasm`, `cli`, `command`, `engine`, `signals`, `control`, `scheduling`, `scheduling-v2`, `depth`, `noise`, `transform`, `warp`, `world`, `ecosystem`, `dynamics`, `dynamics-python`, `failure`, `constraints`, `trees`, `markov`, `science`

### 🧪 Experiment / Research
`experiment`, `experiment-workers`, `cell-python`, `cell`, `dissertation-c`, `fitness-c`, `fitness-python`, `inference-c`, `spreadsheet`, `spreadsheet-c`, `spreadsheet-python`, `protocol-python`, `dynamics-python`

### 📋 Fleet Orchestration Patterns (nautical metaphors)
`anchor`, `beacon`, `bridge`, `captain`, `cargo`, `cartograph`, `compass`, `conduct`, `constellation`, `current`, `dockyard`, `ensign`, `flotilla`, `frontier`, `grace`, `harbor`, `helm`, `lighthouse`, `navigator`, `observatory`, `pilgrim`, `platoon`, `quorum`, `reef`, `rigging`, `shipyard`, `steward`, `tidelight`, `tidepool`, `voyage`

---

## Missing Links by Crate

### ternary-adversarial
**Function:** Adversarial testing for ternary agents — stress-testing strategies against worst-case environments.
**Current See Also:** (none)
**Missing:**
- ternary-arena — competitive multi-agent arena for adversarial testing
- ternary-agent — core agent types being stress-tested
- ternary-failure — failure analysis complements adversarial testing
- ternary-noise — noise tolerance testing is adversarial adjacent

### ternary-agent
**Function:** Core agent struct with ternary state (avoid/explore/choose), pools, memory, behavior tracking.
**Current See Also:** (none)
**Missing:**
- ternary-cortex — hierarchical processing built on top of agents
- ternary-room — rooms contain agents
- ternary-cell — cellular computing with agent-like tick cycles
- ternary-fitness — fitness landscapes evaluate agent strategies
- ternary-memory — memory systems for agents
- ternary-popgen — population-level agent dynamics

### ternary-anchor
**Function:** Stability and persistence — Anchor, AnchorChain, AnchorWatch for rooms.
**Current See Also:** (none)
**Missing:**
- ternary-room — anchors hold position in rooms
- ternary-harbor — harbor is the arrival point; anchor is the staying point
- ternary-drift — drift is the opposite of anchoring
- ternary-beacon — beacons announce presence; anchors maintain it
- ternary-moor (if exists) or ternary-current — currents challenge anchoring

### ternary-archive
**Function:** Append-only knowledge store — immutable scrolls indexed for fast lookup.
**Current See Also:** (none)
**Missing:**
- ternary-database — related persistent storage
- ternary-memory — memory systems for agents
- ternary-chronicle — chronological records are archives with narrative
- ternary-replay — replay depends on archived state
- ternary-compression — archived data benefits from compression

### ternary-arena
**Function:** Multi-agent competition arena for ternary systems.
**Current See Also:** (none)
**Missing:**
- ternary-adversarial — adversarial testing in arenas
- ternary-games — games are played in arenas
- ternary-game-theory — strategic reasoning in competitive settings
- ternary-scoring — scoring/ranking arena participants
- ternary-fitness — fitness evaluation often uses competitive arenas

### ternary-attention
**Function:** Scaled dot-product attention, multi-head attention, cross-attention on ternary sequences.
**Current See Also:** (none)
**Missing:**
- ternary-cortex — cortex uses attention mechanisms
- ternary-transform — attention is a transform
- ternary-language-model — language models use attention
- ternary-entropy — attention patterns relate to information content
- ternary-signals — signal processing parallels to attention

### ternary-auction
**Function:** Auction mechanisms with ternary bids.
**Current See Also:** (none)
**Missing:**
- ternary-market — auctions are market mechanisms
- ternary-econ — economic modeling context
- ternary-signaling — bids are signals
- ternary-game-theory — auction theory is game theory
- ternary-voting — voting and auctions are social choice mechanisms

### ternary-automata
**Function:** Cellular automata with ternary states — rules, simulation, pattern detection, entropy.
**Current See Also:** (none)
**Missing:**
- ternary-life — Conway's Game of Life is a specific CA
- ternary-fire — fire dynamics is a CA rule
- ternary-sandpile — sandpile is a CA
- ternary-collatz — Collatz is related to CA
- ternary-cell — cell uses CA-like tick cycles
- ternary-ising — Ising model runs on grids like CAs

### ternary-bayesian
**Function:** Bayesian inference for ternary variables — networks, belief propagation, variational inference.
**Current See Also:** (none)
**Missing:**
- ternary-predict — prediction uses Bayesian inference
- ternary-kalman — Kalman filtering is Bayesian
- ternary-prophet — forecasting with uncertainty
- ternary-oracle — prediction market with confidence
- ternary-markov — Markov chains relate to Bayesian networks

### ternary-beacon
**Function:** Discovery and presence protocol for fleet agents.
**Current See Also:** (none)
**Missing:**
- ternary-lighthouse — lighthouse observes; beacon announces
- ternary-protocol — beacon uses wire protocols
- ternary-room — beacons operate within rooms
- ternary-anchor — anchors maintain what beacons discover
- ternary-mesh — mesh networking uses beacons

### ternary-benchmark
**Function:** Standardized benchmarks for ternary agent systems.
**Current See Also:** (none)
**Missing:**
- ternary-metrics — benchmarks produce metrics
- ternary-gauge — gauges measure what benchmarks test
- ternary-experiment — experiments run benchmarks
- ternary-scoring — scoring ranks benchmark results
- ternary-fitness — fitness landscapes are benchmarked

### ternary-bridge
**Function:** Bridge pattern connecting heterogeneous ternary systems.
**Current See Also:** (none)
**Missing:**
- ternary-protocol — bridges use protocols
- ternary-channel — channels are bridges for messages
- ternary-mesh — mesh networks bridge agents
- ternary-flux — flux tracks what bridges carry
- ternary-constellation — constellations bridge groups of crates

### ternary-bus
**Function:** Pub/sub message bus with ternary payloads.
**Current See Also:** (none)
**Missing:**
- ternary-channel — channels are the comms backbone
- ternary-event — events travel on buses
- ternary-protocol — wire protocols underlie the bus
- ternary-room — rooms use buses for inter-room comms
- ternary-streaming — streaming is continuous bus traffic

### ternary-captain
**Function:** Captain/leadership pattern for fleet coordination.
**Current See Also:** (none)
**Missing:**
- ternary-consensus — consensus elects captains
- ternary-quorum — quorums validate captain decisions
- ternary-room — rooms have captains
- ternary-helm — captains give helm orders
- ternary-conduct — conductors coordinate like captains
- ternary-steward — stewards manage resources for captains

### ternary-cargo
**Function:** Resource transport and logistics between rooms.
**Current See Also:** (none)
**Missing:**
- ternary-room — cargo moves between rooms
- ternary-harbor — harbors receive cargo
- ternary-shipyard — shipyards build cargo carriers
- ternary-inventory — cargo is inventoried
- ternary-channel — channels carry cargo

### ternary-causality
**Function:** Causal inference — DAGs, do-calculus, counterfactuals.
**Current See Also:** (none)
**Missing:**
- ternary-bayesian — Bayesian networks are causal DAGs
- ternary-markov — Markov assumptions relate to causal structure
- ternary-predict — prediction needs causal models
- ternary-inference — inference from causal structure
- ternary-entropy — entropy measures relate to causal information

### ternary-cell
**Function:** Cellular computing with six-phase tick cycle, signaling, division, apoptosis.
**Current See Also:** (none)
**Missing:**
- ternary-automata — cells run CAs
- ternary-life — life is cells on a grid
- ternary-tissue — if exists, or ternary-grid
- ternary-ecosystem — cells form ecosystems
- ternary-genome — genomes encode cell behavior
- ternary-agent — cells are agent-like
- ternary-steward — stewardship at cellular level

### ternary-channel
**Function:** Communication channel abstractions for inter-room messaging.
**Current See Also:** (none)
**Missing:**
- ternary-bus — bus is the pub/sub layer
- ternary-protocol — protocols define channel behavior
- ternary-room — channels connect rooms
- ternary-signaling — signals travel channels
- ternary-event — events use channels

### ternary-chaos
**Function:** Chaos and nonlinear dynamics — Lyapunov exponents, bifurcation, strange attractors.
**Current See Also:** (none)
**Missing:**
- ternary-dynamics — dynamics is the parent field
- ternary-kuramoto — synchronization edge of chaos
- ternary-entropy — chaos relates to entropy
- ternary-ising — phase transitions at edge of chaos
- ternary-attractor — if exists, or ternary-resonance

### ternary-chronicle
**Function:** Historical record and narrative generation — timelines, pattern prediction.
**Current See Also:** (none)
**Missing:**
- ternary-archive — archives store chronicles
- ternary-epoch — epochs divide chronicles
- ternary-replay — replay uses chronicles
- ternary-event — events are chronicle entries
- ternary-memory — memory is internal chronicle

### ternary-circuit
**Function:** Three-valued logic gates, truth tables, circuit composition under Kleene/Łukasiewicz.
**Current See Also:** (none)
**Missing:**
- ternary-logic — logic systems define circuit semantics
- ternary-hardware — hardware implements circuits
- ternary-ring — ring arithmetic underpins circuits
- ternary-compiler — circuits compile to ternary ops
- ternary-quantum — quantum gates are circuit-like

### ternary-classifier
**Function:** Classifies agent behavior into strategy species.
**Current See Also:** (none)
**Missing:**
- ternary-clustering — clustering is unsupervised classification
- ternary-trees — decision trees classify
- ternary-bayesian — Bayesian classification
- ternary-som — SOMs classify by topology
- ternary-attention — attention patterns classify behavior

### ternary-cli
**Function:** Command-line interface for the ternary agent ecosystem.
**Current See Also:** (none)
**Missing:**
- ternary-engine — CLI runs the engine
- ternary-experiment — CLI runs experiments
- ternary-visualizer — CLI renders visualizations
- ternary-benchmark — CLI runs benchmarks
- ternary-compiler — CLI compiles strategies

### ternary-clustering
**Function:** Clustering algorithms for ternary-valued data vectors.
**Current See Also:** (none)
**Missing:**
- ternary-classifier — classification uses clustering
- ternary-som — SOMs are topology-preserving clustering
- ternary-pca — PCA reduces dimensions before clustering
- ternary-graph — graph clustering algorithms
- ternary-entropy — entropy guides cluster quality

### ternary-codes
**Function:** Error-correcting codes — Hamming, repetition, parity for ternary data.
**Current See Also:** (none)
**Missing:**
- ternary-hash — hashing and codes are information-theoretic
- ternary-ring — codes operate in ring/field structures
- ternary-compression — compression and coding are related
- ternary-noise — codes protect against noise
- ternary-failure — failure analysis uses error correction

### ternary-command
**Function:** Command parsing and dispatch with ternary outcomes.
**Current See Also:** (none)
**Missing:**
- ternary-cli — CLI uses command parsing
- ternary-grammar — grammar defines command syntax
- ternary-protocol — protocols serialize commands
- ternary-event — commands trigger events
- ternary-pipeline — commands flow through pipelines

### ternary-compass
**Function:** Orientation and direction in ternary state space.
**Current See Also:** (none)
**Missing:**
- ternary-navigator — navigation uses compass
- ternary-helm — helm follows compass direction
- ternary-cartograph — maps need compass orientation
- ternary-frontier — frontiers are found by compass
- ternary-geometry — geometric direction in ternary space

### ternary-compiler
**Function:** Compiles ternary strategies into optimized lookup tables.
**Current See Also:** (none)
**Missing:**
- ternary-compiler-v2 — next-gen compiler
- ternary-compiler-optimizer — optimizer passes
- ternary-grammar — grammar feeds the compiler
- ternary-vm — if exists, compiled code runs on VM
- ternary-engine — engine executes compiled code

### ternary-compiler-v2
**Function:** Compilation pipeline — IR, register allocation, trit-encoded bytecode, optimization.
**Current See Also:** (none)
**Missing:**
- ternary-compiler — original compiler
- ternary-compiler-optimizer — optimizer for compiler output
- ternary-grammar — grammar is compiler input
- ternary-hardware — hardware runs compiled code
- ternary-ring — ring arithmetic in compiled code

### ternary-complexity
**Function:** Kolmogorov complexity and compressibility for ternary sequences.
**Current See Also:** (none)
**Missing:**
- ternary-entropy — entropy measures complexity
- ternary-compression — compression exploits low complexity
- ternary-mutual-info — mutual information measures shared complexity
- ternary-collatz — Collatz has unknown complexity
- ternary-codes — code distance relates to complexity

### ternary-compression
**Function:** Compression algorithms — RLE, Huffman, dictionary for ternary sequences.
**Current See Also:** (none)
**Missing:**
- ternary-compression-v2 — next-gen compression
- ternary-complexity — complexity bounds compressibility
- ternary-entropy — entropy limits compression
- ternary-hash — hashing relates to compression
- ternary-archive — archives use compression

### ternary-compression-v2
**Function:** Multi-algorithm compression — RLE, Huffman, LZW, entropy coding.
**Current See Also:** (none)
**Missing:**
- ternary-compression — original compression crate
- ternary-entropy — entropy coding uses entropy measures
- ternary-tensor — tensors need compression
- ternary-streaming — streaming compression
- ternary-pca — PCA is a form of compression

### ternary-consensus
**Function:** Distributed consensus — Raft, BFT, majority/plurality/supermajority voting.
**Current See Also:** (none)
**Missing:**
- ternary-voting — voting is the mechanism of consensus
- ternary-quorum — quorums are consensus thresholds
- ternary-trust — trust affects consensus
- ternary-distributed — distributed systems need consensus
- ternary-petri — Petri nets model consensus protocols
- ternary-room — rooms reach consensus

### ternary-constraint
**Function:** Constraint satisfaction — AC-3, backtracking, ternary N-queens.
**Current See Also:** (none)
**Missing:**
- ternary-planning — planning is constrained optimization
- ternary-logic — logic defines constraints
- ternary-scheduling — scheduling under constraints
- ternary-validation — validation is constraint checking
- ternary-pareto — Pareto fronts are constraint boundaries

### ternary-control
**Function:** Control theory — PID, bang-bang, state machines, stability analysis.
**Current See Also:** (none)
**Missing:**
- ternary-dynamics — dynamics is what control controls
- ternary-robotics — robotics uses control theory
- ternary-kalman — Kalman filtering serves control
- ternary-helm — helm is fleet control
- ternary-chaos — chaotic systems resist control

### ternary-current
**Function:** Information flow and momentum through fleet topologies.
**Current See Also:** (none)
**Missing:**
- ternary-flux — flux tracks current flow
- ternary-channel — channels carry current
- ternary-room — rooms have currents
- ternary-network — network topology determines current
- ternary-mesh — mesh affects current flow

### ternary-curriculum
**Function:** Curriculum learning — progressively harder training environments.
**Current See Also:** (none)
**Missing:**
- ternary-rl — RL uses curriculum learning
- ternary-transfer — transfer learning complements curriculum
- ternary-fitness — fitness determines curriculum progression
- ternary-sandbox — sandboxes run curricula
- ternary-experiment — experiments test curricula

### ternary-database
**Function:** Storage, indexing, querying, transactions for ternary-valued fields.
**Current See Also:** (none)
**Missing:**
- ternary-archive — archive is a specialized database
- ternary-memory — memory is agent-internal database
- ternary-hash — hashing indexes databases
- ternary-compression — databases compress data
- ternary-tensor — tensors could be stored in databases

### ternary-depth
**Function:** Pressure modeling for nested ternary systems.
**Current See Also:** (none)
**Missing:**
- ternary-lattice — depth in lattice structures
- ternary-topology — topological depth
- ternary-nested (if exists)
- ternary-hierarchy — depth implies hierarchy
- ternary-world — nested worlds have depth

### ternary-dice
**Function:** Stochastic exploration with configurable randomness.
**Current See Also:** ternary-arena
**Missing:**
- ternary-noise — noise is stochastic
- ternary-chaos — chaos borders stochastic
- ternary-walk — random walks use dice
- ternary-experiment — experiments use randomization
- ternary-markov — Markov transitions are dice rolls

### ternary-diff
**Function:** Diff, patch, three-way merge for ternary sequences.
**Current See Also:** (none)
**Missing:**
- ternary-compression — diffs compress changes
- ternary-hash — hashing detects diffs
- ternary-tuple — tuples are diffed
- ternary-transform — transforms produce diffs
- ternary-grammar — grammar diffs parse trees

### ternary-distributed
**Function:** Distributed systems primitives — gossip, vector clocks, Paxos, partition detection.
**Current See Also:** ternary-clock, ternary-consensus, ternary-protocol, ternary-voting
**Missing:**
- ternary-mesh — mesh networking is distributed
- ternary-quorum — quorums in distributed systems
- ternary-failure — failure in distributed systems
- ternary-beacon — beacons discover distributed nodes

### ternary-dockyard
**Function:** Maintenance and repair — dry dock, diagnostics, refitting, salvage.
**Current See Also:** (none)
**Missing:**
- ternary-shipyard — shipyard builds; dockyard repairs
- ternary-harbor — harbors have dockyards
- ternary-failure — failure analysis for diagnostics
- ternary-steward — stewardship includes maintenance
- ternary-benchmark — benchmarks run diagnostics

### ternary-dynamics
**Function:** Ternary agent dynamics — time series, phase transitions, critical points.
**Current See Also:** (none)
**Missing:**
- ternary-dynamics-python — Python port
- ternary-chaos — chaos is nonlinear dynamics
- ternary-kuramoto — Kuramoto is synchronization dynamics
- ternary-epoch — epochs detect dynamic regime changes
- ternary-control — control manages dynamics
- ternary-thermodynamics — thermodynamics is statistical dynamics

### ternary-econ
**Function:** Economic models — portfolio, supply/demand, risk, market simulation.
**Current See Also:** (none)
**Missing:**
- ternary-market — markets are economic engines
- ternary-auction — auctions are economic mechanisms
- ternary-game-theory — game theory underpins economics
- ternary-scoring — scoring is economic valuation
- ternary-pareto — Pareto optimization is economic

### ternary-ecosystem
**Function:** Full ecosystem simulation — species, food webs, niches, succession.
**Current See Also:** (none)
**Missing:**
- ternary-cell — cells form ecosystems
- ternary-life — life is an ecosystem
- ternary-popgen — population genetics drives ecosystems
- ternary-evolution-advanced — evolution shapes ecosystems
- ternary-reef — reef is a specific ecosystem pattern

### ternary-energy
**Function:** Thermodynamic models — conservation, entropy, free energy, equilibrium.
**Current See Also:** (none)
**Missing:**
- ternary-thermodynamics — thermodynamics is the theory
- ternary-entropy — entropy is energy dispersal
- ternary-irradiate — irradiation is energy propagation
- ternary-fire — fire releases energy
- ternary-physics — if exists

### ternary-engine
**Function:** Unified platform core embodying what 11 experiments discovered.
**Current See Also:** (none)
**Missing:**
- ternary-experiment — engine runs experiments
- ternary-cli — CLI interfaces with engine
- ternary-wasm — WASM runs engine in browser
- ternary-compiler — compiler feeds engine
- ternary-world — engine runs worlds

### ternary-ensemble
**Function:** Ensemble methods — combine weak agents into strong ones.
**Current See Also:** (none)
**Missing:**
- ternary-classifier — ensembles classify
- ternary-trees — random forests are ensembles of trees
- ternary-federated — federated learning is distributed ensembles
- ternary-fitness — fitness evaluates ensemble members
- ternary-voting — voting is ensemble decision

### ternary-ensign
**Function:** Specialist agent pattern — domain registry, bridging.
**Current See Also:** (none)
**Missing:**
- ternary-agent — ensigns are specialized agents
- ternary-bridge — ensigns bridge domains
- ternary-registry — registry tracks ensigns
- ternary-room — rooms contain ensigns
- ternary-constellation — constellations group ensigns

### ternary-entropy
**Function:** Shannon entropy, conditional entropy, mutual information, KL divergence.
**Current See Also:** (none)
**Missing:**
- ternary-mutual-info — mutual information builds on entropy
- ternary-complexity — complexity is entropy-adjacent
- ternary-compression — compression exploits entropy structure
- ternary-chaos — chaos produces entropy
- ternary-epoch — epoch changes shift entropy

### ternary-envelope
**Function:** ADSR envelope shaping for ternary signals.
**Current See Also:** (none)
**Missing:**
- ternary-wave — envelopes shape waves
- ternary-gate — gates trigger envelopes
- ternary-rack — racks chain envelopes
- ternary-mixer — mixers blend envelopes
- ternary-echo — echoes have temporal envelopes

### ternary-esp32-firmware
**Function:** Running ternary decisions on ESP32 bare metal.
**Current See Also:** (none)
**Missing:**
- ternary-hardware — hardware abstraction
- ternary-sensor — sensors feed ESP32
- ternary-robotics — robotics uses embedded
- ternary-control — control on bare metal
- ternary-spreadsheet — spreadsheet on embedded

### ternary-event
**Function:** Pub/sub event dispatch with ternary priorities.
**Current See Also:** (none)
**Missing:**
- ternary-bus — buses carry events
- ternary-channel — channels deliver events
- ternary-streaming — streaming is continuous events
- ternary-chronicle — chronicles record events
- ternary-pipeline — pipelines process events

### ternary-evolution-advanced
**Function:** Advanced evolutionary algorithms — differential evolution, CMA-ES, NSGA-II.
**Current See Also:** (none)
**Missing:**
- ternary-ga — GA is the base; this is advanced
- ternary-genome — genomes are evolved
- ternary-fitness — fitness evaluates evolution
- ternary-gradient — gradient-free optimization overlaps
- ternary-seed — seeds initialize evolution

### ternary-explain
**Function:** Explainability for ternary agent decisions.
**Current See Also:** (none)
**Missing:**
- ternary-attention — attention is explainable
- ternary-classifier — classification needs explanation
- ternary-trees — trees are inherently explainable
- ternary-causality — causal explanation
- ternary-inference — inference traces explain

### ternary-federated
**Function:** Federated learning — multiple populations sharing insights without raw data.
**Current See Also:** (none)
**Missing:**
- ternary-distributed — federated is distributed
- ternary-ensemble — federated aggregates ensembles
- ternary-privacy — if exists
- ternary-transfer — transfer learning is related
- ternary-protocol — protocols enable federation

### ternary-fitness
**Function:** Fitness landscape analysis for ternary strategies.
**Current See Also:** (none)
**Missing:**
- ternary-ga — GAs optimize fitness
- ternary-genome — genomes encode fitness
- ternary-evolution-advanced — advanced evolution uses fitness
- ternary-popgen — population genetics is fitness-driven
- ternary-gradient — gradient on fitness landscapes

### ternary-flux
**Function:** Flux/state-flow engine for tracking ternary value propagation.
**Current See Also:** (none)
**Missing:**
- ternary-current — current is flux in fleet topology
- ternary-streaming — streaming is continuous flux
- ternary-pipeline — pipelines control flux
- ternary-channel — channels carry flux
- ternary-event — events cause flux

### ternary-frontier
**Function:** Exploration and discovery of unknown ternary state space.
**Current See Also:** (none)
**Missing:**
- ternary-navigator — navigation to frontiers
- ternary-compass — compass points to frontiers
- ternary-room — rooms have frontiers
- ternary-agent — agents explore frontiers
- ternary-search — search finds frontiers

### ternary-fuzzy
**Function:** Fuzzy logic — fuzzy sets, membership functions, inference rules.
**Current See Also:** (none)
**Missing:**
- ternary-logic — fuzzy extends ternary logic
- ternary-classifier — fuzzy classification
- ternary-control — fuzzy control systems
- ternary-entropy — fuzzy entropy measures
- ternary-bayesian — fuzzy Bayesian inference

### ternary-ga
**Function:** Genetic algorithm toolkit — selection, crossover, mutation for ternary genomes.
**Current See Also:** (none)
**Missing:**
- ternary-genome — GA operates on genomes
- ternary-fitness — fitness is GA's objective
- ternary-evolution-advanced — advanced evolution builds on GA
- ternary-popgen — population genetics is GA's theory
- ternary-gradient — gradient-free optimization is GA alternative

### ternary-game-theory
**Function:** Game theory — normal-form, Nash equilibrium, cooperative games.
**Current See Also:** (none)
**Missing:**
- ternary-games — games implements game theory
- ternary-auction — auctions are game-theoretic
- ternary-signaling — signaling games
- ternary-consensus — consensus is a game
- ternary-econ — economics uses game theory

### ternary-games
**Function:** Game theory for ternary agents — payoff matrices, Nash equilibria.
**Current See Also:** (none)
**Missing:**
- ternary-game-theory — game theory is the theory behind games
- ternary-arena — games are played in arenas
- ternary-scoring — scoring game outcomes
- ternary-voting — voting is a game
- ternary-dice — dice add randomness to games

### ternary-genome
**Function:** Genetic encoding — genome, chromosome, gene, mutation, crossover.
**Current See Also:** (none)
**Missing:**
- ternary-ga — GA operates on genomes
- ternary-fitness — fitness evaluates genomes
- ternary-popgen — population genetics studies genomes
- ternary-evolution-advanced — advanced evolution mutates genomes
- ternary-cell — cells express genomes

### ternary-geometry
**Function:** Geometric algorithms — distances, Voronoi, convex hulls on ternary grids.
**Current See Also:** (none)
**Missing:**
- ternary-topology — topology is abstract geometry
- ternary-field — field calculus uses geometry
- ternary-projection — projections are geometric
- ternary-morph — morphology is geometric
- ternary-compass — compass is geometric direction

### ternary-gradient
**Function:** Gradient-free/gradient-like optimization — coordinate descent, SA, hill climbing.
**Current See Also:** (none)
**Missing:**
- ternary-fitness — fitness landscapes have gradients
- ternary-ga — GA is gradient-free optimization
- ternary-control — control follows gradients
- ternary-rl — RL uses gradient-like updates
- ternary-field — fields have gradients

### ternary-grain
**Function:** Granular synthesis — fragment, window, scatter ternary streams.
**Current See Also:** (none)
**Missing:**
- ternary-sampler — sampling is granular
- ternary-wave — grains recombine into waves
- ternary-loop — loops repeat grains
- ternary-echo — echoes are delayed grains
- ternary-rack — rack chains grain processors

### ternary-grammar
**Function:** CFG parser for ternary strategy expressions — recursive descent, AST, evaluator.
**Current See Also:** (none)
**Missing:**
- ternary-compiler — grammar feeds the compiler
- ternary-language — language processing uses grammar
- ternary-regex — regex is grammar-based
- ternary-command — commands have grammar
- ternary-regex — regex is a grammar subclass

### ternary-harbor
**Function:** Harbor pattern — agent docking, berths, pilot assistance.
**Current See Also:** (none)
**Missing:**
- ternary-room — rooms have harbors
- ternary-anchor — anchors hold in harbors
- ternary-cargo — cargo arrives at harbors
- ternary-dockyard — dockyards are in harbors
- ternary-shipyard — ships leave from harbors

### ternary-hardware
**Function:** HAL for balanced ternary — trits, trytes, registers, ALU on {-1, 0, +1}.
**Current See Also:** (none)
**Missing:**
- ternary-circuit — circuits are hardware components
- ternary-esp32-firmware — firmware runs on hardware
- ternary-ring — ring arithmetic in hardware
- ternary-compiler-v2 — compiler targets hardware
- ternary-quantum — quantum hardware analogs

### ternary-hash
**Function:** Hashing, fingerprinting, MinHash, Bloom filters, LSH for ternary data.
**Current See Also:** (none)
**Missing:**
- ternary-codes — codes and hash are information-theoretic
- ternary-diff — diffs use hashing
- ternary-compression — compression uses hashing
- ternary-database — databases index with hashes
- ternary-steganography — steganography hides in hashes

### ternary-helm
**Function:** Steering and control — Helm, Rudder, Autopilot for fleet navigation.
**Current See Also:** (none)
**Missing:**
- ternary-captain — captains issue helm orders
- ternary-compass — compass guides helm
- ternary-navigator — navigator uses helm
- ternary-control — control theory for steering
- ternary-room — rooms have helms

### ternary-inference
**Function:** Inference from ternary negative spaces — deducing from absences.
**Current See Also:** (none)
**Missing:**
- ternary-bayesian — Bayesian inference
- ternary-predict — prediction uses inference
- ternary-explain — explainability needs inference traces
- ternary-causality — causal inference
- ternary-oracle — oracles perform inference

### ternary-kalman
**Function:** Kalman filtering for ternary state spaces with fixed-point arithmetic.
**Current See Also:** (none)
**Missing:**
- ternary-bayesian — Kalman is Bayesian filtering
- ternary-sensor — sensors feed Kalman filters
- ternary-predict — Kalman filters predict state
- ternary-control — control uses Kalman estimates
- ternary-robotics — robotics uses Kalman for localization

### ternary-language-evolution
**Function:** How communication protocols evolve over time.
**Current See Also:** (none)
**Missing:**
- ternary-language — language is what evolves
- ternary-grammar — grammar evolves
- ternary-signaling — signaling is language evolution
- ternary-genome — genomes encode language
- ternary-protocol — protocols are evolved languages

### ternary-language-model
**Function:** N-gram language modeling with ternary tokens.
**Current See Also:** (none)
**Missing:**
- ternary-language — language processing
- ternary-markov — N-grams are Markov chains
- ternary-attention — attention in language models
- ternary-entropy — entropy of language models
- ternary-grammar — grammar constrains language models

### ternary-language
**Function:** Language and grammar processing — tokenization, sentiment, parsing, Markov chains.
**Current See Also:** (none)
**Missing:**
- ternary-grammar — grammar defines language
- ternary-language-model — language models predict language
- ternary-language-evolution — language evolves
- ternary-regex — regex matches language patterns
- ternary-compiler — compilers parse language

### ternary-lattice
**Function:** Lattice structures — partial orders, semilattice operations, morphisms.
**Current See Also:** (none)
**Missing:**
- ternary-logic — logic has lattice structure
- ternary-ring — rings and lattices are algebraic
- ternary-topology — topology on lattices
- ternary-field — fields on lattice grids
- ternary-morph — morphology operates on lattices

### ternary-locks
**Function:** Lock algebra — constraint composition, dependency graphs, critical mass.
**Current See Also:** (none)
**Missing:**
- ternary-constraint — constraints are locks
- ternary-scheduling — scheduling uses locks
- ternary-validation — validation locks patterns
- ternary-planning — planning resolves locks
- ternary-dependency — if exists

### ternary-logic
**Function:** Advanced ternary logic — Kleene, Łukasiewicz, Bochvar, Gödel-Dummett.
**Current See Also:** (none)
**Missing:**
- ternary-circuit — circuits implement logic
- ternary-fuzzy — fuzzy extends ternary logic
- ternary-lattice — lattices structure logic
- ternary-ring — ring arithmetic for logic values
- ternary-hardware — hardware implements logic

### ternary-market
**Function:** Market engine — order books, price discovery, auctions, market making.
**Current See Also:** (none)
**Missing:**
- ternary-econ — economics models markets
- ternary-auction — auctions are market mechanisms
- ternary-game-theory — market is a game
- ternary-scoring — scoring market performance
- ternary-trust — trust affects market participation

### ternary-markov
**Function:** Markov chains — transition matrices, stationary distributions, mixing.
**Current See Also:** (none)
**Missing:**
- ternary-language-model — N-grams are Markov
- ternary-walk — random walks are Markov chains
- ternary-chaos — chaos relates to Markov
- ternary-entropy — Markov entropy rates
- ternary-predict — Markov chains predict

### ternary-matrix
**Function:** Compact ternary matrix — 2-bit packed, GF(3) inverse, eigenvalue estimation.
**Current See Also:** (none)
**Missing:**
- ternary-tensor — tensors generalize matrices
- ternary-ring — matrix algebra over rings
- ternary-tuple — tuples are matrix row/columns
- ternary-pca — PCA uses matrix decomposition
- ternary-network — adjacency matrices

### ternary-memory
**Function:** Memory systems — short-term, long-term, episodic for agents.
**Current See Also:** (none)
**Missing:**
- ternary-agent — agents have memory
- ternary-archive — external memory
- ternary-database — database as memory store
- ternary-replay — replay from memory
- ternary-chronicle — chronicle is narrative memory

### ternary-mesh
**Function:** Dynamic mesh networking between agents.
**Current See Also:** (none)
**Missing:**
- ternary-network — mesh is a network topology
- ternary-beacon — beacons discover mesh nodes
- ternary-channel — channels in mesh
- ternary-distributed — mesh is distributed
- ternary-current — current flows through mesh

### ternary-metrics
**Function:** Time-series metrics — latency, throughput, accuracy, reporting.
**Current See Also:** (none)
**Missing:**
- ternary-gauge — gauges display metrics
- ternary-benchmark — benchmarks produce metrics
- ternary-lighthouse — lighthouse collects metrics
- ternary-observatory — observatory watches metrics
- ternary-vu — VU meters display metrics

### ternary-mixer
**Function:** Multi-channel ternary mixer — gain, pan, EQ, bus routing.
**Current See Also:** (none)
**Missing:**
- ternary-wave — mixers combine waves
- ternary-pan — pan is mixer channel positioning
- ternary-crossfader — crossfader is a mixer
- ternary-rack — racks hold mixers
- ternary-envelope — envelopes shape mixer levels

### ternary-navigator
**Function:** Wayfinding and pathfinding using ternary-weighted graph traversal.
**Current See Also:** (none)
**Missing:**
- ternary-compass — compass orients navigation
- ternary-helm — helm steers navigation
- ternary-room — rooms are navigation nodes
- ternary-graph — graph algorithms for navigation
- ternary-frontier — frontiers are navigation targets

### ternary-network
**Function:** Network science — shortest paths, clustering, centrality, community detection.
**Current See Also:** (none)
**Missing:**
- ternary-graph — graphs are network structure
- ternary-mesh — mesh is network topology
- ternary-topology — topology of networks
- ternary-petri — Petri nets are networks
- ternary-current — current flows in networks

### ternary-noise
**Function:** Effect of noise on ternary agent systems.
**Current See Also:** (none)
**Missing:**
- ternary-chaos — chaos vs. noise
- ternary-codes — codes resist noise
- ternary-sensor — sensors have noise
- ternary-dice — dice add noise
- ternary-walk — noisy walks

### ternary-observatory
**Function:** Long-range observation and forecasting of room states.
**Current See Also:** (none)
**Missing:**
- ternary-lighthouse — lighthouse observes
- ternary-gauge — gauges in observatories
- ternary-metrics — metrics feed observatories
- ternary-weather — weather is observed
- ternary-prophet — prophets forecast from observatories

### ternary-oracle
**Function:** Prediction market for fleet intelligence with confidence staking.
**Current See Also:** (none)
**Missing:**
- ternary-predict — prediction is oracle's purpose
- ternary-prophet — prophets are oracles
- ternary-bayesian — Bayesian prediction
- ternary-trust — trust in oracle predictions
- ternary-market — prediction markets

### ternary-pareto
**Function:** Pareto optimization — multi-objective strategies.
**Current See Also:** (none)
**Missing:**
- ternary-scoring — scoring finds Pareto fronts
- ternary-econ — economic Pareto efficiency
- ternary-game-theory — Pareto in game theory
- ternary-fitness — fitness is multi-objective
- ternary-evolution-advanced — NSGA-II finds Pareto fronts

### ternary-pipeline
**Function:** Composable data processing — filter, transform, aggregate, sort.
**Current See Also:** (none)
**Missing:**
- ternary-streaming — streaming through pipelines
- ternary-flux — flux through pipelines
- ternary-event — events flow in pipelines
- ternary-transform — transforms are pipeline stages
- ternary-channel — channels connect pipelines

### ternary-planning
**Function:** Planning and scheduling with ternary priorities.
**Current See Also:** (none)
**Missing:**
- ternary-scheduling — scheduling implements plans
- ternary-constraint — plans have constraints
- ternary-rl — RL learns plans
- ternary-search — search finds plans
- ternary-voyage — voyage is a long-term plan

### ternary-platoon
**Function:** Group formation and coordinated movement for agents.
**Current See Also:** (none)
**Missing:**
- ternary-swarm — swarms are platoons
- ternary-room — rooms contain platoons
- ternary-sync — platoons need synchronization
- ternary-mesh — mesh connects platoon members
- ternary-motion — platoon movement

### ternary-projection
**Function:** Dimensionality reduction for ternary data.
**Current See Also:** (none)
**Missing:**
- ternary-pca — PCA is a projection method
- ternary-visualization — visualization uses projections
- ternary-geometry — projections are geometric
- ternary-tensor — tensors project
- ternary-topology — topology of projections

### ternary-prophet
**Function:** Prediction and forecasting with uncertainty — trends, seasonality, ensembles.
**Current See Also:** (none)
**Missing:**
- ternary-predict — prediction is prophet's job
- ternary-oracle — oracle is the prediction mechanism
- ternary-bayesian — Bayesian forecasting
- ternary-kalman — Kalman for state forecasting
- ternary-epoch — epoch detection aids forecasting

### ternary-protocol
**Function:** Wire protocol — message passing, serialization, synchronization.
**Current See Also:** (none)
**Missing:**
- ternary-channel — channels use protocols
- ternary-bus — bus uses protocol
- ternary-distributed — distributed uses protocol
- ternary-bridge — bridges use protocol
- ternary-beacon — beacon uses protocol

### ternary-quantum
**Function:** Qutrits, Pauli operators, gates, entanglement, QFT over Z/3Z.
**Current See Also:** (none)
**Missing:**
- ternary-ring — ring arithmetic for qutrits
- ternary-circuit — quantum circuits
- ternary-tensor — tensor products for entanglement
- ternary-hardware — hardware analogs of quantum
- ternary-matrix — unitary matrices

### ternary-quorum
**Function:** Distributed decision making with ternary voting and thresholds.
**Current See Also:** (none)
**Missing:**
- ternary-consensus — consensus needs quorums
- ternary-voting — voting forms quorums
- ternary-trust — trust affects quorum
- ternary-distributed — distributed quorums
- ternary-room — rooms reach quorums

### ternary-rack
**Function:** Modular signal routing — pedalboard metaphor for ternary processing chains.
**Current See Also:** (none)
**Missing:**
- ternary-wave — racks process waves
- ternary-mixer — mixer is a rack module
- ternary-envelope — envelope module
- ternary-bite — bite effect in rack
- ternary-patch — if exists

### ternary-reef
**Function:** Coral reef ecosystem — persistent structures, slow growth, collective intelligence.
**Current See Also:** (none)
**Missing:**
- ternary-ecosystem — reef is an ecosystem
- ternary-constellation — constellation groups like reef
- ternary-room — rooms as reef structures
- ternary-trust — trust builds slowly like coral
- ternary-chronicle — reefs are long-lived chronicles

### ternary-regex
**Function:** Pattern matching on ternary sequences — NFA, DFA, minimization.
**Current See Also:** (none)
**Missing:**
- ternary-grammar — grammar defines regex patterns
- ternary-language — language processing uses regex
- ternary-automata — automata are regex engines
- ternary-search — search uses regex
- ternary-hash — hashing and pattern matching

### ternary-registry
**Function:** Capability and skill registry — versioning, dependency resolution.
**Current See Also:** (none)
**Missing:**
- ternary-registry-v2 — next-gen registry
- ternary-room — rooms have registries
- ternary-ensign — ensigns register capabilities
- ternary-constellation — constellations use registries
- ternary-protocol — protocol for registry sync

### ternary-replay
**Function:** Deterministic recording and replay of ternary experiments.
**Current See Also:** (none)
**Missing:**
- ternary-experiment — replay experiments
- ternary-archive — archive stores replays
- ternary-chronicle — chronicle records replays
- ternary-validation — validate via replay
- ternary-sandbox — sandbox replays

### ternary-robotics
**Function:** Robotics control — ternary actuators, differential drive, BFS path planning.
**Current See Also:** (none)
**Missing:**
- ternary-control — control for robots
- ternary-sensor — sensors on robots
- ternary-kalman — Kalman for robot localization
- ternary-esp32-firmware — embedded robot firmware
- ternary-motion — robot motion

### ternary-room
**Function:** Room abstraction — agents, environment state, doors with ternary access.
**Current See Also:** (none)
**Missing:**
- ternary-agent — agents live in rooms
- ternary-channel — channels connect rooms
- ternary-bus — bus between rooms
- ternary-navigator — navigate between rooms
- ternary-consensus — rooms reach consensus

### ternary-sampler
**Function:** Sampling and triggering ternary patterns — statistical sampling strategies.
**Current See Also:** (none)
**Missing:**
- ternary-wave — sampled waves
- ternary-grain — granular sampling
- ternary-loop — loops repeat samples
- ternary-rack — rack holds samplers
- ternary-needledrop — needledrop is a sampler type

### ternary-sandbox
**Function:** Safe sandbox for ternary experiments — environments, seeds, result capture.
**Current See Also:** (none)
**Missing:**
- ternary-experiment — experiments run in sandboxes
- ternary-tidepool — tidepool is a sandbox
- ternary-validation — validate in sandbox
- ternary-benchmark — benchmark in sandbox
- ternary-curriculum — curriculum in sandbox

### ternary-scheduling
**Function:** Priority scheduling — queues, deadline-aware, round-robin with ternary signals.
**Current See Also:** (none)
**Missing:**
- ternary-scheduling-v2 — next-gen scheduling
- ternary-planning — plans need scheduling
- ternary-constraint — constraints on scheduling
- ternary-locks — locks in scheduling
- ternary-pipeline — pipeline scheduling

### ternary-science
**Function:** Negative Space Intelligence — Experimental Evidence.
**Current See Also:** (none)
**Missing:**
- ternary-inference — inference from negative spaces
- ternary-dissertation-c — dissertation on negative space
- ternary-engine — engine embodies science
- ternary-entropy — entropy of negative space
- ternary-explain — explaining negative space

### ternary-scoring
**Function:** Multi-criteria scoring and ranking — weighted, Pareto, min-max normalization.
**Current See Also:** (none)
**Missing:**
- ternary-pareto — Pareto scoring
- ternary-fitness — fitness is scoring
- ternary-benchmark — benchmark scoring
- ternary-game-theory — game payoff scoring
- ternary-voting — voting is a score

### ternary-search
**Function:** Graph search — BFS, DFS, A*, beam search over ternary strategy spaces.
**Current See Also:** (none)
**Missing:**
- ternary-graph — search on graphs
- ternary-navigator — navigation is search
- ternary-planning — planning uses search
- ternary-rl — RL searches strategy space
- ternary-frontier — frontier is search boundary

### ternary-seed
**Function:** Seeded-Model-Programming (SMP) foundation for inference.
**Current See Also:** ternary-evolution-advanced, ternary-fitness, ternary-hash, ternary-inference
**Missing:**
- ternary-genome — seeds grow into genomes
- ternary-ga — GA starts from seeds
- ternary-sandbox — sandboxes run from seeds
- ternary-experiment — experiments use seeds
- ternary-world — worlds start from seeds

### ternary-sensor
**Function:** Sensor data processing — classification, fusion, anomaly detection, calibration.
**Current See Also:** (none)
**Missing:**
- ternary-predict — prediction from sensors
- ternary-kalman — Kalman filters sensor data
- ternary-robotics — robots use sensors
- ternary-weather — weather from sensors
- ternary-noise — sensor noise

### ternary-shipyard
**Function:** Construction from declarative blueprints.
**Current See Also:** (none)
**Missing:**
- ternary-dockyard — dockyard repairs what shipyard builds
- ternary-harbor — harbor receives from shipyard
- ternary-constellation — constellation is a blueprint
- ternary-foundry — foundry forges like shipyard builds
- ternary-cargo — cargo ships from shipyard

### ternary-signaling
**Function:** Signaling games on ternary channel — honesty, deception, costly signals.
**Current See Also:** ternary-auction, ternary-bus, ternary-consensus, ternary-signaling, ternary-trust
**Missing:**
- ternary-game-theory — signaling is game theory
- ternary-language-evolution — language evolves via signaling
- ternary-channel — signals travel channels
- ternary-protocol — protocols encode signals
- ternary-markov — Markov signaling

### ternary-signals
**Function:** Signal processing — DFT, autocorrelation, spectral density, frequency detection.
**Current See Also:** (none)
**Missing:**
- ternary-wave — signals are waves
- ternary-noise — noise in signals
- ternary-transform — transforms process signals
- ternary-entropy — entropy of signals
- ternary-streaming — streaming signals

### ternary-som
**Function:** Self-organizing maps — competitive learning, ternary distance, U-matrix.
**Current See Also:** (none)
**Missing:**
- ternary-clustering — SOMs cluster
- ternary-classifier — SOMs classify
- ternary-pca — PCA and SOMs both reduce dimensions
- ternary-topology — SOMs preserve topology
- ternary-visualization — SOM U-matrix visualization

### ternary-spreadsheet
**Function:** Spreadsheet where every cell is a tiny ternary intelligence.
**Current See Also:** (none)
**Missing:**
- ternary-spreadsheet-c — C port
- ternary-spreadsheet-python — Python port
- ternary-wasm — WASM runs spreadsheet in browser
- ternary-cell — cells are the unit
- ternary-formula — if exists

### ternary-steganography
**Function:** Hide and extract data in ternary signals — embedding, spread-spectrum.
**Current See Also:** (none)
**Missing:**
- ternary-hash — hashing detects steganography
- ternary-noise — steganography hides in noise
- ternary-signals — signal processing for stego
- ternary-compression — compression interacts with stego
- ternary-codes — codes for steganographic encoding

### ternary-streaming
**Function:** Streaming processing — sliding windows, running statistics, pattern detection.
**Current See Also:** (none)
**Missing:**
- ternary-signals — streaming signals
- ternary-pipeline — pipeline for streams
- ternary-event — streaming events
- ternary-flux — flux of streams
- ternary-window — if exists

### ternary-swarm
**Function:** Swarm intelligence — PSO, ant colony, flocking on ternary grid.
**Current See Also:** (none)
**Missing:**
- ternary-ga — GA and swarm are evolutionary
- ternary-platoon — platoon is coordinated swarm
- ternary-fitness — fitness evaluates swarm
- ternary-grad (if exists) or ternary-gradient — gradient-guided swarms
- ternary-ecosystem — swarm in ecosystem

### ternary-tenforward
**Function:** Conversation engine — multiple AI agents in cyclic dialogue with RPS dynamics.
**Current See Also:** (none)
**Missing:**
- ternary-jam — jam sessions are conversations
- ternary-sync — sync in conversations
- ternary-game-theory — RPS is game theory
- ternary-room — rooms host conversations
- ternary-bus — conversations on bus

### ternary-thermodynamics
**Function:** Statistical mechanics analogs for ternary agent systems.
**Current See Also:** (none)
**Missing:**
- ternary-energy — energy in thermodynamic context
- ternary-entropy — entropy is thermodynamic
- ternary-chaos — chaos at thermodynamic limits
- ternary-complexity — complexity and thermodynamics
- ternary-ising — Ising model is statistical mechanics

### ternary-tidelight
**Function:** Temporal rhythm and timing coordination across fleet.
**Current See Also:** (none)
**Missing:**
- ternary-tempo — tempo is tidal rhythm
- ternary-conduct — conductor sets tidelight
- ternary-sync — sync with tidal timing
- ternary-rhythm — rhythm of tides
- ternary-epoch — epochs like tidal cycles

### ternary-tidepool
**Function:** Small protected environments for agent experimentation.
**Current See Also:** (none)
**Missing:**
- ternary-sandbox — sandbox is a tidepool
- ternary-experiment — experiments in tidepools
- ternary-room — tidepool is a small room
- ternary-curriculum — curricula in tidepools
- ternary-reef — reef surrounds tidepool

### ternary-topology
**Function:** Topological analysis — connectedness, holes, boundaries, invariants.
**Current See Also:** (none)
**Missing:**
- ternary-graph — graphs have topology
- ternary-network — network topology
- ternary-geometry — geometry and topology
- ternary-som — SOMs preserve topology
- ternary-mesh — mesh topology

### ternary-transfer
**Function:** Transfer learning — knowledge from one environment to another.
**Current See Also:** (none)
**Missing:**
- ternary-curriculum — curriculum enables transfer
- ternary-federated — federated transfers knowledge
- ternary-fitness — fitness transfer between landscapes
- ternary-rl — RL uses transfer
- ternary-ensemble — ensemble transfers knowledge

### ternary-transform
**Function:** Signal transformations — shift, scale, invert, permute, convolve.
**Current See Also:** ternary-bite, ternary-echo, ternary-filter, ternary-mixer, ternary-transform, ternary-warp
**Missing:**
- ternary-signals — signals are transformed
- ternary-wave — wave transforms
- ternary-tensor — tensor transforms
- ternary-entropy — entropy of transforms
- ternary-projection — projection is a transform

### ternary-trees
**Function:** Decision trees and random forests — ternary splits, pruning, Gini impurity.
**Current See Also:** (none)
**Missing:**
- ternary-classifier — trees classify
- ternary-ensemble — forests are ensembles of trees
- ternary-entropy — entropy for tree splits
- ternary-explain — trees are explainable
- ternary-gradient — gradient boosting uses trees

### ternary-trust
**Function:** Bidirectional trust scores — five stages from Hostile to Family.
**Current See Also:** (none)
**Missing:**
- ternary-consensus — consensus requires trust
- ternary-signaling — signaling builds trust
- ternary-reputation — if exists
- ternary-quorum — quorums depend on trust
- ternary-reef — reefs build slow trust

### ternary-tuple
**Function:** Fixed-length ternary vectors — Hamming distance, correlation, algebra.
**Current See Also:** ternary-diff, ternary-matrix, ternary-mutual-info, ternary-permutation, ternary-tuple
**Missing:**
- ternary-tensor — tensors are multi-dimensional tuples
- ternary-hash — hash tuples
- ternary-codes — code distance on tuples
- ternary-geometry — geometric distance on tuples
- ternary-clustering — clustering uses tuple distances

### ternary-validation
**Function:** Rule-based validation of ternary strategies — bounds, conservation, diversity.
**Current See Also:** (none)
**Missing:**
- ternary-constraint — constraints validate
- ternary-locks — locks are validated patterns
- ternary-logic — logical validation
- ternary-sandbox — sandbox validates
- ternary-replay — replay validates determinism

### ternary-visualization
**Function:** ASCII art, SVG heatmaps, scatter plots, ternary triangle diagrams.
**Current See Also:** (none)
**Missing:**
- ternary-visualizer — visualizer is ASCII-focused
- ternary-color — color for visualization
- ternary-pca — PCA results need visualization
- ternary-graph — graph visualization
- ternary-som — SOM U-matrix visualization

### ternary-voting
**Function:** Voting and consensus — for (+1), against (−1), abstain (0).
**Current See Also:** (none)
**Missing:**
- ternary-consensus — consensus through voting
- ternary-quorum — quorum for valid vote
- ternary-game-theory — voting is a game
- ternary-scoring — voting scores candidates
- ternary-trust — trust affects votes

### ternary-voyage
**Function:** Long-duration mission planning with ternary progress tracking.
**Current See Also:** (none)
**Missing:**
- ternary-navigator — navigate the voyage
- ternary-helm — steer the voyage
- ternary-room — rooms are voyage waypoints
- ternary-chronicle — chronicle records voyage
- ternary-planning — plan the voyage

### ternary-wasm
**Function:** Ternary agent system compiled to WebAssembly.
**Current See Also:** (none)
**Missing:**
- ternary-engine — engine compiled to WASM
- ternary-spreadsheet — spreadsheet runs on WASM
- ternary-compiler-v2 — compiler targets WASM
- ternary-cli — CLI vs WASM runtime
- ternary-visualization — browser visualization

### ternary-world
**Function:** Grid world model — conservation laws, discrete time, observer.
**Current See Also:** (none)
**Missing:**
- ternary-life — life is a world simulation
- ternary-experiment — experiments run worlds
- ternary-sandbox — sandbox holds a world
- ternary-ecosystem — ecosystem in a world
- ternary-engine — engine runs worlds

---

## Top 20 Most Isolated Crates

Ranked by: zero See Also links × high thematic relevance to multiple unlinked neighbors.

| Rank | Crate | Cluster | Should Link To (top 5) |
|------|-------|---------|----------------------|
| 1 | **ternary-agent** | Agent/Core | cortex, room, fitness, memory, cell |
| 2 | **ternary-room** | Fleet/Core | agent, channel, bus, navigator, consensus |
| 3 | **ternary-consensus** | Agent Coord | voting, quorum, trust, distributed, petri |
| 4 | **ternary-circuit** | Core/Low-Level | logic, hardware, ring, compiler, quantum |
| 5 | **ternary-genome** | Evolution | ga, fitness, popgen, evolution-advanced, cell |
| 6 | **ternary-logic** | Math | circuit, fuzzy, lattice, ring, hardware |
| 7 | **ternary-hardware** | Core/Low-Level | circuit, esp32-firmware, ring, compiler-v2, quantum |
| 8 | **ternary-fitness** | Evolution | ga, genome, popgen, evolution-advanced, gradient |
| 9 | **ternary-bayesian** | Perception/AI | predict, kalman, prophet, oracle, markov |
| 10 | **ternary-memory** | Storage | agent, archive, database, replay, chronicle |
| 11 | **ternary-kalman** | Perception/AI | bayesian, sensor, predict, control, robotics |
| 12 | **ternary-network** | Math/Infra | graph, mesh, topology, petri, current |
| 13 | **ternary-database** | Storage | archive, memory, hash, compression, tensor |
| 14 | **ternary-topology** | Math | graph, network, geometry, mesh, som |
| 15 | **ternary-market** | Games/Econ | econ, auction, game-theory, scoring, trust |
| 16 | **ternary-robotics** | Perception | control, sensor, kalman, esp32-firmware, motion |
| 17 | **ternary-chaos** | Math | dynamics, kuramoto, entropy, ising, thermodynamics |
| 18 | **ternary-energy** | Math | thermodynamics, entropy, irradiate, fire, ising |
| 19 | **ternary-thermodynamics** | Math | energy, entropy, chaos, complexity, ising |
| 20 | **ternary-archive** | Storage | database, memory, chronicle, replay, compression |

---

## Summary Statistics

| Metric | Count |
|--------|-------|
| Total crates | 211 |
| Crates with any See Also | 76 |
| Crates with 0 See Also | 135 |
| Crates with only self-references | ~15 |
| Median outbound links (non-zero) | 5 |
| Max outbound links | 8 (failure, jam, life, muse, music, rhythm, wave) |
| Audio/Music cluster cross-links | Strong (well-connected internally) |
| Grid/CA cluster cross-links | Strong (well-connected internally) |
| Fleet/Coordination cluster cross-links | Weak (mostly 0 links) |
| Math/Complexity cluster cross-links | Weak (mostly 0 links) |
| Storage/Infrastructure cluster cross-links | Weak (mostly 0 links) |

## Key Findings

1. **The audio/music cluster is the best-connected subgraph** — bite, echo, wave, rack, and harmonic form a dense mesh of cross-references. This is the gold standard for the fleet.

2. **The Grid/CA cluster is second-best** — life, fire, sandpile, ising, percolation, and drift form a solid network.

3. **Fleet orchestration crates are severely isolated** — the nautical metaphor crates (anchor, beacon, captain, cargo, compass, harbor, helm, etc.) form a conceptual cluster with almost zero cross-links between them.

4. **Core infrastructure crates are the most under-linked** — agent, room, consensus, protocol, and memory are foundational crates that should be referenced by dozens of others but currently reference nothing.

5. **The compiler/language stack is internally disconnected** — compiler, compiler-v2, compiler-optimizer, grammar, and language all operate on the same domain but don't reference each other.

6. **Math crates form isolated silos** — ring, matrix, tensor, lattice, topology, and geometry are deeply related algebraically but share no cross-links.

7. **About 64% of the fleet has zero See Also sections** — the single highest-impact improvement would be adding See Also to these 135 crates.

---

## Recommendations

1. **Priority 1:** Add See Also to the top 20 most isolated crates (table above). These are foundational and should link outward extensively.

2. **Priority 2:** Complete the Fleet Orchestration cluster — the nautical metaphor crates should all reference each other.

3. **Priority 3:** Bridge the Math cluster — ring → matrix → tensor → topology → geometry should form a chain.

4. **Priority 4:** Connect the Compiler stack — compiler → compiler-v2 → compiler-optimizer → grammar → language → regex.

5. **Priority 5:** Add cross-cluster bridges — e.g., ising → thermodynamics (physics), music → math (fib, kuramoto), sensor → robotics (embodied).
