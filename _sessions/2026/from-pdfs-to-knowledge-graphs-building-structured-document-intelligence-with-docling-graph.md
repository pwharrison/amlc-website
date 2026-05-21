---
layout: session-2026
title: "From PDFs to Knowledge Graphs: Building Structured Document Intelligence with Docling-Graph"
permalink: /2026/sessions/from-pdfs-to-knowledge-graphs-building-structured-document-intelligence-with-docling-graph/
youtube_id:
---

# From PDFs to Knowledge Graphs: Building Structured Document Intelligence with Docling-Graph

**Saturday, April 18, 2026 · 3:30 PM – 5:00 PM · Classroom 305**

---

Tutorial resources: https://github.com/KrishnaRekapalli/docling-graph-tutorial

Setup instructions, example files and notebooks are in the repo above. Please clone it and make sure to follow the SETUP.md for a smooth tutorial experience. 

Most of us have hit the same wall. RAG works fine until the question requires understanding relationships, not just finding relevant text. A financial analyst querying a 200-page prospectus needs to know which risk factor links to which instrument, not the three paragraphs that mention "risk." A compliance team reviewing contracts needs to know which clause overrides which other clause, cross-referenced across annexes. A researcher parsing clinical trial reports needs compound-to-outcome chains, not keyword matches. Embeddings get you in the right neighborhood. They don't get you the answer.
This tutorial is about building the layer that does. Docling-Graph is an open-source Python library (MIT licensed, IBM Research) that turns documents into validated, queryable knowledge graphs. Feed it a PDF, Word doc, HTML, or scanned image. It parses the document with Docling, extracts entities and relationships, validates output against a Pydantic schema you define, and returns a directed NetworkX graph ready to visualize, query, or push to Neo4j.

One Pydantic model defines both the extraction logic and the graph structure. No separate ontology to maintain.
Two extraction paths are available. If you have access to an LLM API (Mistral, OpenAI, Watsonx) or run local inference with Ollama or vLLM, the LLM path handles complex schemas well. If you'd rather not touch an API key at all, the VLM path runs entirely through Docling's built-in vision model on your machine. No external calls, no data leaving your environment.

We'll spend 90 minutes building something real: a template for a financial document, running it on an actual annual report, walking through the graph, and tackling the things that make production use hard: long documents, nested schemas, cross-section references, and debugging extractions that don't look right.
You'll leave with a working setup, a notebook with everything we built, and an honest sense of where this beats vector search and where it doesn't.

Good fit if you work with document-heavy pipelines in finance, legal, or research; have used LLMs or RAG before; and know Python. No graph database experience needed. We'll cover the Pydantic basics as we go.

## About the Speaker

<div class="speaker-profile">
    <div class="speaker-profile-headshot">
    <img src="/assets/images/2026/speakers/Krishna_Rekapalli.jpg" alt="Krishna Rekapalli">
  </div>
  <div class="speaker-profile-info">
    <h3>Krishna Rekapalli</h3>
    <p><em>Sr AI Engineer, IBM watsonx DataLabs</em></p>
    <p>Krishna Teja Rekapalli is a Senior Data Scientist at IBM's Watsonx.ai Solution Architecture Center of Excellence, where he specializes in designing and implementing enterprise-scale LLM-powered AI solutions and agentic workflows. With over 7 years of experience building production ML applications, he has architected RAG systems for clients across financial services, healthcare, and manufacturing sectors.
Krishna works at the intersection of research and practice, translating cutting-edge AI capabilities into production-ready architectures that handle real-world constraints: data quality issues, latency requirements, compliance frameworks. His expertise spans the full RAG stack i.e from document ingestion pipelines to vector search optimization to agentic workflow orchestration with deep experience in the open-source AI ecosystem including Langflow, OpenSearch, and modern LLM frameworks.</p>
  </div>
</div>
