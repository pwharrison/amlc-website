---
layout: session-2026
title: "Building Organizational Intelligence with Property Graphs, Agentic AI, and MCP"
permalink: /2026/sessions/building-organizational-intelligence-with-property-graphs-agentic-ai-and-mcp/
youtube_id:
---

# Building Organizational Intelligence with Property Graphs, Agentic AI, and MCP

**Friday, April 17, 2026 · 1:45 PM – 2:15 PM · Auditorium 2**

---

Large organizations are surprisingly opaque. Answering questions like "who owns this product?", "who's responsible for this system?", or "who sells this?" often means navigating a maze of siloed systems and tribal knowledge, even at companies whose entire business is data.

To address that, we've designed a system for both integrating and serving this data at a single point of contact. At its core, it's a property graph that links organizational structure, technical ownership, sales territories, and product data into a single queryable source of truth. But the interesting part is how we built it and how we serve it.

On the construction side, we use a multi-agent propose-and-critique loop to automatically discover graph structure across heterogeneous data sources. One agent proposes a schema, another critiques it, and they iterate until they converge. Because the schema is agent-derived rather than hand-crafted, the graph can adapt as underlying datasets change or new data sources are added without any manual re-engineering.

On the serving side, we deploy the graph as an MCP server with tools for node search, relationship traversal, and shortest-path queries that both humans and AI agents can call directly in real time. Any agent in our ecosystem can tap into it as a tool with no bespoke integration required.

In this talk, we'll walk through the architecture, what we learned along the way, and make the case for why the combination of knowledge graphs and MCP is an underrated pattern for organizational intelligence in the agentic era.

## About the Speaker

<div class="speaker-profile">
    <div class="speaker-profile-headshot">
    <img src="/assets/images/2026/speakers/MacKenzye_Leroy.jpg" alt="MacKenzye Leroy">
  </div>
  <div class="speaker-profile-info">
    <h3>MacKenzye Leroy</h3>
    <p><em>Lead Data Scientist, S&P Global Market Intelligence</em></p>
    <p>MacKenzye Leroy is a Lead Data Scientist at S&P Global, where he leads the Organizational Intelligence team within MI Enterprise Technology — a shared internal resource focused on developing AI-powered productivity solutions for non-technical stakeholders across Sales, Commercial, Legal, and Marketing.

He combines an M.S. in Data Science from the University of Virginia with a physics background to tackle complex business challenges, with expertise spanning agentic AI, knowledge systems, data pipeline development, and full-stack data science from initial concept through production deployment. He previously spoke at PyData Virginia 2025 on building robust LLM evaluation frameworks for enterprise GenAI tools.

When not working with data, MacKenzye can be found exploring mountain trails by foot, bike, or snowboard, reading, or cheering on his beloved New York Mets.</p>
  </div>
</div>
