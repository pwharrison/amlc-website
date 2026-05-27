---
layout: session-2026
title: "Best of Both Worlds: Combining Domain Knowledge with Deep Learning"
permalink: /2026/sessions/best-of-both-worlds-combining-domain-knowledge-with-deep-learning/
youtube_id:
session_photo: https://amlc-images.appliedml.us/2026/041826_MMP_Multi332.jpg
---

# Best of Both Worlds: Combining Domain Knowledge with Deep Learning

**Saturday, April 18, 2026 · 1:30 PM – 3:00 PM · UVA School of Data Science**

---

Most ML models treat domain knowledge as optional. You hand your data to a neural network and it ignores every constraint humans have spent millennia building intuition about. Physics, regulatory limits, accounting rules, etc., that background knowledge doesn't carry over. The predictions look great on your test set. Then they fail in production because the model never learned that inventory can't go negative or that debits have to equal credits.

Pure rule-based systems have the opposite problem. They enforce everything you know perfectly. They also miss every pattern you haven't manually encoded. And the world is full of complex, nonlinear relationships.

Hybrid systems let you keep both. You separate what you know from what you don't know yet. The rules handle the first part. ML learns the rest (the complex patterns hiding in data that your rules can't capture).

This is the architecture behind some of the most reliable production ML systems in fraud detection, compliance risk, forecasting, and simulation. Where you've got known structure plus unknown factors, this pattern can apply.

In this workshop you'll build a hybrid model using JAX from scratch. This hybrid model is inspired by the architecture used in NeuralGCM (the world's first fully-differentiable hybrid general circulation model). You'll train it two ways, offline and online, and see firsthand why learning in context versus learning in isolation produces different results.

By the end you'll have a better understanding of JAX and a new way to implement a fully differentiable hybrid model that combines mathematical modeling/scientific computing with deep learning. We'll also discuss how this architecture can be applied to your domain.

Who this is for: ML practitioners, data scientists, and research engineers.

What you need coming in: Python, NumPy, and basic ML training concepts (losses, gradients, optimizers). A conceptual understanding of derivatives helps. No differential equations or climate science background required. A JAX primer is included for anyone new to it.

Main notebook: https://colab.research.google.com/drive/1K7pmkkzSnxwwDhN_M6CPj2f3SqDgGeuc?usp=sharing

JAX primer: https://colab.research.google.com/drive/1Wr3lZrihbWyYbYdY2kn2ucQxmAvsCaJf?usp=sharing

## About the Speaker

<div class="speaker-profile">
    <div class="speaker-profile-headshot">
    <img src="/assets/images/2026/speakers/Cynthia_Ukawu.jpg" alt="Cynthia Ukawu">
  </div>
  <div class="speaker-profile-info">
    <h3>Cynthia Ukawu</h3>
    <p><em>Machine Learning Engineer @ DARPA</em></p>
    <p>Cynthia is a Machine Learning Engineer, where she serves as head architect and developer for a DARPA-funded ML analysis platform. The platform analyzes LLM embeddings using topology as the underlying mathematical framework, enabling researchers to study language model behavior at scale.

Beyond the core platform, she builds production APIs for vision-language models and text-to-speech systems, bringing cutting-edge AI research into operational deployment.

With an MS in Applied & Computational Mathematics from Johns Hopkins and prior experience at General Atomics-CCRi and Arity (geospatial ML at scale), she combines deep mathematical foundations with practical engineering expertise in PyTorch, AWS, and distributed systems.

She has mentored over 30 students through programs at The Coding School, Masterschool, and Springboard, helping them transition into data and ML roles. She also writes about ML systems on her blog: cynscode.com</p>
  </div>
</div>
