---
layout: session-2026
title: "The Future of OCR? Structured Text Extraction with LLMs"
permalink: /2026/sessions/the-future-of-ocr-structured-text-extraction-with-llms/
youtube_id: 5ahp4fWLOUQ
---

# The Future of OCR? Structured Text Extraction with LLMs

**Friday, April 17, 2026 · 3:10 PM – 3:40 PM · Violet Crown Charlottesville**

---

Optical character recognition (OCR) has been a long standing method of extracting text data from images. Traditional OCR models relied on pattern recognition and feature extraction using computer vision techniques. Recently, large language models (LLMs) and multimodal AI assistants have provided an alternative method of text extraction that seeks to outperform older models in terms of accuracy and flexibility.

Structured data extraction is a classic problem that has applications to many domains, such as document digitization, information extraction, and accessibility. There is great potential for LLMs to enhance automation for routine document processing tasks, but there are also genuine concerns for deploying these models to production. LLMs can produce inconsistent outputs, produce hallucinations and confabulations, and are vulnerable to prompt injection. When evaluating the efficacy of OCR solutions, it's important to define metrics that capture not only accuracy but also latency, cost, and energy expenses.

This talk explores the benefits and challenges of applying LLMs to extracting text from scanned images. Three OCR methods are contrasted: small scale transformer-based OCR models, modern SOTA assistants such as Gemini, Claude, and Qwen, and a hybrid approach that combines both methods. I will present an evaluation strategy that utilizes both automated and human feedback to compare LLM-based approaches to traditional OCR.

This talk is for data scientists and machine learning engineers who are interested in prototyping and evaluating text extraction solutions. I will walk through several Python code examples for structured extraction using open source libraries such as docling and docTR, and demonstrate how to evaluate these libraries against LLM-based solutions.

Provisional Outline

1. Traditional OCR techniques (5 minutes)
    a. Object detection approaches
        i. docling
        ii. RF-DETR
    b. Deep learning with open source models and the docTR library
2. Text extraction with LLMs (10 minutes)
    a. Extracting structured outputs with pydantic
    b. Prompt engineering
    c. Combining traditional OCR with LLMs
3. Evaluating text extraction approaches (5 minutes)
    a. Automated vs. human evaluation
    b. Cost metrics (latency, compute and API expenses, energy)
4. Production scaling for OCR (5 minutes)
    a. Separation of concerns
    b. Provisioning GPUs vs API calls

## About the Speaker

<div class="speaker-profile">
    <div class="speaker-profile-headshot">
    <img src="/assets/images/2026/speakers/Patrick_Deziel.jpg" alt="Patrick Deziel">
  </div>
  <div class="speaker-profile-info">
    <h3>Patrick Deziel</h3>
    <p><em>Distributed Systems Engineer - Machine Learning Specialist</em></p>
    <p>Patrick Deziel is a distributed systems engineer and Go and Python programmer. He has extensive experience building end-to-end machine learning applications in the private sector and has contributed to various open source projects such as Yellowbrick. He currently works at Rotational Labs where he builds backend services, client SDKs, and AI-powered applications. In his free time, Patrick enjoys rock climbing and dance dance revolution.</p>
  </div>
</div>
