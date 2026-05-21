---
layout: session-2026
title: "Human-Interpretable ML Explanations in High-Stakes Graph ML"
permalink: /2026/sessions/human-interpretable-ml-explanations-in-high-stakes-graph-ml/
youtube_id:
---

# Human-Interpretable ML Explanations in High-Stakes Graph ML

**Friday, April 17, 2026 · 3:10 PM – 3:40 PM · Auditorium 4**

---

Graph Neural Networks (GNNs) are now powering high-impact systems, from intrusion detection in the security domain to large-scale recommendation engines in the real estate domain, but their adoption still hits the same opaque wall: stakeholders cannot trust what they cannot interpret because black-box Graph ML decisions are not transparent. This session distills two explainability frameworks, ProvExplainer for Intrusion Detection System (IDS) and Z-REx for heterogeneous link-prediction recommendations, into a practical guide for building a human-interpretable, domain-grounded explanation framework for black-box ML pipelines.

We begin with ProvExplainer, which explains GNN-based intrusion detection by mapping GNN predictions into an interpretable explanation space: discriminative subgraph patterns and global structural features that correspond to recognizable attacker behaviors and system dependencies. We show that a specialized domain requires a domain-aware explanation framework, as common GNN explainers struggle in the security domain, whereas ProvExplainer does not. 

We then shift to Z-REx, designed for a gap most explainers struggle with: explaining heterogeneous link prediction (the core of many recommender systems). Z-REx combines feature perturbation with structural perturbation (to isolate influential subgraphs), while using domain heuristics to reduce combinatorial search and keep explanations coherent around the predicted link. We show that, similar to the security domain, the real-estate domain also requires a domain-aware explanation framework, Z-REx.

We expect this session to be helpful for applied ML engineers building graph ML systems, recommender practitioners, security/DFIR data scientists, and researchers who want explanations that hold up to real-world use. Some familiarity with Graph Neural Networks is beneficial, but in the introduction, I will cover the concepts needed to understand the work. 

Concrete takeaways:

- A reusable framework for domain-grounded explanations: choose an interpretable explanation space people understand (subgraphs + attributes).
- Two production-relevant patterns: surrogate-based interpretation (ProvExplainer) and link-focused perturbation (Z-REx).
- How to evaluate explanations beyond a single “fidelity” number (what to measure, and why it matters).
- How to incorporate the explanation methodology is already pre-established ML workflow (security telemetry, marketplaces, fraud graphs, etc.).

## About the Speaker

<div class="speaker-profile">
    <div class="speaker-profile-headshot">
    <img src="/assets/images/2026/speakers/Kunal_Mukherjee.jpg" alt="Kunal Mukherjee">
  </div>
  <div class="speaker-profile-info">
    <h3>Kunal Mukherjee</h3>
    <p><em>Postdoctoral Associate, Virginia Tech</em></p>
    <p>I am a Postdoctoral Research Associate in the Department of Computer Science at Virginia Tech (Blacksburg, VA). I received my M.S. and Ph.D. in Computer Science from The University of Texas at Dallas.

My current research focuses on the adversarial robustness of graph learning and the governed, forensic use of LLMs in system provenance and security operations. I develop agentic, retrieval-augmented pipelines that transform threat reports into actionable signals, and I study how to make GNNs and LLMs trustworthy under real-world attacks and constraints.

Research Focus:
- Agentic RAG for Threat Intel: Designed a retrieval-augmented pipeline where an LLM-based agent parses threat reports and extracts indicators of compromise (IOCs) and TTPs for downstream detection and hunt workflows.
- Adversarial Attacks on GNNs: Building realistic attack generators and evaluation suites for domains beyond system logs, including blockchain and social networks, to stress-test link/node classification and detection tasks.
- LLM-Guided Forensics & Governance: Developing methods for LLM-assisted provenance forensics (triage, explanation, evidence tracing) alongside policy and guardrails for reliable, auditable agent behavior in security settings.</p>
  </div>
</div>
