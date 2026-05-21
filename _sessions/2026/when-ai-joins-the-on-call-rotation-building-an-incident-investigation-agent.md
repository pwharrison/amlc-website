---
layout: session-2026
title: "When AI Joins the On-Call Rotation: Building an Incident Investigation Agent"
permalink: /2026/sessions/when-ai-joins-the-on-call-rotation-building-an-incident-investigation-agent/
youtube_id:
---

# When AI Joins the On-Call Rotation: Building an Incident Investigation Agent

**Saturday, April 18, 2026 · 11:00 AM – 12:30 PM · Classroom 305**

---

As large language models (LLMs) have become widely available, the primary challenge has shifted from model training to system design. Agentic AI represents the next step in this evolution: LLM-powered systems that can reason about tasks, use tools, and iteratively act toward a goal.

One compelling application of agentic AI is incident investigation and response support. In this talk, I’ll walk through the design of a practical agentic AI assistant for incident analysis. Given an alert or error description, the agent gathers relevant context from logs and metrics, correlates signals across tools, and produces a structured incident summary with suggested next steps for engineers.

Using this concrete application as a lens, we’ll roll up our sleeves together walkthrough creating:

• A starter agent loop (observe → plan → act → evaluate)
• Basic tooling (log search, retrieval, and code execution) enables applied agents
• Error handling for common failure modes and safety considerations in incident analysis
• A finished pipeline for incident investigation to be used in multiple scenarios.

The focus is on building a human-in-the-loop system—one that accelerates investigation while remaining safe, interpretable, and auditable. We’ll also discuss how limited, well-scoped actions (such as information gathering or ticket enrichment) can be safely delegated to agents. Attendees will leave with a clear mental model of agentic AI and practical guidance for applying these principles to real-world incident management systems.

## About the Speaker

<div class="speaker-profile">
    <div class="speaker-profile-headshot">
    <img src="/assets/images/2026/speakers/Nathan_Todd.jpg" alt="Nathan Todd">
  </div>
  <div class="speaker-profile-info">
    <h3>Nathan Todd</h3>
    <p><em>MS of Data Science @ UVA | AI Engineering @ Winning by Design</em></p>
    <p>Nathan Todd is a Masters of Data Science candidate at the University of Virginia. He earned a B.S. in Applied & Computational Mathematics from Brigham Young University, with an emphasis on computer science applications.
His experience spans AI engineering, machine learning, and data engineering, with roles at Winning by Design, Data Driven Streets, and Aspen Mountain Partners where he has built production AI solutions, ML pipelines, and data infrastructure. Nathan’s recent work focuses on Agentic AI systems and their integration into modern data and software pipelines, developing intelligent processes that automate workflows and augment human decision-making.</p>
  </div>
</div>
