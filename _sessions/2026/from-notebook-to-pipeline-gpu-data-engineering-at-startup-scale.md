---
layout: session-2026
title: "From Notebook to Pipeline: GPU Data Engineering at Startup Scale"
permalink: /2026/sessions/from-notebook-to-pipeline-gpu-data-engineering-at-startup-scale/
youtube_id: 1y4PNhP2yX0
---

# From Notebook to Pipeline: GPU Data Engineering at Startup Scale

**Friday, April 17, 2026 · 1:10 PM – 1:40 PM · Violet Crown Charlottesville**

---

When it's time to scale your data engineering pipeline from "it works on my machine" to hundreds of machines in parallel, picking the right approach can feel overwhelming.  When you factor in GPU compute costs, design mistakes can quickly deplete a startup's runway. Most online resources focus on model training, but when your use case is compute-intensive data engineering, you're largely on your own. That's the problem we faced at Hardshell, a startup focusing on securing companies’ AI data layer, as we built a production data engineering pipeline with no prior ML pipeline experience on the team.  If you're in the same boat, this talk will give you the framework and confidence to tackle it too.

We'll draw from several architectural patterns we implemented on GCP, with cloud platform agnostic strategies applicable to any platform. Because pipelines are never "done," we'll focus on practices that compound over time: building observability in from the start, containerizing steps early for portability, and establishing data versioning to manage inevitable recomputes. We'll also get into the mechanics of cost control: strategic caching and checkpointing, and how routing workloads intelligently between CPU and GPU workers can meaningfully reduce your compute bill.

This isn't a talk about the "right" architecture; it's about how to evaluate your options when you have a tight timeline and need to rapidly bootstrap a solution. You'll walk away with a practical framework for deciding when a managed service is good enough, when it's time to take on the operational complexity of Kubernetes, and how to keep data quality and costs under control along the way.

Who should attend: ML engineers, data scientists, and software engineers building or scaling GPU-accelerated data pipelines, especially at startups where cost and timeline constraints are real. Familiarity with basic cloud concepts is helpful, but deep GCP expertise is not required, as the architectural lessons apply across cloud platforms.

## About the Speaker

<div class="speaker-profile">
    <div class="speaker-profile-headshot">
    <img src="/assets/images/2026/speakers/Ben_Cutter.jpg" alt="Ben Cutter">
  </div>
  <div class="speaker-profile-info">
    <h3>Ben Cutter</h3>
    <p><em>Founding Staff Software Engineer, Hardshell</em></p>
    <p>Ben is the Founding Staff Software Engineer at Hardshell, a Charlottesville based startup working to secure the AI data layer.  Prior to Hardshell, he worked at Indeed for over a decade, working across the stack to improve the employer experience.  He holds a Master's in Systems Engineering from the University of Virginia.</p>
  </div>
</div>
