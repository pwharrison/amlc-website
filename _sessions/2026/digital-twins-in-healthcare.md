---
layout: session-2026
title: "Digital Twins in Healthcare"
permalink: /2026/sessions/digital-twins-in-healthcare/
youtube_id: oaUqzbdublQ
---

# Digital Twins in Healthcare

**Friday, April 17, 2026 · 10:20 AM – 10:50 AM · Violet Crown Charlottesville**

---

Digital twins—computational replicas of real-world systems that stay synchronized with operational data—are moving from manufacturing and aerospace into healthcare. In this talk, I’ll show what “digital twin” means in clinical and operational settings, what it does not mean (a static simulation or a dashboard), and how to build twins that are credible enough to influence real decisions.

We’ll start with a practical taxonomy of healthcare digital twins: (1) operational twins (throughput, capacity, crowding, staffing), (2) patient/physiology twins (risk trajectories, deterioration, response to interventions), and (3) care-process twins (workflows, handoffs, coordination, quality and safety). I’ll then walk through a reference architecture that can be implemented today: data layer (EHR + devices + operational signals), world/state model, causal and statistical components, agent-based and discrete-event simulation options, and AI/LLM “control surfaces” for decision support, note generation, and scenario exploration—while keeping numeric ground truth (vitals/labs) in the world model rather than hallucinated by language models.

Concrete examples will include emergency department use cases: dynamic forecasting of arrivals and bed needs, simulating policy changes (fast track, triage rules, staffing), and evaluating AI interventions (ambient documentation, triage copilots, sepsis alerts) in a sandbox before deployment. We’ll close with a deployment checklist: validation and calibration, governance and auditability, bias/fairness considerations, integration into workflows, and the minimum evidence threshold needed to move from “interesting simulation” to “operational tool.”

Attendees will leave with a clear mental model, a build-vs-buy framework, and an actionable blueprint for starting a digital twin pilot in their own health system.

## About the Speaker

<div class="speaker-profile">
    <div class="speaker-profile-headshot">
    <img src="/assets/images/2026/speakers/Andrew_Taylor.jpg" alt="Andrew Taylor">
  </div>
  <div class="speaker-profile-info">
    <h3>Andrew Taylor</h3>
    <p><em>Professor of Emergency Medicine, University of Virginia</em></p>
    <p>R. Andrew Taylor, MD, MHS is Vice Chair of Research & Innovation in the Department of Emergency Medicine at the University of Virginia. He is a physician-scientist double-boarded in Emergency Medicine and Clinical Informatics with a research portfolio focused on applied AI, data infrastructure, decision support, and diagnostic safety in acute care. His work spans development and evaluation of clinical AI systems, LLM-enabled documentation and chart review tools, and scalable data pipelines (e.g., OMOP/FHIR) to support multi-site research and implementation. He collaborates across health system operations, data science, and engineering to translate computational methods into deployable tools that improve care delivery, safety, and equity.</p>
  </div>
</div>
