---
layout: session-2026
title: "Lightweight Breast Cancer Detection Model: Parameter-Efficient Fine-Tuning & Knowledge Distillation"
permalink: /2026/sessions/lightweight-breast-cancer-detection-model-parameter-efficient-fine-tuning-knowledge-distillation/
youtube_id:
---

# Lightweight Breast Cancer Detection Model: Parameter-Efficient Fine-Tuning & Knowledge Distillation

**Friday, April 17, 2026 · 10:55 AM – 11:25 AM · Auditorium 4**

---

Breast cancer remains one of the leading causes of cancer-related death worldwide, with the burden rising fastest in regions that lack access to advanced diagnostic technology. Breast cancer detection through medical imaging has the potential to save lives, however, many of today’s most powerful AI models are simply too large and resource-intensive to be deployed where they are needed most. This session explores how we can make state-of-the-art segmentation models both efficient and practical, without compromising performance.

We’ll walk through a hands-on investigation of modern vision foundation models, including SAM2 and MedSAM, and examine how architectural design, data augmentation, and training strategy impact real-world usability. Surprisingly, we find that SAM2 consistently outperforms MedSAM, even without medical-specific pretraining, which highlights how newer model architectures can outweigh domain specialization.

The core of the session focuses on knowledge distillation as a powerful tool for accessibility. By distilling large foundation models into much smaller student networks (both CNN-based and transformer-based) we demonstrate that lightweight models (as small as 4% of the original size) can match or even exceed their teachers’ segmentation performance. Even more striking, this is achieved without using prompts, challenging common assumptions about SAM-style models.

Attendees will leave with practical insights into:

- When large foundation models are worth deploying, as well as when they aren’t.
- How to design efficient segmentation pipelines for resource-constrained environments.
- Why knowledge distillation may be a better path forward than fine-tuning alone.

This session is ideal for researchers, practitioners, and healthcare technologists interested in deployable medical AI, efficient model design, and bridging the gap between cutting-edge research and real clinical impact.

## About the Speaker

<div class="speaker-profile">
    <div class="speaker-profile-headshot">
    <img src="/assets/images/2026/speakers/Steven_Cocke.jpg" alt="Steven Cocke">
  </div>
  <div class="speaker-profile-info">
    <h3>Steven Cocke</h3>
    <p><em>Chief Technology Officer & Lead Data Scientist - Doctorate in AI/ML</em></p>
    <p>Steven Cocke is the Chief Technology Officer and Lead Data Scientist at Walker Engineering Solutions, where he leads applied AI/ML, computer vision, modeling & simulation, and data science efforts in support of U.S. government and defense missions. He holds a doctoral degree in Artificial Intelligence and Machine Learning from George Washington University, where his research focused on developing lightweight, deployable breast cancer segmentation models using vision foundation models and knowledge distillation.

Steven has over a decade of experience building and deploying machine learning systems across healthcare, geospatial analysis, modeling and simulation, and large-scale data platforms. His work spans convolutional and transformer-based architectures, vision foundation models, parameter-efficient training methods, and resource-constrained deployment. In addition to his industry work, he serves as a lecturer at the George Washington University, teaching graduate and doctoral-level courses in applied machine learning and data engineering.</p>
  </div>
</div>
