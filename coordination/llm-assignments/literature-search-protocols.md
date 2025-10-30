# LITERATURE SEARCH PROTOCOLS
**Multi-LLM Coordination Framework**

**Purpose:** Systematic literature acquisition across six priority domains, with LLM-specific processing pipelines.

**Status:** Active - Domain 4 (Big Data Failures) is Week 1 priority

**Last Updated:** 2025-10-30

---

## GENERAL PROTOCOL

### Acquisition Workflow
1. **Execute Google Scholar searches** using domain-specific strings below
2. **Download PDFs** to `literature/by-domain/[domain]/`
3. **Create analysis file** `[paper-name]_[LLM]-analysis.md` in same folder
4. **Feed to assigned LLM** with domain-specific prompt template
5. **Commit both** PDF + analysis markdown to repository
6. **Track progress** in `coordination/weekly-status/`

### File Naming Convention
```
[FirstAuthorLastName][Year]_[ShortTitle].pdf
[FirstAuthorLastName][Year]_[ShortTitle]_[LLM]-analysis.md
```

**Example:**
```
Lazer2014_GoogleFluTrends.pdf
Lazer2014_GoogleFluTrends_GPT-analysis.md
```

---

## DOMAIN 4: BIG DATA FAILURES (WEEK 1 PRIORITY)

**Target:** 10-15 papers
**Assigned LLM:** GPT (Creative Pattern Detector)
**Analysis Focus:** Failure modes through PCA lens
**Directory:** `literature/by-domain/big-data-failures/`

### Google Scholar Search Strings

**Search 1: Google Flu Trends**
```
"Google Flu Trends" failure analysis postmortem
```
**Expected Papers:** 5-8
**Priority:** CRITICAL - This is the canonical Big Data failure case

---

**Search 2: Election & Healthcare Prediction Failures**
```
"big data" prediction failure "election" OR "healthcare"
```
**Expected Papers:** 10-15
**Priority:** HIGH - Recent, well-documented failures

---

**Search 3: Correlation vs Causation**
```
("data science" OR "analytics") limitations "correlation causation"
```
**Expected Papers:** 15-20
**Priority:** MEDIUM - Provides theoretical backing for PCA claims

---

**Search 4: Recommendation System Failures**
```
"recommendation system" failure "Netflix" OR "Amazon"
```
**Expected Papers:** 5-10
**Priority:** MEDIUM - Shows industry-scale problems

---

**Search 5: Organizational Analysis Paralysis**
```
"big data" "analysis paralysis" organizational
```
**Expected Papers:** 5-8
**Priority:** LOW - Contextualizes human factors

---

### Must-Have Papers

**Critical (Get First):**
1. **Lazer et al. (2014)** - "The Parable of Google Flu: Traps in Big Data Analysis"
   - *The* canonical post-mortem
   - Search: `Lazer "Google Flu" 2014`

2. **boyd & Crawford (2012)** - "Critical Questions for Big Data"
   - Foundational critique
   - Search: `boyd Crawford "Critical Questions for Big Data"`

3. **Silver (2016)** - Any analysis of 2016 election polling failures
   - Recent, public-facing failure
   - Search: `2016 election polling failure analysis`

**Important (Get Second):**
4. Healthcare analytics failures (any well-documented case)
5. Financial prediction failures (2008 crisis, flash crashes)
6. Social media analytics overpromises (Cambridge Analytica era)

---

### GPT Analysis Prompt Template

**For each Domain 4 paper, use this prompt:**

```
I'm analyzing Big Data failures through the Pattern-Completion Architecture (PCA) framework.

PCA claims that current Big Data systems excel at correlation detection but lack completion mechanisms - they stop at pattern recognition without synthesis.

Paper: [TITLE]
Authors: [NAMES]
Year: [YEAR]

Please extract the following:

1. FAILURE DESCRIBED
   - What specific failure occurred?
   - What predictions/claims were made and proven wrong?
   - Scale and impact of the failure?

2. ROOT CAUSE ANALYSIS
   - Technical factors (algorithm, data quality, sampling)
   - Conceptual factors (flawed assumptions, theory gaps)
   - Organizational factors (incentives, pressures, constraints)

3. PATTERN-COMPLETION LENS
   - Where did the system DETECT patterns successfully?
   - Where did COMPLETION fail? (correlation → causation, detection → synthesis)
   - What completion mechanisms were missing?

4. PCA COUNTERFACTUAL
   - How would Pattern-Completion Architecture handle this differently?
   - What completion pathways would be needed?
   - What validation loops were absent?

5. KEY QUOTES
   - 2-3 direct quotes suitable for citation
   - Include page numbers

6. RELATED WORK
   - Papers this cites that we should acquire
   - Suggested follow-up searches

7. K-E METRICS CONNECTION
   - How does this relate to Knowledge Diffusion (K)?
   - How does this relate to Institutional Elasticity (E)?
   - Was this a high-K, low-E failure or vice versa?

Format your response as structured markdown for easy integration into synthesis documents.
```

---

## DOMAIN 2: PATTERN COMPLETION (WEEK 2 PRIORITY)

**Target:** 8-10 papers
**Assigned LLM:** DeepSeek (Technical Validator)
**Analysis Focus:** Technical mechanisms, mathematical models, neural substrates
**Directory:** `literature/by-domain/pattern-completion/`

### Google Scholar Search Strings

**Search 1: Neural Pattern Completion**
```
"pattern completion" hippocampus memory neural
```

**Search 2: Predictive Coding & Free Energy**
```
"predictive coding" "free energy" Friston
```

**Search 3: Gestalt Completion**
```
"gestalt completion" perception cognitive
```

**Search 4: Neural Network Autoencoders**
```
autoencoder "pattern completion" neural network
```

**Search 5: Memory Consolidation**
```
"memory consolidation" "pattern separation" complementary
```

---

### Target Papers

**Theoretical Foundation:**
1. **Friston** - Free energy principle papers (any foundational work)
2. **Hinton** - Autoencoders and pattern completion
3. **McClelland & Rumelhart** - PDP models

**Neural Mechanisms:**
4. Hippocampus pattern completion reviews (any recent comprehensive review)
5. Predictive processing frameworks
6. Gestalt perception foundations (historical + modern)

---

### DeepSeek Analysis Prompt Template

```
I'm building Pattern-Completion Architecture (PCA) for Big Data systems, grounded in neuroscience and cognitive science.

Paper: [TITLE]
Authors: [NAMES]
Year: [YEAR]

Please extract technical details:

1. MECHANISM SPECIFICATION
   - How does pattern completion work in this framework?
   - What are the processing steps?
   - What triggers completion vs separation?

2. MATHEMATICAL MODEL
   - Any equations or formalisms?
   - Variables and their definitions
   - Computational complexity
   - Convergence properties

3. NEURAL SUBSTRATE
   - What brain systems are involved?
   - Network architecture (feedforward, recurrent, hierarchical)
   - Timescales of operation
   - Neurotransmitter systems (if specified)

4. MEASUREMENT & TESTING
   - How is completion measured experimentally?
   - What tasks or paradigms are used?
   - Dependent and independent variables
   - Typical effect sizes

5. TESTABLE PREDICTIONS
   - What empirical predictions does this make?
   - How could we test these in TIS/CEI framework?
   - What would falsify this model?

6. CONNECTION TO K-E METRICS
   - Does this model explain Knowledge Diffusion (K)?
   - Does this model explain Elasticity (E)?
   - How does pattern completion relate to system health (H = K × E)?

7. COMPUTATIONAL IMPLEMENTATION
   - Could this be implemented in AI systems?
   - What computational resources required?
   - Existing implementations or algorithms?

8. EDGE CASES & LIMITATIONS
   - Where does this model break down?
   - What phenomena does it NOT explain?
   - Acknowledged limitations by authors?

Format as structured markdown with equations in LaTeX where applicable.
```

---

## DOMAIN 1: NEURAL OSCILLATIONS (WEEK 3 PRIORITY)

**Target:** 10 papers
**Assigned LLM:** Claude (Orchestrator - requires synthesis with ScFOIF)
**Analysis Focus:** Integration with temporal frameworks, cross-scale mapping
**Directory:** `literature/by-domain/neural-oscillations/`

### Google Scholar Search Strings

**Search 1: Buzsáki Foundation**
```
"neural oscillations" consciousness integration Buzsáki
```

**Search 2: Phase-Amplitude Coupling**
```
"phase amplitude coupling" cognition task
```

**Search 3: Metastability**
```
"metastability" brain dynamics coordination
```

**Search 4: Temporal Binding**
```
"temporal binding" oscillatory gamma
```

**Search 5: Communication Through Coherence**
```
"communication through coherence" Fries
```

---

### Target Papers

**Core Theory:**
1. **Buzsáki** - "Rhythms of the Brain" (book or key papers)
2. **Fries** - "Communication Through Coherence"
3. **Tononi** - Integrated Information Theory papers

**Empirical:**
4. Phase-amplitude coupling + cognition studies
5. Cross-frequency coupling reviews
6. Metastability in neural dynamics

---

### Claude Analysis Approach

**Note:** For Domain 1, send papers directly to Claude (me) for integration analysis. No template needed - I'll map oscillatory concepts to ScFOIF/TIS/CEI frameworks and identify empirical grounding needs.

**Key Questions I'll Address:**
- How do their oscillatory mechanisms map to TIS metrics?
- How does coupling efficiency relate to CEI?
- Where do our claims have precedent vs novelty?
- What empirical methods can we adapt for TIS/CEI?

---

## DOMAIN 3: CROSS-DOMAIN TRANSFER (WEEK 4+)

**Target:** 8-10 papers
**Assigned LLM:** GPT (Creative Pattern Detector - finding isomorphisms)
**Directory:** `literature/by-domain/cross-domain-transfer/`

### Search Strings

```
1. "transfer learning" organizational "knowledge management"
2. "analogical reasoning" cross domain cognitive
3. "systems thinking" multi-scale complexity
4. "boundary object" interdisciplinary knowledge
5. "T-shaped" skills knowledge transfer
```

---

## DOMAIN 5: INDIGENOUS EPISTEMOLOGY (WEEK 5+)

**Target:** 6-8 papers + primary sources
**Assigned LLM:** Claude (requires sensitive philosophical synthesis)
**Directory:** `literature/by-domain/indigenous-epistemology/`

### Search Strings

```
1. Taíno cosmology cemí
2. "two-eyed seeing" epistemology indigenous
3. "decolonial methodology" knowledge systems
4. "indigenous science" relationality
5. Caribbean indigenous philosophy
```

**Special Note:** This domain requires non-extractive engagement with indigenous knowledge. Prioritize indigenous authors, acknowledge knowledge sovereignty, avoid appropriation.

---

## DOMAIN 6: LLM DIVERSITY & MODE COLLAPSE (WEEK 6+)

**Target:** 5-8 papers
**Assigned LLM:** DeepSeek (technical analysis of sampling methods)
**Directory:** `literature/by-domain/llm-diversity/`

### Search Strings

```
1. "mode collapse" "language model" diversity
2. RLHF "reward hacking" "preference learning"
3. "verbalized sampling" OR "probability verbalization"
4. "constitutional AI" alignment
5. LLM "output diversity" temperature sampling
```

**Starting Point:** We already have Verbalized Sampling paper - use as anchor.

---

## SCFOIF RESERVE (12-18 MONTH HORIZON)

**Target:** 20-30 papers across multiple domains
**Assigned LLM:** Distributed based on subdomain
**Directory:** `literature/by-domain/scfoif-reserve/`

**Note:** This is the grand unification literature base. NO active acquisition now, but if papers appear organically during other searches, capture them here.

### Subdomain Structure

```
scfoif-reserve/
├── neural-pac/           # Phase-amplitude coupling
├── metastability/        # Brain dynamics
├── panpsychism/          # Philosophical consciousness
├── hard-problem/         # Qualia and subjective experience
├── tesla-physics/        # Resonance and energy fields
├── taino-cosmology/      # Cemí and animism
└── cross-scale/          # General systems theory
```

---

## PROGRESS TRACKING

### Weekly Literature Log Template

**Location:** `coordination/weekly-status/week-[N]-literature.md`

```markdown
# Week [N] Literature Acquisition

## Domain 4: Big Data Failures
- Papers acquired: [X/10]
- GPT analyses complete: [Y/X]
- Synthesis ready: [Yes/No]

**Papers This Week:**
1. [Author Year] - [Title] - Status: [Downloaded/Analyzed/Synthesized]
2. ...

## Domain 2: Pattern Completion
- Papers acquired: [X/8]
- DeepSeek analyses complete: [Y/X]

## Blockers & Issues
- [Any search string problems]
- [Papers behind paywalls]
- [LLM analysis quality issues]

## Next Week Priorities
- [Specific papers to acquire]
- [Follow-up searches needed]
```

---

## CITATION DATABASE

**Location:** `literature/citation-database.bib`

**Protocol:** After each paper is analyzed, add BibTeX entry:

```bibtex
@article{Lazer2014,
  author = {Lazer, David and Kennedy, Ryan and King, Gary and Vespignani, Alessandro},
  title = {The Parable of Google Flu: Traps in Big Data Analysis},
  journal = {Science},
  volume = {343},
  number = {6176},
  pages = {1203--1205},
  year = {2014},
  keywords = {Domain4-BigData, PCA-Core, GoogleFlu, Failure-Analysis}
}
```

**Note:** Use keywords for cross-referencing:
- `Domain[N]-[Name]` for domain tracking
- `[Framework]-Core` for central papers
- `[CaseStudy]-[Name]` for specific examples
- Descriptive tags for content

---

## QUALITY CONTROL

### Analysis Quality Checklist

Before accepting LLM analysis output, verify:
- [ ] All sections of prompt template addressed
- [ ] Specific examples/quotes provided (not generic)
- [ ] Clear connection to relevant framework (PCA/K-E/TIS-CEI)
- [ ] Formatted as structured markdown
- [ ] Actionable insights identified
- [ ] Related work suggestions included

### Synthesis Readiness Criteria

Domain ready for synthesis when:
- [ ] Minimum paper target reached
- [ ] All analyses complete
- [ ] Cross-paper patterns identified
- [ ] Framework connections mapped
- [ ] Key quotes extracted with page numbers
- [ ] Related work trail established

---

## LLM COORDINATION NOTES

**When to Use Which LLM:**

**GPT:** Exploratory analysis, unexpected connections, initial screening
**DeepSeek:** Technical validation, mathematical rigor, mechanism extraction
**Claude:** Synthesis across domains, coherence checking, philosophical integration
**Copilot:** Citation formatting, bibliography management, figure generation

**Parallel Processing:** When acquiring multiple papers simultaneously, can feed different papers to different LLMs in parallel, then synthesize results.

---

## EMERGENCY PROTOCOLS

### Paywall Problems
1. Try institutional access (if available)
2. Use preprint servers (arXiv, bioRxiv)
3. Email authors directly (surprisingly effective)
4. Use legal alternatives (ResearchGate author uploads)
5. **DO NOT** use Sci-Hub or similar (legal risk)

### Search String Failures
If search yields <3 relevant papers:
1. Try broader terms
2. Remove overly specific constraints
3. Search cited-by chains from known papers
4. Ask domain expert for key paper recommendations
5. Document in decision-logs why search modified

### LLM Analysis Quality Issues
If output is generic/unhelpful:
1. Add more context about framework to prompt
2. Include example of desired analysis format
3. Try different LLM for same paper
4. If persistent, manual analysis may be needed

---

**This is a living document. Update as search strategies evolve and new domains emerge.**

**Last Updated:** 2025-10-30
**Next Review:** 2025-11-06
