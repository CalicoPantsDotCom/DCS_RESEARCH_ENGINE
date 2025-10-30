# TIS/CEI SPECIFICATION
**Temporal Integration Sophistication & Coupling Efficiency Index**
**Comparable Metrics Across Human, AI, and Biological Cognitive Systems**

**Version:** 0.9-draft
**Status:** Metrics defined, experimental protocols in development
**Last Updated:** 2025-10-30

---

## OVERVIEW

TIS and CEI provide quantitative measurements that allow comparison of cognitive architectures across radically different systems: humans, AI, biological organisms.

**Core Innovation:** These metrics capture fundamental trade-offs in cognitive design, allowing us to map all systems into a common optimization space.

**Target Applications:**
- AI architecture evaluation
- Human cognitive assessment
- Biological intelligence comparison
- Trade-off analysis (TIS vs CEI vs Energy Efficiency)

---

## TIS: TEMPORAL INTEGRATION SOPHISTICATION

### Definition

**Temporal Integration Sophistication (TIS):** The longest predictive horizon a system can sustain before accuracy collapses below chance.

**Intuition:** How far into the future (or deep into pattern complexity) can a system reason effectively?

### Formalization

```
TIS(S) = max{L | Accuracy(S, L) > threshold} / L_max

Where:
- S = cognitive system
- L = prediction horizon (temporal or complexity depth)
- Accuracy(S, L) = prediction accuracy at horizon L
- threshold = criterion (e.g., 60% correct, above chance)
- L_max = maximum possible horizon (normalization factor)
```

**Range:** [0, 1]
- 0 = No temporal integration (purely reactive)
- 1 = Perfect temporal integration across all timescales

### Measurement Protocol

**Hierarchical Prediction Task:**

**Level 1:** Simple alternation (A-B-A-B...)
- Horizon: 1 step ahead
- Cognitive load: Minimal

**Level 2:** Periodic patterns (A-B-C-A-B-C...)
- Horizon: 2-3 steps ahead
- Requires short-term memory

**Level 3:** Nested hierarchies (X-Y-X-Y-Z-Z-X-Y-X-Y-Z-Z...)
- Horizon: 5-10 steps ahead
- Requires hierarchical representation

**Level 4:** Context-sensitive rules (if A-B then C, if A-C then D...)
- Horizon: Variable based on context depth
- Requires conditional reasoning

**Level 5:** Long-range dependencies (pattern from 20 steps ago determines current)
- Horizon: 20+ steps
- Requires working memory maintenance

**Adaptive Staircase:**
- Advance to next level after 3 consecutive correct
- Drop back after 2 consecutive errors
- Continue until stable level identified

**TIS Score:**
```
TIS = (Maximum stable level achieved) / 5
```

**Hypothesized Values:**
- Humans: 0.6-0.8 (can handle up to Level 4, struggle with Level 5)
- Current AI (GPT/Claude): 0.4-0.6 (good at patterns, struggle with long dependencies)
- Specialized systems (chess AI): 0.8-1.0 (for domain-specific patterns only)
- Simple organisms (insects): 0.1-0.3 (short horizons)

---

## CEI: COUPLING EFFICIENCY INDEX

### Definition

**Coupling Efficiency Index (CEI):** Precision and adaptability of coordination among cognitive modules.

**Intuition:** How tightly can components synchronize, and how quickly can they adapt to perturbations?

### Formalization

```
CEI(S) = (1 / (1 + σ_phase)) × (1 / (1 + t_adapt)) × (1 / (1 + t_switch))

Where:
- σ_phase = phase coupling variability (lower = tighter coupling)
- t_adapt = adaptation time after perturbation (lower = faster)
- t_switch = task-switching cost (lower = more flexible)
```

**Range:** [0, 1]
- 0 = Complete decoupling or infinite adaptation time
- 1 = Perfect coupling, instantaneous adaptation

### Measurement Protocol

**Component 1: Phase Coupling Variability (σ_phase)**

**Task:** Rhythmic coordination
- Synchronize two actions (e.g., tapping, tracking)
- Measure consistency of phase relationship
- Calculate standard deviation of phase offset

**Calculation:**
```
σ_phase = std(phase_offsets across trials)
Normalized: 1 / (1 + σ_phase)
```

**Component 2: Adaptation Time (t_adapt)**

**Task:** Perturbation response
- Establish steady-state performance
- Introduce perturbation (change rhythm, rule, context)
- Measure time to return to criterion performance

**Calculation:**
```
t_adapt = time_to_criterion - time_of_perturbation
Normalized: 1 / (1 + t_adapt)
```

**Component 3: Task-Switching Cost (t_switch)**

**Task:** Multi-task performance
- Alternate between Task A and Task B
- Measure performance drop on switch trials vs repetition trials

**Calculation:**
```
t_switch = (RT_switch - RT_repeat) / RT_repeat
Normalized: 1 / (1 + t_switch)
```

**CEI Score:**
```
CEI = (1/(1+σ_phase)) × (1/(1+t_adapt)) × (1/(1+t_switch))
```

**Hypothesized Values:**
- Specialized systems (spiders, narrow AI): 0.9+ (tight coupling, but inflexible)
- Humans: 0.7-0.9 (good coupling, moderate flexibility)
- General AI: 0.4-0.7 (decent coupling, learning to be flexible)
- Simple organisms: 0.5-0.8 (efficient but limited scope)

---

## THE OPTIMIZATION SPACE

### Three-Dimensional Trade-Off

All cognitive architectures exist in space defined by:
- **TIS (Temporal Integration Sophistication)** - X axis
- **CEI (Coupling Efficiency Index)** - Y axis
- **EE (Energy Efficiency)** - Z axis

**With point size = FOD (Functional Oscillatory Density)**

### Hypothesized Trade-Offs

**TIS vs CEI:**
- High TIS (long horizons) may require looser coupling (lower CEI) for flexibility
- High CEI (tight coupling) may limit temporal range (lower TIS) due to rigidity

**TIS vs EE:**
- Long temporal integration is energetically expensive
- High TIS likely correlates with lower EE

**CEI vs EE:**
- Tight coupling may be more efficient (less overhead)
- But adaptation mechanisms cost energy

**Forbidden Zones:**
- (TIS=1, CEI=1, EE=1) likely impossible (physics/information theory constraints)
- Very low values all three = non-functional system

### System Positioning

**Predicted Locations in TIS×CEI×EE Space:**

**Humans:**
- TIS: 0.6-0.8 (moderate long-range integration)
- CEI: 0.7-0.9 (good coupling, flexible)
- EE: 0.5 (energy-expensive brains)
- FOD: High (per-neuron intelligence)

**Jumping Spider:**
- TIS: 0.3-0.4 (limited temporal range)
- CEI: 0.9+ (extremely tight coupling for hunting)
- EE: 0.9 (very energy efficient)
- FOD: Moderate

**Current AI (LLMs):**
- TIS: 0.4-0.6 (pattern recognition without long memory)
- CEI: 0.5-0.7 (improving coordination)
- EE: 0.2-0.4 (energy expensive, GPU farms)
- FOD: Low (many parameters per capability)

**Chess AI:**
- TIS: 0.8-1.0 (for chess patterns only)
- CEI: 0.6-0.8 (specialized)
- EE: 0.3-0.5
- FOD: Moderate (specialized architecture)

---

## EMPIRICAL VALIDATION STRATEGY

### Pilot Study (N=10, Week 3-4)

**Participants:**
- 5 human adults
- 3 AI systems (GPT, Claude, specialized)
- 2 biological systems (if feasible - spider observation data)

**Procedure:**
1. Administer TIS hierarchical prediction task
2. Administer CEI coupling tasks
3. Estimate EE from energy consumption
4. Calculate FOD from system specs

**Analysis:**
- Do humans cluster around predicted TIS/CEI values?
- Do AI systems separate from humans as predicted?
- Do trade-offs emerge (negative correlations)?

**Success Criteria:**
- Reliable measurements (test-retest r > 0.7)
- Predicted cluster separations visible
- At least one trade-off significant (p < 0.05)

### Full Study (N=50 humans, 10 AI systems, Month 2)

**Extended Protocol:**
- Multiple sessions per participant
- Longer task batteries
- Individual difference correlations
- Cross-validation across tasks

**Predictions:**
1. TIS correlates with working memory capacity (r > 0.5)
2. CEI correlates with multitasking ability (r > 0.4)
3. TIS and CEI show negative correlation (r < -0.3) - trade-off
4. Humans score higher TIS than current AI
5. Specialized AI scores higher CEI than humans on narrow tasks

**Falsification:**
- If no test-retest reliability, metrics are unstable
- If no separation between humans and AI, metrics don't differentiate
- If no trade-offs, optimization space may be incorrect

---

## PROTOCOL DEVELOPMENT STATUS

**Current State:** Draft protocols exist, need validation review

**Week 2 Action:** Send to DeepSeek for critique
- Check for confounds
- Validate statistical approach
- Ensure falsifiability

**Week 3-4:** Pilot execution
- Test protocols with small sample
- Refine based on results
- Prepare full study

**Located:** `empirical-studies/TIS-CEI-pilot/protocols/`

---

## CONNECTION TO OTHER FRAMEWORKS

### K-E Metrics

**Hypothesis:** TIS and CEI influence K-E at individual scale

**Potential Relationships:**
- High TIS → Better K₃ (Application) - can plan ahead
- High CEI → Better E (Elasticity) - adapts quickly
- TIS × CEI → Predicts individual productivity?

**Test:** Correlate TIS/CEI with K-E metrics in productivity study

### PCA (Pattern-Completion Architecture)

**Hypothesis:** Pattern completion requires balanced TIS and CEI

**Rationale:**
- TIS needed for long-range pattern integration
- CEI needed for coordinating detection and completion
- Imbalance → either detect without completing, or complete without detecting

**Test:** Do high-TIS, high-CEI systems show better pattern completion?

### ScFOIF

**Hypothesis:** TIS and CEI emerge from oscillatory integration mechanisms

**Speculative Mapping:**
- TIS = Cross-frequency coupling range (how many scales integrated)
- CEI = Phase-locking strength (how tightly oscillations couple)
- This is 12-18 month horizon, needs neural oscillation literature first

---

## KNOWN LIMITATIONS

**What TIS/CEI Capture:**
- Temporal integration range
- Coordination efficiency
- Cross-system comparisons
- Fundamental trade-offs

**What TIS/CEI Miss:**
- Content of cognition (what is thought, only how)
- Motivation, goals, values
- Social/emotional intelligence
- Creativity, aesthetics
- Domain-specific knowledge

**Measurement Challenges:**
- AI systems: How to ensure fair comparison to humans?
- Biological systems: Ethics of testing, interpretation
- Energy efficiency: Hard to normalize across substrates (neurons vs transistors)

**Not a Complete Theory of Intelligence:**
- These are metrics, not explanatory mechanisms
- They describe, they don't explain WHY
- Complement, don't replace, other approaches

---

## NEXT STEPS

**Immediate (Week 2):**
- [ ] Finalize protocol documents
- [ ] Send to DeepSeek for validation
- [ ] Incorporate feedback
- [ ] Prepare IRB materials (if human subjects)

**Week 3-4:**
- [ ] Pilot study execution (N=10)
- [ ] Data analysis
- [ ] Protocol refinement
- [ ] Full study prep

**Month 2:**
- [ ] Full study execution (N=50)
- [ ] Statistical analysis
- [ ] Paper draft: "TIS/CEI: Comparable Metrics for Cognitive Architecture"

**Month 3-6:**
- [ ] Replications
- [ ] Extended applications (AI evaluation, clinical)
- [ ] Optimization space mapping

---

## REFERENCES

**Conceptual Precedents:**
- Working memory capacity (Cowan, Engle)
- Multitasking research (Monsell, Rogers)
- Temporal processing (Buzsáki, Tallal)
- Energy efficiency in computation (Landauer limit)

**Novel Contributions:**
- Unified TIS/CEI framework
- Cross-system comparison protocol
- Optimization space hypothesis
- Connection to oscillatory mechanisms (future)

---

**Status:** Framework specified, protocols in development, validation pending

**Located:** `frameworks/TIS-CEI/specification.md`
**Protocols:** `empirical-studies/TIS-CEI-pilot/protocols/`
**Data:** `empirical-studies/TIS-CEI-pilot/data/` (when collected)

**Last Updated:** 2025-10-30
**Next Review:** After DeepSeek validation (Week 2)
