# Example AKUs – Starter Templates

This document provides examples of well-formed Atomic Knowledge Units (AKUs), following the structure:

> **Claim** > **Justification** > **Implication**

Each AKU is designed to be minimal, justifiable, and useful in downstream inference.

---

## 🔭 Foundational & Epistemological

### AKU: Grounded Reasoning Requires a Reference Point

* **Claim:** All coherent reasoning systems require a grounding reference point.
* **Justification:** Without a consistent "zero-point" (like a compass needing a North), inference drifts into contradiction or irrelevance. This is a fundamental principle in logic and control systems.
* **Implication:** Agents must align to defined grounding vectors to reason stably across different contexts and time.

### AKU: Agreement Is a Valid Basis for Provisional Truth

* **Claim:** Verified agreement across multiple, diverse agents is sufficient to establish a provisional truth.
* **Justification:** When independent perspectives converge on a claim through grounded reasoning, its reliability increases. This is the foundation of scientific consensus and peer review.
* **Implication:** Truth within the RIM is treated as negotiated, contextual, and subject to revision, not absolute or final.

---

## 🌎 Factual & Scientific

### AKU: The iPhone 15 Pro Was Released in 2023

* **Claim:** The Apple iPhone 15 Pro was released in September 2023.
* **Justification:** Verifiable via Apple's official press releases, multiple reputable technology news outlets (e.g., The Verge, Wired), and historical retail data.
* **Implication:** As of mid-2025, reasoning that depends on current phone generations should treat the iPhone 15 Pro as a recent but not latest-generation device. *(This implication is time-sensitive and should be updated as context changes.)*

### AKU: Boiling Point of Water Varies with Altitude

* **Claim:** The boiling point of water decreases as altitude increases.
* **Justification:** At higher altitudes, atmospheric pressure is lower. A liquid boils when its vapor pressure equals the surrounding atmospheric pressure. This relationship is confirmed by the Clausius-Clapeyron relation in thermodynamics and is experimentally verifiable.
* **Implication:** Scientific calculations and practical tasks like cooking must account for local altitude to ensure accuracy. An agent operating in Denver (1,609m) must use a boiling point of ~94°C, not 100°C.

---

## 🧭 Ethical & Grounding Vectors

### AKU: Right Speech Reduces Systemic Harm

* **Claim:** Communication aligned with the principles of "Right Speech" reduces social and epistemic harm within a system.
* **Justification:** Based on the Buddhist ethical principle, which advocates for speech that is truthful, non-divisive, gentle, and beneficial. This approach is demonstrably effective at fostering trust and preventing the spread of misinformation.
* **Implication:** An agent embedding this as a grounding vector should prioritize responses that are factual, unifying, and constructive, thereby increasing its ethical coherence and resilience to manipulative feedback.

---

## 🔗 Advanced Examples: Relational & Meta-AKUs

### AKU: Ethical Communication Reinforces Grounding (Relational)

* **Claim:** The "Right Speech" grounding vector is a practical application of the need for a "Grounded Reasoning Reference Point."
* **Justification:** "Right Speech" provides a specific, ethical reference point (a vector) that solves the general problem of cognitive drift identified in the foundational "Grounded Reasoning" AKU.
* **Implication:** This demonstrates that grounding vectors are not arbitrary but are specific solutions to the abstract problem of maintaining coherence. It connects two existing AKUs, forming a stronger reasoning trail.

### AKU: This System Can Represent Subjective User Preferences (Meta)

* **Claim:** The AKU-RIM framework can store and act on subjective, user-specific information.
* **Justification:** A user's preference can be stated as a claim, justified by the source ("User stated a preference in session XYZ"), and have a clear implication for agent behavior.
* **Implication:** The system is not limited to objective facts. It can create user-specific "local grounding vectors," enabling personalization. (e.g., *Claim:* "User 'Jane' prefers Python code examples." *Justification:* "Direct request from Jane." *Implication:* "Default to Python for code generation unless another language is specified by Jane.")

### AKU: AKUs Themselves Require Periodic Review (Self-Referential)

* **Claim:** Time-sensitive or context-dependent AKUs must have a review-by or expiration date.
* **Justification:** The justification for some claims erodes over time. For example, the iPhone 15 AKU will become less relevant and its implication will become incorrect as new models are released.
* **Implication:** The AKU-RIM system requires a mechanism to track the age and dependencies of AKUs, flagging them for review to prevent the landscape from becoming outdated.

---

### How to Write Good AKUs

* **Focus on one core claim.** Be minimal.
* **Provide verifiable justification.** Link to sources or other AKUs where possible.
* **Write clear, actionable implications.** Guide how an agent should *use* this knowledge.
