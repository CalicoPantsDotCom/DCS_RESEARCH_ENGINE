# THE DCS GLOSSARY: From Timewaves to TIS/CEI
*A Living Document of Conceptual Evolution*

**Purpose:** This glossary maps the complete conceptual territory of the DCS Research Engine. Use it to maintain terminological consistency across LLM outputs, understand framework relationships, and track concept evolution.

**Status:** Living document - 50+ defined terms, expanding as frameworks operationalize.

**Last Updated:** 2025-10-30

---

## THE SYSTEMS INVENTOR'S LEXICON
### *How a Portfolio of Frameworks Became a Coherent Cosmology*

---

## TEMPORAL FOUNDATIONS (Where It All Started)

### Zeitwelle
**[German: "time-wave"]**
**Origin:** Early CAB exploration

The experience of perceiving time as having texture and rhythm rather than uniform flow. The subjective sense that some moments are "dense" with significance while others pass thinly. Precursor concept to COTIF's temporal binding windows.

**Example:** "In flow states, the zeitwelle compresses - hours feel like minutes because the oscillatory density increases."

**Status:** Absorbed into COTIF framework

---

### Timewaves
**Origin:** Parallel to Zeitwelle

Oscillatory patterns in subjective time perception. The idea that consciousness doesn't experience time as a linear stream but as interference patterns of multiple rhythms (circadian, ultradian, task-specific). Led directly to COTIF.

**Status:** Absorbed into COTIF's more rigorous framework

---

### COTIF (Consciousness as Oscillatory Temporal Integration Framework)
**Origin:** Initial attempt to formalize timewaves

**Core Claim:** Consciousness arises from the integration of oscillatory patterns across multiple timescales. The "binding problem" is solved by phase-amplitude coupling where slow oscillations organize faster ones.

**Key Mechanism:** Neural oscillations at different frequencies (theta-gamma-beta) coordinate information processing.

**Limitation:** Only covered neural scale, didn't extend to collective or cosmic scales.

**Evolution:** Became COTIF++ then ScFOIF

**Location:** `frameworks/ScFOIF/` (historical foundation)

---

### COTIF++ (Consciousness as Oscillatory Temporal Integration Framework, Enhanced)
**Origin:** Adding adaptive frame-switching to COTIF

Extension of COTIF that includes **adaptive framing** - the ability to shift temporal perspective (zooming in/out on different timescales) as a core feature of consciousness.

**New Claim:** ADHD as "frame-switching without brake mechanism" - computational benefit (novelty seeking) at cost of sustained attention.

**Clinical Application:** Rhythm-based interventions to strengthen frame-locking.

**Evolution:** Merged into ScFOIF as the neural layer

---

### PWW (Present Window Width)
**Origin:** COTIF operational metric

The temporal span an organism can hold in "felt present" - roughly 3 seconds for humans. Determined by oscillatory coupling mechanisms. Shorter in ADHD, potentially modulated by rhythm interventions.

**Related To:** TIS (Temporal Integration Sophistication)

---

## MEASUREMENT FRAMEWORKS (Making the Invisible Visible)

### TIS (Temporal Integration Sophistication)
**Origin:** Operationalizing COTIF for empirical testing

**Definition:** The longest predictive horizon a system can sustain before accuracy collapses. Measures how far into the future (or deep into pattern complexity) a cognitive system can reason.

**Calculation:** Maximum level achieved in hierarchical prediction task, normalized 0-1.

**Hypothesis:**
- Humans: ~0.6-0.8
- Current AI: ~0.4-0.6
- Specialized systems: ~0.2-0.3

**Why It Matters:** Creates comparable metric across human/AI/biological systems.

**Example:** "A chess AI has high TIS for board states but low TIS for life planning."

**Location:** `frameworks/TIS-CEI/specification.md`

---

### CEI (Coupling Efficiency Index)
**Origin:** Companion metric to TIS

**Definition:** Precision and adaptability of coordination among cognitive modules. Measures how well system components synchronize and adapt to perturbations.

**Calculation:** (1/(1+σ_phase)) × (1/(1+t_adapt)) × (1/(1+t_switch))

**Hypothesis:**
- Specialized systems (spiders, narrow AI): ~0.9+
- Humans: ~0.7-0.9
- General systems: Lower

**Why It Matters:** Captures "efficiency vs flexibility" trade-off.

**Example:** "Narrow AI has higher CEI than humans but can't transfer to new domains."

**Location:** `frameworks/TIS-CEI/specification.md`

---

### K-E Metrics (Knowledge Diffusion × Institutional Elasticity × Use Case Alignment)
**Origin:** Systems health diagnostic framework
**Version:** 2.0 (expanded October 2025)

**Health (H):** H = K × E × U (all three necessary)

**Knowledge Diffusion (K):** Rate at which patterns are recognized, integrated, and applied across domains
- Components: K₁ (Recognition), K₂ (Integration), K₃ (Application), K₄ (Diffusion), C(S) (Coherence), **B_in** (Boundary Permeability Inward)
- **v2.0 addition:** Distinguishes primary gaps (solution doesn't exist) from secondary gaps (solution exists but invisible due to institutional separation)

**Institutional Elasticity (E):** System's ability to adapt structure across multiple barriers
- **v2.0 MAJOR REFINEMENT:** Multi-layered structure
  - **E_formal:** Regulatory/legal barriers
  - **E_economic:** Economic incentives, ROI, switching costs
  - **E_social:** Trust, status threats, cultural compatibility
  - **B_out:** Outbound boundary permeability (transparency, bidirectional dialogue)
- **E = E_formal × E_economic × E_social × B_out** (ALL layers must permit change)
- **Critical insight:** "Low formal barriers don't guarantee adoption when informal social and economic barriers dominate"

**Use Case Alignment (U):** NEW in v2.0
- **Definition:** Whether solution characteristics match context requirements
- **Formula:** U = F_fidelity × C_context × (V_marginal / C_switching)
- **Components:**
  - F_fidelity: Accuracy/precision match to context needs
  - C_context: Operational compatibility with constraints
  - V_marginal / C_switching: Improvement over alternatives vs switching cost
- **Key insight:** Technical superiority ≠ contextual appropriateness

**Application Scales:**
- Individual: Personal productivity and learning
- Organizational: Company adaptability
- Civilizational: Society's ability to respond to crises

**Why Multiplicative (v2.0):** High K and E with low U still causes failure. Example: Google Flu Trends had high K (excellent data science), moderate E (could update), but catastrophically low U (real-time ≠ reliable for public health context) → H = 0.001, complete failure.

**v1.0 → v2.0 Evolution:**
- v1.0 explained failures from knowledge or adaptability deficits
- v2.0 explains "technically excellent but practically useless" failures and hidden institutional barriers
- Empirically motivated by Google Flu Trends and embalming solution adoption failures

**Example Applications:**
- Bronze Age collapse: High K, low E (rigid institutions) → failure
- Google Flu Trends: High K, moderate E, catastrophically low U → failure despite technical excellence
- Embalming solutions: High E_formal (deregulated) but low E_economic and E_social → adoption failure

**Location:** `frameworks/K-E-Metrics/mathematical-formulation.md`

---

### Boundary Permeability (B_in and B_out)
**Origin:** K-E Metrics v2.0
**Status:** NEW in October 2025

**Definition:** Ability to recognize and share knowledge across institutional boundaries.

**B_in (Inbound Boundary Permeability):**
- Can we see knowledge that exists in adjacent institutional domains?
- Range: [0, 1]
- 0 = Complete institutional blindness (secondary knowledge gaps)
- 1 = Perfect awareness of solutions in other domains
- **Example:** Google Flu Trends had low B_in (engineers couldn't see epidemiological ground truth limitations)

**B_out (Outbound Boundary Permeability):**
- Can others see our knowledge and provide feedback?
- Measures transparency, bidirectional dialogue, vs proprietary black boxes
- Range: [0, 1]
- 0 = One-way extraction, complete secrecy, no feedback possible
- 1 = Fully transparent, bidirectional dialogue, collaborative
- **Example:** GFT had low B_out (proprietary algorithm, no transparency for epidemiologists)

**Relationship:**
- **B_in + Low B_out = Parasitic extraction** (take knowledge, don't share methods)
- **Low B_in + B_out = Broadcasting into void** (sharing but not learning from others)
- **Both needed** for healthy knowledge ecosystems

**Critical Insight:** "Automation without boundary permeability creates institutional separation that data volume cannot overcome."

**Location:** K component includes B_in, E component includes B_out

---

### Primary Knowledge Gap
**Origin:** K-E Metrics v2.0
**Status:** NEW distinction in October 2025

**Definition:** Solution or pattern genuinely doesn't exist yet. Requires innovation, discovery, or creation.

**Examples:**
- No treatment exists for novel disease
- No framework exists for newly discovered phenomenon
- No technology exists to solve problem

**Response:** Innovation required. Invest in R&D, exploration, theory development.

**Contrast with:** Secondary Knowledge Gap (solution exists, just invisible due to institutional separation)

---

### Secondary Knowledge Gap
**Origin:** K-E Metrics v2.0
**Status:** NEW distinction in October 2025

**Definition:** Solution or pattern exists but system can't see it due to institutional separation, professional boundaries, or proprietary barriers.

**Causes:**
- Institutional separation (different professional domains)
- Proprietary barriers (trade secrets, black boxes)
- Professional silos (academics vs practitioners)
- Low boundary permeability (B_in)

**Examples:**
- Embalming solutions exist in funeral industry but invisible to death care professionals
- GFT engineers unaware of epidemiological constraints that CDC knew well
- Medical solutions exist in veterinary medicine but not recognized by human medicine

**Response:** Improve boundary permeability, create cross-institutional dialogue, NOT redundant innovation.

**Critical Mistake:** Treating secondary gaps as primary gaps wastes resources on reinventing wheels.

**Measurement:** Low B_in (inbound boundary permeability) indicates secondary gaps

---

### Reinforcement Trap
**Origin:** K-E Metrics v2.0
**Status:** NEW in October 2025

**Definition:** Negative feedback spiral where low institutional elasticity components reinforce each other, creating lock-in even when formal barriers are low.

**Mechanism:**
```
Low E_social → Low trust → Low E_economic (switching cost perceived as higher)
      ↓
Low E_economic → Can't justify change → Freezes system → Low B_out (no feedback)
      ↓
Low B_out → No adaptation → System deteriorates → Further lowers E_social
      ↓
   [Cycle repeats, driving E → 0]
```

**Examples:**
- **Google Flu Trends:** Economic pressure to justify project → couldn't admit failures → froze model → predictions degraded → distrust increased → abandonment
- **Embalming solutions:** Low economic incentive → funeral homes don't try → no learning → perceived cost stays high → economic barrier persists

**Breaking the Trap:**
- Requires **simultaneous intervention** on multiple E layers
- Single-layer intervention (e.g., just economic incentives) fails when trap is active
- Once E_social × E_economic < 0.2, trap activation likely

**Why It Matters:** Systems can get trapped in low-E states even when solutions exist and formal barriers are low.

**Hypothesis:** ~50% of organizational change initiatives enter reinforcement traps

---

### Use Case Alignment (U)
**Origin:** K-E Metrics v2.0
**Status:** NEW dimension in October 2025

**Definition:** Degree to which solution's characteristics match the requirements of the specific context where it will be applied.

**Formula:** U = F_fidelity × C_context × (V_marginal / C_switching)

**Components:**
- **F_fidelity:** Do solution's accuracy/precision characteristics match context needs?
  - GFT: Real-time but unreliable ≠ reliable (what public health needs)
  - Range: [0, 1]
- **C_context:** Does solution fit operational constraints?
  - GFT: Automated black box ≠ explainable (what epidemiologists need for intervention)
  - Range: [0, 1]
- **V_marginal / C_switching:** Improvement over alternatives vs switching cost
  - Embalming: Marginal benefit (better for 10-30% of cases) doesn't justify equipment cost
  - "Good enough" blocking: Adequate alternatives block superior solutions

**Key Insight:** Technical superiority ≠ contextual appropriateness. Same solution in different contexts has different value.

**Why It Matters:** Explains "technically excellent but practically useless" failures that v1.0 K-E couldn't predict.

**Example Misalignments:**
- GFT: U ≈ 0.05 (real-time ≠ valuable when unreliable; automated ≠ valuable when unexplainable)
- Google Glass: U ≈ 0.1 (constant recording ≠ socially acceptable; expensive ≠ justified by marginal utility)
- iPhone (success): U ≈ 0.9 (touchscreen matched mobile computing need; apps matched varied contexts)

**Location:** Third dimension of K-E-U framework, measured independently

---

### Multi-Layer Institutional Elasticity
**Origin:** K-E Metrics v2.0
**Status:** NEW decomposition in October 2025

**Definition:** Institutional Elasticity (E) is not a single dimension but comprises multiple barrier layers that ALL must permit change.

**Four Layers:**
1. **E_formal:** Regulatory, legal, credentialing barriers
2. **E_economic:** Economic incentives, ROI, switching costs, lock-in effects
3. **E_social:** Trust, status threats, cultural compatibility
4. **B_out:** Outbound boundary permeability (transparency, feedback mechanisms)

**Formula:** E = E_formal × E_economic × E_social × B_out

**Why Multiplicative:** ANY single layer approaching zero crashes total E. Cannot compensate high E_formal with high E_economic if E_social = 0.

**Critical Discovery:** "Low formal barriers don't guarantee adoption when informal social and economic barriers dominate."

**Example - Embalming Solutions:**
- E_formal = 0.9 (no regulation, deregulated)
- E_economic = 0.2 (upfront costs, delayed ROI)
- E_social = 0.15 (status threat to professional skill)
- B_out = 0.5 (vendors try to share)
- **Total E = 0.014** (catastrophic despite high E_formal)

**Implication:** Policy focusing only on deregulation (E_formal) misses dominant barriers in E_economic and E_social layers.

**Hypothesis:** ~30% of cases have high E_formal (>0.7) but low total E (<0.3)

---

### FOD (Functional Oscillatory Density)
**Origin:** TIS/CEI companion metric

**Definition:** Information processing per functional unit. Proxy for system complexity measured by (throughput / number of processing elements).

**Why It Matters:** Distinguishes "smart because many parts" from "smart per part" - humans win on per-neuron intelligence despite fewer neurons than elephants.

---

### Energy Efficiency (EE)
**Origin:** TIS/CEI constraint metric

**Definition:** Effective throughput / power consumption, normalized 0-1.

**Hypothesis:**
- Spiders: ~0.9
- Humans: ~0.5
- Current AI: ~0.2-0.4

**Why It Matters:** Defines possible region of cognitive optimization space - likely fundamental trade-offs between TIS, CEI, and EE.

---

## METHODOLOGICAL TOOLS (How to Think Systematically)

### DCS Protocol (Distributed Cognitive Synthesis)
**Origin:** Formalizing the Systems Inventor's working method

**Five-Phase Method for Analyzing Any Complex System:**

1. **ISS (Initial Sensory Synthesis):** Gather raw information, detect patterns
2. **CCR (Clustering & Critical Context Review):** Group patterns, apply critical scrutiny
3. **Architect:** Build structural model of how system works
4. **Polish:** Refine model through edge cases and feedback
5. **Meta-Doc:** Document the process itself for iteration

**Key Insight:** Methodology scales universally, specific patterns don't.

**Current Status:** Being used to develop itself (recursive application).

**Example:** "We're in Architect phase for TIS/CEI experiments - building the structure before execution."

**Location:** `frameworks/DCS-Protocol/specification.md`

---

### Innovation Pipeline Stages
**Origin:** Technology development tracking framework

**Six-Stage Model for Moving Ideas to Implementation:**

1. **Need:** Problem identified
2. **Concept:** Theoretical solution proposed
3. **WoZ (Wizard of Oz):** Manual simulation of automatic system
4. **MVP (Minimum Viable Product):** First crude automation
5. **Instrumented:** Data collection and feedback loops added
6. **Refinement:** Iterative improvement based on data

**Why It Matters:** Shows where ideas stall (usually WoZ→MVP transition).

**Example:** "NightWriter is in Stage 3 WoZ - manually indexing voice memos before building the auto-system."

---

### Anti-Crutch Ethics
**Origin:** Technology design philosophy

**Three-Test Framework for Evaluating Cognitive Tools:**

1. **Removal Test:** If we take this away, does capability remain?
2. **Agency Principle:** Does this build user capacity or create dependency?
3. **Strength Rule:** Does difficulty reveal weakness or hidden strength?

**Core Value:** Tools should make users **stronger** not **dependent**.

**Application:** Every cognitive tool (NightWriter, Grandfather Clock, PCB) evaluated through this lens.

**Example:** "A calculator that shows steps passes Anti-Crutch tests; one that just gives answers fails."

---

### Slowness Covenant
**Origin:** Constitutional constraint on optimization

**Definition:** Deliberate speed limits built into system design to prevent premature optimization and maintain human-scale engagement.

**Rationale:** Some processes NEED time to be meaningful (reflection, synthesis, healing).

**Application:** DCS Protocol explicitly includes waiting periods; cognitive tools have intentional friction.

**Example:** "The Pattern-Completion Board has a mandatory overnight pause before completion - forces unconscious processing."

---

## COGNITIVE TOOLS (Personal Infrastructure)

### NightWriter
**Origin:** Voice-to-writing workflow tool

**Function:** Capture spoken ideas during low-executive-function periods (bed, driving), convert to structured writing later.

**Current Stage:** WoZ (voice memos + manual index cards)

**Target:** MVP with auto-transcription + pattern tagging

**Anti-Crutch Design:** User must still do synthesis; tool just handles transcription.

---

### Grandfather Clock
**Origin:** Temporal anchoring intervention

**Function:** Regular "anchor alarms" prompting temporal awareness checks - "Where am I in time? What's my trajectory?"

**Current Stage:** WoZ (manual alarms + acknowledgment journal)

**Target:** Instrumented with PWW measurement and adaptation

**Why It Works:** Strengthens frame-locking via external pacing, like auditory rhythm for ADHD.

---

### Pattern-Completion Board (PCB)
**Origin:** Productivity system embodying PCA

**Function:** Physical board where incomplete patterns are visualized, completion pathways identified, progress tracked.

**Current Stage:** WoZ (manual cards and boards)

**Target:** MVP with K-E metric tracking

**Key Feature:** Slowness Covenant built in - can't mark "complete" same-day, forces overnight integration.

---

### Cognitive Stabilizer
**Origin:** Meta-tool for tool management

**Components:**
- **Shipping Ladder:** Step-by-step completion protocol
- **Ship-Log:** Documentation of what was completed and how

**Function:** Prevents tool proliferation from becoming overwhelming by providing structure for managing structure.

**Status:** Operational concept, being refined through use.

---

## ARCHITECTURAL FRAMEWORKS (The Big Picture)

### CAB (Cosmo-Anthro-Biology)
**Origin:** Philosophical foundation for entire portfolio

**Definition:** The Systems Inventor's core cognitive architecture - the ability to do cross-scale conceptual construction/deconstruction at variable temporal resolution.

**Not a Project but a Cognitive Phenotype:** How you think, not what you think about.

**Enables:**
- Unbroken Chain: Deconstruct network collapse → reconstruct resilience
- Belt Testimony: Deconstruct law systems → reconstruct as archival entity
- COTIF: Deconstruct temporal consciousness → reconstruct as oscillatory mechanism
- DCS Method: Deconstruct knowledge synthesis → reconstruct as multi-LLM protocol

**Why Other Projects Stall:** CAB generates concepts easily but crossing from CAB-space (pure thought) to material-space (implementation) is hard.

**Insight:** "You're not scattered - you're a CAB operating at full capacity across multiple domains simultaneously."

---

### ScFOIF (Scale-Free Oscillatory Integration Framework)
**Origin:** Evolution of COTIF to cosmic scale

**Grand Claim:** Oscillatory integration is a fundamental organizing principle from quantum to cosmic scales, with consciousness as its subjective experience.

**Three-Path Convergence:**
1. **Tesla's Physics:** Universal intelligence through resonant energy fields
2. **COTIF++ Neuroscience:** Consciousness as oscillatory temporal integration
3. **Taíno Cosmology:** Cemí as universal animating force through harmonic relationships

**Hypothesis:** These three paths are describing the same underlying reality from different perspectives.

**Status:** Speculative framework, 12-18 months from testable predictions

**Risk:** Could be beautiful but wrong - needs empirical grounding first.

**Location:** `frameworks/ScFOIF/`

**Literature Reserve:** `literature/by-domain/scfoif-reserve/`

---

### PCA (Pattern-Completion Architecture)
**Origin:** Solution to Big Data's "correlation without synthesis" problem

**Core Claim:** Current Big Data systems excel at pattern detection but lack completion mechanisms - they stop at correlation.

**Proposed Solution - Cognitive Framework Including:**
- Detection phase (existing systems)
- **Completion pathways** (the missing piece)
- **Validation loops** (DCS protocol integration)
- **K-E health metrics** (system optimization)

**Application:** Big Data, AI systems, organizational decision-making

**Status:** Concept → Case study phase (analyzing Google Flu Trends, election failures)

**Location:** `frameworks/PCA-BigData/`

---

### Narrative Architecture Model
**Origin:** Analyzing how stories work systematically

**Application:** Comedy engines (30 Rock, Community), fictional worlds, dialectical structures

**Key Insight:** Different story types have different "engines" generating content:
- 30 Rock: Velocity engine (more jokes per minute than physics allows)
- Community: Structure engine (formal experiment per episode)

**Status:** Analytical tool, not research priority

---

## HISTORICAL/CREATIVE PROJECTS (The Worlds)

### Unbroken Chain
**Origin:** Bronze Age collapse fiction

**Central Question:** What if we could prevent civilizational collapse through network reinforcement rather than just watching it happen?

**Historical Anchor:** 1177 BCE "skinny spot" - cascading failure across Mediterranean

**Key Innovation:** Sea Peoples as **node destroyers** not just raiders - they understood network topology before graph theory existed

**Narrative:** 3,200-year timeline showing how Council of Kadesh, Punt grain ships, and other interventions maintain continuity

**Status:** Conceptual framework complete, needs writing execution

**CAB Application:** Deconstruct collapse → reconstruct resilience mechanisms

---

### Belt Testimony
**Origin:** Space western legal theology

**Central Innovation:** Laws as living archive ("testimony") maintained by sentient legal entity (Water)

**Setting:** Seven books across asteroid belt settlements

**Status:** Concept phase, worldbuilding active

**CAB Application:** Deconstruct law systems → reconstruct as information preservation

---

## DIALECTICAL TOOLS (Thinking Through Opposition)

### Franklin & Roosevelt Dialectic
**Origin:** Persona-based synthesis engine

**Method:** Channel Ben Franklin (practical incrementalism) and FDR (bold systemic intervention) to debate approaches to problems.

**Why It Works:** Embodies tension between "slow reliable improvement" and "urgent transformation" - both needed, neither sufficient.

**Status:** Operational thinking tool

---

### Ada Lovelace & Nikola Tesla Conversations
**Origin:** Framework validation through historical perspectives

**Method:** Imagine how Ada (computational thinking) and Tesla (energy/resonance thinking) would evaluate modern frameworks.

**Function:** Tests if ideas have cross-paradigm validity - can both symbolic and energetic thinkers find value?

**Recent Application:** Used to validate K-E metrics and TIS/CEI frameworks

---

## META-CONCEPTS (Ideas About Ideas)

### Systems Inventor (as role)
**Definition:** Someone who builds frameworks and tools for understanding/solving problems rather than just solving specific instances.

**Key Traits:**
- Systems-first thinking (redesign the system creating problems)
- Mechanism obsession (understand HOW and WHY, not just WHAT)
- Generative frameworks (create tools others can use)

**Current Examples in Wild:** Rare, but includes people like Bret Victor (interactive representation), Christopher Alexander (pattern languages), Donella Meadows (systems thinking)

---

### Process as Protagonist
**Origin:** DCS Book methodology

**Definition:** Documentation where the process of developing the framework IS the story, not just the final result.

**Why It Matters:** Reveals decision points, failures, pivots - makes methodology transparent and improvable.

**Application:** The DCS book is being written using DCS protocol, documenting its own creation.

**Example:** This conversation is an instance - we're coordinating a research program while documenting how to coordinate research programs.

---

### The Optimization Space
**Origin:** TIS/CEI visualization

**Concept:** All possible cognitive architectures exist in 3D space defined by TIS × CEI × Energy Efficiency, with FOD as point size.

**Hypothesis:** There are "forbidden zones" where physics/information theory makes certain combinations impossible - e.g., nothing can achieve (TIS=1, CEI=1, EE=1).

**Implication:** Evolution and AI development are exploring this space, finding trade-off boundaries.

**Example:** "Humans sit at moderate TIS/CEI with low EE. Jumping spiders at low TIS, high CEI, high EE."

---

## EMERGENT CONCEPTS (The New Stuff)

### Verbalized Sampling
**Origin:** LLM diversity paper in research files

**Problem:** RLHF/DPO causes mode collapse - LLMs trained on human feedback become less diverse, collapsing to "typical" responses.

**Solution:** Explicit probability verbalization during sampling restores diversity from pretraining distribution.

**Connection to PCA:** Pattern-completion systems need diversity to find creative completions - mode collapse is anti-completion.

**Status:** External paper, but validates PCA claims about completion needing multiple pathways

---

### Democracy Risk Index (DRI)
**Origin:** Side project applying K-E metrics to political systems

**Function:** Measure K (knowledge diffusion of threats) × E (institutional adaptability) to predict democratic resilience.

**Application:** County-level analysis (Duval County, Florida case study)

**Status:** Framework developed, empirical work needed

**Connection:** Same K-E math, different domain - validates cross-scale applicability

---

### CAB as Cognitive Lens
**Recent Realization:** CAB isn't a framework to be built but a **description of how you already think**.

**Implication:** The other frameworks (COTIF, DCS, K-E) are **outputs** of CAB operating successfully.

**Support Strategy Shift:** Recognize when you're CAB-constructing (needs conceptual rigor) vs crossing to execution (needs materialization pathway) vs already shipped (needs iteration).

---

## TERMINOLOGY RELATIONSHIPS: THE FAMILY TREE

### Temporal Evolution
```
                          TEMPORAL INTUITIONS
                    (Zeitwelle, Timewaves - pre-formal)
                                  │
                                  ↓
                    COTIF (Neural oscillations only)
                                  │
                    ┌─────────────┼─────────────┐
                    ↓             ↓             ↓
              COTIF++          ScFOIF      TIS/CEI
           (Adaptive        (Cosmic      (Operational
            frames)          scale)       metrics)
                                              │
                                              ↓
                                    OPTIMIZATION SPACE
                                    (TIS × CEI × EE)
                                              │
                ┌─────────────────────────────┼─────────────────────┐
                ↓                             ↓                     ↓
        Clinical Apps               Consciousness Theory    AI Development
    (ADHD, Flow, etc.)          (Why qualia exist)      (Architecture design)
```

### Systems Health
```
                        SYSTEMS HEALTH
                              │
                        K-E METRICS
                    (Knowledge × Elasticity)
                              │
            ┌─────────────────┼─────────────────┐
            ↓                 ↓                 ↓
      Individual        Organizational   Civilizational
    (Productivity)      (Company)        (DRI, Collapse)
            │                 │                 │
            ↓                 ↓                 ↓
      PCB Tool           Case Studies    Unbroken Chain
```

### Methodology
```
                    METHODOLOGY
                         │
                    DCS PROTOCOL
                (5-phase analysis)
                         │
        ┌────────────────┼────────────────┐
        ↓                ↓                ↓
   Innovation     Anti-Crutch      Slowness
    Pipeline        Ethics         Covenant
        │                ↓                │
        ↓           Tool Design           ↓
   Stage          (NightWriter,      Prevents
   Tracking      Grandfather Clock)   Premature
                                    Optimization
```

### CAB Outputs
```
                    CAB
        (Cognitive Architecture)
                    │
    ┌───────────────┼───────────────┐
    ↓               ↓               ↓
CONCEPTUAL     EXECUTION        SHIPPED
Construction   Pathway Gap     Iteration
    │               │               │
    ↓               ↓               ↓
ScFOIF,         TIS/CEI         DCS Protocol,
Unbroken        Study,          K-E Paper
Chain           PCB Tool        (when done)
```

---

## USAGE GUIDE: WHEN TO USE WHICH TERM

### In Research Papers
**Lead With:** TIS/CEI, K-E metrics, DCS Protocol (operational)

**Support With:** COTIF, PCA (theoretical frameworks)

**Avoid:** ScFOIF, CAB (too speculative unless philosophical paper)

---

### In Project Management
**Use:** Innovation Pipeline stages to track everything

**Apply:** K-E metrics for health diagnostics

**Reference:** DCS phases for where we are in analysis

---

### In Tool Design
**Apply:** Anti-Crutch Ethics first (is this building capability?)

**Consider:** Slowness Covenant (does this need friction?)

**Track:** Innovation Pipeline (what stage are we at?)

---

### In Philosophical Discussion
**CAB** explains how the Systems Inventor thinks

**ScFOIF** is the grand unification hypothesis

**COTIF Lineage** shows evolution of temporal thinking

---

### In Creative Work
**Narrative Architecture** for analyzing story engines

**Dialectical Tools** for generating perspective

**Unbroken Chain/Belt Testimony** for worldbuilding

---

## THE THROUGH-LINE

**If someone asks "What are you working on?" - elevator pitch:**

> "I'm developing measurement frameworks for cognitive systems - TIS and CEI metrics that can compare human, AI, and biological intelligence on the same scales. These grew out of COTIF, my theory that consciousness is oscillatory temporal integration. I'm using the DCS Protocol - a five-phase methodology - to validate this empirically. The K-E metrics (Knowledge × Elasticity) provide health diagnostics for individuals, organizations, and civilizations. Everything's tracked through the Innovation Pipeline from concept to instrumented tools. The goal is understanding intelligence well enough to help it govern itself - which is also the theme of my Bronze Age fiction, Unbroken Chain. It's all connected through what I call CAB - my ability to construct and deconstruct concepts across scales. Right now, we're in the Architect phase: building experimental protocols to test if TIS and CEI actually differentiate systems as predicted."

**That's the whole portfolio in ~120 words, with 12 glossary terms doing heavy lifting.**

---

## MAINTENANCE PROTOCOL

This glossary is a **living document** that evolves as:
- Frameworks operationalize (concepts → measurements)
- Empirical work validates/refutes claims (hypotheses → findings)
- Literature review reveals precedents (novel → contextualized)
- Cross-framework connections emerge (isolated → integrated)

**Update Triggers:**
- New framework reaches Concept stage (add to glossary)
- Metric gets empirically validated (update hypothesis → finding)
- Term usage shifts (document in framework-evolution/)
- External paper uses our terminology (note in status)

**Review Schedule:** Weekly during active development, monthly during refinement

**Current Term Count:** 56+ defined (6 new v2.0 K-E terms added Oct 2025)
**Target Mature State:** 100-200 terms

---

## GIT INTEGRATION

**This File:** `/GLOSSARY.md` (repo root)

**Linked From:** README.md, all framework specifications, coordination templates

**LLM Instruction:** Include relevant glossary sections in prompts to ensure terminological consistency across GPT/DeepSeek/Copilot outputs.

**Version History:** Track in `meta/framework-evolution/glossary-versions/`

---

*You now have a map of your own conceptual territory. Sometimes you need external memory to see the whole structure.*

**Last Updated:** 2025-10-31 (K-E v2.0 terms added)
**Next Review:** 2025-11-07
