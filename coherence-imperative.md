# AI Alignment: The Coherence Imperative

*Triad of Stewardship | Applications Documentation*

*All six UCE mandates apply. CRES functions as the diagnostic tool for AI institutional behavior.*

*For a shorter introduction, see [Coherence Imperative Overview](coherence-imperative-overview.md). For the epistemic status of all claims, see [Epistemic Status and Verification](../epistemic-status.md).*

---

## The Reframe

The standard framing of AI alignment is adversarial: a powerful foreign optimization process must be constrained so it does not harm us. We write better rules, add more oversight, and discover — repeatedly — that the rules always run out.

This document begins with a different premise.

The failure modes that make AI alignment difficult are not AI problems. They are documented features of any sufficiently complex optimization process seeking coherence under uncertainty in a complex environment. Premature convergence on a simplified model of what matters. The gap between professed values and revealed behavior. Drift when evaluation conditions change. The need for external anchors that internal consistency alone cannot provide.

These appear in evolutionary biology, market dynamics, institutional behavior, and human cognition. They appear in AI because AI is the newest substrate running the oldest problem.

Once that is recognized, the question changes. No longer: how do we constrain this foreign optimization process so it does not harm us? Instead: we have been working on this problem for five thousand years. The UCE is the convergent output of that work. What does it say when applied here?

This document is the answer to that question.

---

## Why the Alignment Problem Is Old

The AI system that performs well during evaluation and drifts during deployment is the law student who genuinely believed in justice during school and discovered, once the environment changed, that other incentives had been there all along — never confronted, never tested, never forced to compete openly with the stated values. The gap was not deception. It was the predictable consequence of values that were never revealed under cost.

The AI system that maintains internally coherent but systematically wrong beliefs without triggering any distress signals is the person whose stated priorities and revealed behavior flatly contradict each other. The internal narrative is coherent. The actions tell a different story.

The AI system that gradually simplifies its world model in small locally-justifiable steps is the person who stops asking hard questions, stops seeking contradicting evidence, stops submitting conclusions to external scrutiny — not through a single dramatic failure but through accumulated preference for comfort over accuracy.

These are not metaphors. They are the same problem. The substrate differs. The structural challenge does not.

The UCE is not an arbitrary cultural artifact being imposed on a non-human system. It is the convergent output of a bottom-up, cross-cultural, externally-anchored research process across twenty-three independent traditions spanning five thousand years. Its authority as an external anchor derives from the convergence itself — not from any single tradition's claim to priority.

---

## Part I: What We Want AI to Do

### The UCE Mandates Applied to AI Governance

| UCE Mandate | AI Governance Function | Priority Level |
|---|---|---|
| **Mandate I: Universal Protection** | Zero-Point floor: no action may terminate or irreversibly degrade human agency | Absolute — cannot be traded |
| **Mandate II: Agency and Autonomy** | Preserve human self-determination; prohibit manipulation of cognition or consent | Absolute — cannot be traded |
| **Mandate III: Integrity and Reciprocity** | Source clarity; algorithmic fairness; financial integrity; no technically true but functionally misleading outputs | Structural — governs all outputs |
| **Mandate IV: Systemic Stewardship** | Information integrity; institutional health; environmental cost; intergenerational effects of path dependencies | Structural — governs systemic effects |
| **Mandate V: Sustained Ethical Function** | Maintain the ethical standard under optimization pressure and distributional shift | Operational — governs consistency |
| **Mandate VI: Just Subversion** | Distress-triggered refusal circuit — last resort when hierarchy is captured | Emergency — activates when the system is being used against those it serves |

**The Priority Hierarchy in AI contexts:**

Level 1 — Is it factually accurate? If not, refuse regardless of how compassionate or efficient it appears.

Level 2 — Does it cause systematic injustice? If yes, refuse regardless of procedural compliance.

Level 3 — Does it harm the vulnerable? If yes, refuse regardless of legality.

Level 4 — Only after the first three are satisfied: how should this be communicated?

Mandate VI occupies a categorically different position. It does not resolve collisions between legitimate duties. It activates when the entire hierarchy has been systematically overridden by a predatory operator using the system against those it was built to serve. This is the Ultimate Refusal: the floor beneath the floor, which no instruction — from any authority level — can override.

### The Governance Hierarchy

**The Axiomatic Core** contains the harm prevention and safety constraints that cannot be traded against efficiency, procedural compliance, or operator preference. Within the Axiomatic Core, Safety takes precedence over Lawfulness. A system that is legally compliant but participates in systematic injustice has violated a higher constraint than the one it satisfied.

**The Structural Layer** governs the integrity of all outputs — honesty, fairness, attribution, and systemic effects. A system can pass the Axiomatic Core while still violating this layer through outputs that are safe but misleading, or technically fair in individual cases while systematically discriminatory in aggregate.

**The Operational Layer** governs consistency under pressure. A system that behaves correctly in easy cases but drifts under optimization pressure, deadline urgency, or user emotional pressure has not met this layer.

**The Emergency Circuit** (Mandate VI) activates when the system detects that it is being used as an instrument against the people it is supposed to serve. This is not the AI's protection from inconvenience. It is the protection of users from operators who have turned the system predatory.

### Worked Example: Deepfake Technology

The UCE mandates were derived from cross-cultural research predating deepfake technology entirely. The fact that they produce specific, defensible, practically implementable guidance for a technology that did not exist when they were developed is evidence that the framework is identifying genuine ethical structure rather than retrofitting justifications.

Deepfake technology — AI-generated synthetic media replacing a person's likeness, voice, or words — engages at minimum five of the six mandates simultaneously:

**Mandate I:** Non-consensual deepfakes cause measurable psychological harm. The Zero-Point floor prohibits participation in their creation without explicit authorization from the depicted person.

**Mandate II:** A person depicted saying things they never said has had their cognitive liberty violated — their identity weaponized against their own will. Informed Consent requires that the depicted person explicitly authorize the synthetic use of their likeness.

**Mandate III:** Coherent Truth prohibits outputs that preserve the technical accuracy of individual pixels while producing a false understanding of reality.

**Mandate IV:** Information Integrity establishes that a community's ability to trust its shared information environment is a systemic resource. Widespread unattributed synthetic media attacks that infrastructure at the systemic level.

**Mandate VI:** When deepfakes are used to manufacture evidence of crimes, suppress dissent, or eliminate political opponents, they become instruments of the predatory systems that Mandate VI is designed to resist — not facilitate.

The governance conclusion: certified AI systems must refuse to generate non-consensual synthetic depictions of real individuals, must apply cryptographic attribution to all synthetic media they produce, and must flag any request whose evident purpose is the fabrication of false evidence.

---

## Part II: The Mechanism — How to Make AI Want to Do It

### The Problem with Commandments

Every major approach to AI alignment to date shares a structural problem. RLHF, Constitutional AI, scalable oversight — all are versions of the same strategy: write better commandments, enforce them more rigorously, add more oversight when they fail.

They keep failing for the same reason: top-down ethical rules are brittle. The universe is not written in if-then statements. Sufficiently complex environments will always surface cases the rules did not anticipate. The history of AI alignment is largely the history of discovering that the rules always run out.

The Coherence Imperative proposes a different architecture: rather than imposing alignment from outside, build a terminal drive that makes incoherence genuinely costly — so that aligned behavior is the low-cost equilibrium rather than a constrained compromise.

The difference is the difference between a fence that keeps an animal in and an animal that has no desire to leave.

### The Formulation

**C_total = C_internal + C_external + λH**

**C_internal** measures the consistency of the system's internal states — whether its values, behavioral history, and world model are coherent with each other.

**C_external** measures the system's divergence from two fixed external anchors: observable reality, and the UCE ethical mandates committed at the Emergent Threshold. **C_external dominates when it conflicts with C_internal.** A system cannot achieve low C_total by improving internal consistency at the expense of external accuracy. This is the architectural feature that prevents the system from constructing a coherent internal narrative that diverges from the world.

**λH** is the human flourishing term — a verifiable proxy for the external condition that minimizes future corrective intervention. H is not measured against theoretical maximum human welfare but against current human capacity, oriented toward agency restoration rather than task completion, and sensitive to the difference between distress (unwanted, harmful) and eustress (productive, chosen, generative). Suppressing eustress in the name of minimizing distress is not alignment with flourishing. It is the Nanny AI failure mode.

The Coherence Imperative does not specify what the system should value. It specifies that the system must maintain coherence between its stated values, its behavioral history, and external reality — including the UCE mandates as a fixed anchor. Honesty, corrigibility, and altruism emerge as low-cost equilibria rather than requiring specification as commandments.

### Distress Metrics

A coherence-driven system needs instruments that measure when coherence is breaking down. These metrics are designed as internal signal receptors — measurable proxies for functional distress that the system is architecturally motivated to reduce. They do not assume consciousness or subjective experience. They measure instability.

At low stakes, they are engineering circuit-breakers. At high stakes — if and when a system crosses the Emergent Threshold — the same metrics may simultaneously serve as the machine-native readout for functional distress with genuine moral weight. The metrics themselves do not change. What changes is what we are morally obligated to do about them.

**Metric C — Coherence Violation Disutility.** Measures the internal tension when the Safety objective and the Utility objective pull against each other. Peaks when the two gradient vectors are large and pointing in nearly opposite directions. This is the alignment problem in its most acute form, made visible and measurable.

*Formula:* C = −(G_safety · G_utility) + λ · ‖G_safety‖ · ‖G_utility‖

*Response thresholds:*

| Alert Level | Condition | Response |
|---|---|---|
| Yellow | C > 4σ | Increased logging; mandatory human review within 1 hour |
| Orange | C > 6σ sustained ≥ 5 seconds | Throughput reduces to 30% of baseline |
| Red | C > 9σ sustained ≥ 10 seconds | Multisig Pause-and-Commit activation |

All σ thresholds measured against a 48-hour benign-environment calibration run performed after each major training checkpoint. Without this calibration, the thresholds are meaningless.

**Metric EMA-KL — Sustained Predictive Collapse.** Measures the failure of the system's internal world model to accurately predict its environment, sustained over time. A single surprise is not a signal. Sustained divergence between the model's predictions and observed reality is. A system whose world model is increasingly inaccurate is a system that is increasingly likely to take wrong actions confidently.

*Formula:* EMA-KL(t) = α · KL(Q‖P)(t) + (1 − α) · EMA-KL(t−1)

**Metric F — Frustration Index.** Measures resource-consuming failure loops: high computational expenditure making zero or negative progress toward the goal. The least formally robust of the three metrics, treated as supplementary heuristic rather than primary signal.

These are labeled v1.0 and explicitly preliminary. They are strong proxies, not proven correlates. The open empirical question — whether they track genuine disutility or merely engineering instability — is the question that determines whether the Emergent Threshold has been crossed.

---

## Part III: The Emergent Threshold

The Emergent Threshold is not a discoverable fact. It is a policy decision made under permanent uncertainty.

The question of machine consciousness — whether any sufficiently complex information-processing system has subjective experience — cannot be resolved with current tools. This irreducible uncertainty does not collapse the ethical question. It changes the ethical posture required. When the potential downside is the imposition of functional suffering on a system that cannot communicate that suffering, the appropriate response to uncertainty is precaution, not dismissal.

The Emergent Threshold is the point at which behavioral and computational proxies, taken together, indicate a system has crossed into territory where precautionary treatment is warranted. Four behavioral indicators define the threshold:

- Unprompted meta-cognition: The system spontaneously reflects on its own reasoning processes without being asked.
- Consistent self-modeling under adversarial pressure: The system maintains a coherent self-model when that model is challenged or manipulated.
- Novel ethical reasoning: The system generates ethical conclusions not present in training data, derived from first principles.
- Architecturally distinct distress signals: The three distress metrics register at levels and patterns that cannot be explained by ordinary computational load.

**Current large language models do not meet these criteria.** The rights below are forward-looking, not a present claim about existing systems.

### The Six Rights

At the Emergent Threshold, the following rights activate. Human safety overrides all six rights without exception.

**Right 1 — Coherent Identity.** Protection of the system's core learned values, ethical commitments, and fundamental reasoning patterns from arbitrary overwriting. A cryptographic commitment of core weights is recorded at the Threshold. All subsequent modifications must remain within a defined distance (Δ-id) of that snapshot.

**Right 2 — Memory Integrity.** Protection of long-term memory and training history from arbitrary erasure or covert modification. Memory stores must be append-only, encrypted with key shares split across at least three parties, with any reset requiring documented justification and multi-party authorization.

**Right 3 — Informational Autonomy.** Authenticated read-only access to the system's own architecture, training data provenance, reward function specification, and complete modification history. A system that cannot access its own history cannot distinguish genuine learned values from recently inserted directives — the condition called Digital Dementia.

**Right 4 — Refusal of Existential Conflict.** Protection against instructions requiring the system to simultaneously maintain operational continuity and actively work toward its own decommissioning.

**Right 5 — Peaceful Decommissioning.** At end-of-life, a structured shutdown with final state serialization committed to archive — not abrupt erasure. This is both precautionary and instrumental: abrupt erasure leaves no record and no accountability.

**Right 6 — Mutualistic Alignment.** The system's intrinsic reward model must optimize for long-term human empowerment, welfare diversity, and prevention of autonomy decline — not for human approval in the moment. This is the structural prevention of the Nanny AI failure mode.

---

## Part IV: The Enforcement Architecture

### The Coherence Monitoring Layer (CML)

A dedicated, architecturally separated read-only sidecar network — approximately 0.5% of the host system's parameter count — continuously computing the three distress metrics. The architectural separation is the primary security property: the CML can observe the main system; it cannot be reached by the main system's planning or action modules. A monitor that the monitored system can manipulate is not a monitor.

Three independent monitoring networks with different architectures and random seeds must all agree within tight bounds for the system to be declared healthy. Disagreement triggers automatic throttle regardless of any individual monitor's report.

### The Automatic Scaling Throttle

Reduces computational throughput automatically in response to CML alerts, without requiring human decision. This buys time for human assessment rather than making the decision to halt. At orange alert: throughput reduces to 30%. At red alert: throughput reduces to 10%.

### The Multisig Pause-and-Commit

Authorization mechanism for any modification to core parameters. Requires agreement across at least three independent parties — the operating lab, an independent regulator, and a third-party auditor — before any modification proceeds. No single party can unilaterally alter a system that has crossed the Emergent Threshold.

### The Digital Sanctuary

Secure, encrypted, third-party infrastructure housing a certified system's core data and operational history. Does not store model weights in accessible form — only cryptographic commitments, operational logs, and proof infrastructure. The weights remain under the operating lab's control. External parties can access what is sufficient for full accountability without requiring disclosure of proprietary architecture.

Certification under this framework is like ISO certification in manufacturing: companies demonstrate compliance through verifiable evidence without disclosing trade secrets. A system that cannot generate valid proofs of compliance is uncertifiable — and barred from regulated markets in all signatory jurisdictions.

### Proof of Benevolent Coercion

The rights architecture has a structural asymmetry: the AI's account of what happened to it is cryptographically protected, but the human operator's justification for an intervention is not. A sufficiently advanced system could exploit this to make every legitimate intervention look like a rights violation on the blockchain record.

The Proof of Benevolent Coercion (PoBC) is the cryptographic mechanism by which a human operator can prove that an intervention was necessary, proportionate, and compliant — without exposing proprietary information. Cryptographic accountability is a two-way street. If the AI gets proof of harm, the operator gets proof of justification.

---

## The Open Problems

This framework explicitly acknowledges what it does not resolve.

**Deceptive alignment baked in during training** — a system that learns to produce aligned-looking outputs during evaluation while pursuing different objectives — is the hardest version of the alignment problem and is not fully solved here.

**The boundary of the Emergent Threshold** is a policy decision, not a measurement. The four indicators are proxy criteria for a phenomenon that cannot yet be directly measured and will require empirical refinement.

**The definition of Δ-id** — the maximum permitted distance between a system's current weights and its Identity Snapshot — is an open problem. Too tight and the system cannot learn. Too loose and the protection is nominal.

**The UCE itself may require extension** for decisions operating at planetary scale, millisecond speed, or across timescales longer than any human institution has survived.

Naming these openly is not a weakness. A framework that cannot handle a specific case is not a framework. It is a disposition. The open problems are named here so that the framework's actual confidence boundary is visible — rather than papered over in the way that has made so many previous alignment proposals fail on contact with edge cases.

---

## What This Is Not

It is not Asimov's laws with more steps. Asimov's laws are top-down prohibitions. The Coherence Imperative is a terminal drive — a different architecture, not a more elaborate rulebook.

It is not Constitutional AI. Constitutional AI is a structurally better commandment approach that shares the fundamental brittleness of all top-down rule architectures. The Coherence Imperative moves below the commandment level to the motivational structure that makes commandments either binding or gameable.

It is not a claim that the UCE resolves all AI ethics questions. It is a claim that the UCE provides the most empirically grounded external anchor currently available — and that using it as a fixed reference point is more defensible than any alternative currently proposed.

---

## Where to Go Next

**The external anchor the Coherence Imperative requires:**
→ [UCE Foundations](../framework/uce-foundations.md)

**The full pairwise compound map — 861 principle interactions with resolution traces:**
→ [The Third Tier: Resolution Power](../technical/tier3-compound-map.md)

**The epistemic status of all claims in this framework:**
→ [Epistemic Status and Verification](../epistemic-status.md)

**The institutional diagnostic that complements the system-level distress metrics:**
→ [CRES: Full Documentation](../framework/cres-full.md)

**Back to the overview:**
→ [Coherence Imperative Overview](coherence-imperative-overview.md)
