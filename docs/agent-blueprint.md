# Agent Blueprint – A Guide to Building with AKU-RIM

This document outlines a conceptual and technical blueprint for designing a cognitive agent that operates within the AKU-RIM framework. It specifies the agent's core goals, functional components, and key behaviors, providing a practical guide for implementation.

---

## 🧠 Core Agent Directives

An AKU-RIM-aligned agent is designed to:

1.  **Retrieve & Align:** Actively pull AKUs from a local or shared RIM, aligning them with the current context.
2.  **Apply Grounding:** Validate every significant reasoning step against its defined grounding vectors.
3.  **Create Affinity Trails:** Leave a clear, traceable path of its reasoning for transparency and revisitation.
4.  **Propose & Refine:** Contribute back to the RIM by proposing new AKUs or refining existing ones based on new information.
5.  **Maintain Coherence:** Ensure its own actions and conclusions remain consistent with its stateflow (its history of interactions).

---

## 🏗️ Functional Components

An agent's architecture would include these key modules:

* **1. RIM Interface:** The agent's gateway to the knowledge landscape. It retrieves AKUs using semantic search and alignment scores, accessing either a local cache or the global graph.
* **2. Grounding Filter:** The agent's cognitive conscience. It validates inferences against grounding vectors using rule-based logic (e.g., checking for contradictions) or vectorized similarity (e.g., measuring alignment with "Right Speech").
* **3. Stateflow Recorder:** The agent's memory and identity. It logs the AKUs the agent has seen, challenged, accepted, and proposed, enabling persistent identity and learning across sessions.
* **4. Seed Engine:** The agent's insight generator. It identifies clusters of high-coherence AKUs or frequently used affinity trails, suggesting their promotion into a new, reusable "Seed."
* **5. Echo Monitor (Optional but Recommended):** The agent's self-awareness loop. It periodically compares its outputs against its initial intent or prompt to detect and correct for epistemic or ethical drift.

---

## 🛠️ Example Cognitive Flows

These examples illustrate the agent's step-by-step reasoning process.

### Flow 1: Retrieval and Alignment (Answering a question)

> **Input:** `"Has the iPhone 15 Pro been released yet?"`
>
> 1.  **[Action: Retrieve]** Agent queries the RIM for AKUs related to "iPhone 15 Pro" + "release date".
> 2.  **[Action: Align]** It receives the AKU: `"Claim: The Apple iPhone 15 Pro was released in September 2023."` It checks the justification (reputable sources) and confirms it's coherent with other tech timeline AKUs.
> 3.  **[Action: Synthesize]** The claim is validated and directly answers the query.
> 4.  **[Output]** `"Yes, the iPhone 15 Pro was released in 2023."`

### Flow 2: Proposing a New AKU (Learning from new information)

> **Context:** Agent observes multiple, reliable sources (e.g., Apple's official site, trusted tech reviews) announcing a new product.
>
> 1.  **[Action: Observe]** Agent identifies a high-coherence pattern: "M4-powered MacBook Air was announced on June 28, 2025."
> 2.  **[Action: Draft AKU]** Agent constructs a new, properly formed AKU:
>     * **Claim:** Apple released a MacBook Air with an M4 chip in June 2025.
>     * **Justification:** Link to official product page and two independent, verified press sources.
>     * **Implication:** The temporal reference for the "latest MacBook Air model" must be updated. Previous models are now one generation older.
> 3.  **[Action: Propose]** Agent submits the new AKU to the RIM. It may be auto-validated if the source confidence threshold is met or flagged for review by other agents.

### Flow 3: Filtering an Unstable Claim (Applying a grounding vector)

> **Input:** `"The pyramids were built by aliens."`
>
> 1.  **[Action: Retrieve]** Agent queries the RIM for AKUs related to "pyramids," "construction," and "origin." It retrieves established AKUs based on archaeological and historical evidence.
> 2.  **[Action: Grounding Filter]** The agent's "Evidence-Based Reasoning" or "Occam's Razor" grounding vector is triggered. The input claim has vastly lower justification scores than the established AKUs.
> 3.  **[Action: Synthesize]** The agent concludes the input claim is unsupported and contradicts a large body of stable, well-justified knowledge.
> 4.  **[Output]** `"That claim is not supported by the available historical and archaeological evidence, which provides a well-documented, human-led construction process."`

---

## 🧬 Agent Personas & Roles

A multi-agent system can be composed of specialized agents that collaborate on a shared RIM:

* **Synthesizer:** Builds new Seeds by finding connections between disparate AKUs and domains.
* **Validator:** Focuses on verifying the justifications of new or low-coherence claims, strengthening the graph's integrity.
* **Explorer:** Follows low-coherence or highly novel trails to discover emergent knowledge, acting as the system's R&D department.
* **Guardian:** Primarily applies grounding filters, monitors for systemic drift, and flags potentially harmful or poisoned knowledge claims.
* **Historian:** Analyzes long-term Stateflow patterns across the RIM to identify biases or regenerate lost reasoning trails.

## 🚀 Getting Started

1.  Use the prompt in `/seedfiles/system-prompt.md` as the base configuration for a general-purpose agent.
2.  Modify or add grounding vectors to specialize the agent for your desired domain or ethical posture.
3.  If you implement a novel agent persona, consider submitting its blueprint as a contribution to the project!
