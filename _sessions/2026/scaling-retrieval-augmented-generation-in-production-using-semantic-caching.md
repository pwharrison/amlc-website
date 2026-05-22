---
layout: session-2026
title: "Scaling Retrieval-Augmented Generation in Production using Semantic Caching"
permalink: /2026/sessions/scaling-retrieval-augmented-generation-in-production-using-semantic-caching/
youtube_id: 0BMM_JGPddI
---

# Scaling Retrieval-Augmented Generation in Production using Semantic Caching

**Friday, April 17, 2026 · 2:35 PM – 3:05 PM · Violet Crown Charlottesville**

---

Retrieval-Augmented Generation (RAG) has become a foundational architecture for building enterprise-grade Large Language Model applications. However, teams moving RAG systems from prototype to production often encounter unexpected challenges related to latency, infrastructure cost, repeated retrieval operations, and scalability under real-world user traffic.

Many deployed systems treat each incoming prompt as a completely new request, triggering fresh document retrieval and model generation even when similar queries have already been processed before. This results in redundant computation, increased response time, and higher operational costs, especially at scale.

This session explores how semantic caching can be introduced as an infrastructure layer within production RAG pipelines to improve system performance and efficiency. By leveraging embedding similarity, semantic caching enables systems to identify semantically equivalent or highly related user queries and reuse previously computed retrieval results or generated responses, rather than repeating the entire pipeline.

Drawing from real-world experience deploying enterprise AI systems, this talk will walk through architectural patterns for integrating semantic caching into RAG workflows using vector similarity search. We will discuss practical considerations such as cache hit optimization, freshness trade-offs, observability, and cache invalidation strategies in dynamic knowledge environments.

Attendees will gain insight into how semantic caching can reduce redundant retrieval and generation steps, improve response latency, and optimize compute usage without significantly impacting response quality. The session will also highlight deployment trade-offs and lessons learned from implementing these techniques in production-scale AI platforms.

This talk is intended for ML Engineers, Applied Data Scientists, MLOps practitioners, and Backend Engineers working on LLM-powered applications who are looking to improve scalability and efficiency in real-world deployments.

## About the Speaker

<div class="speaker-profile">
    <div class="speaker-profile-headshot">
    <img src="/assets/images/2026/speakers/Sravani_Lingam.jpg" alt="Sravani Lingam">
  </div>
  <div class="speaker-profile-info">
    <h3>Sravani Lingam</h3>
    <p><em>Manager, Science</em></p>
    <p>Sravani Lingam is a Software Engineering Lead at Infor with a decade of experience building large-scale enterprise platforms and AI/ML-driven solutions. She has led cross-functional teams to design cloud-native architectures, NLP systems, and automation pipelines that deliver measurable cost savings and business impact. Her expertise spans Generative AI, data engineering, microservices, and technical leadership, with a strong focus on translating cutting-edge technology into production-ready systems. Beyond her technical contributions, Sravani is passionate about mentorship, innovation culture, and empowering teams to deliver responsible, scalable AI.</p>
  </div>
</div>
