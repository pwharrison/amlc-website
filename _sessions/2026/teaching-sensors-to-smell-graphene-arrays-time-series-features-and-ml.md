---
layout: session-2026
title: "Teaching Sensors to Smell: Graphene Arrays, Time-Series Features, and ML"
permalink: /2026/sessions/teaching-sensors-to-smell-graphene-arrays-time-series-features-and-ml/
youtube_id:
---

# Teaching Sensors to Smell: Graphene Arrays, Time-Series Features, and ML

**Friday, April 17, 2026 · 10:55 AM – 11:25 AM · Auditorium 2**

---

Machine olfaction (artificial olfaction / electronic noses) aims to mimic aspects of human smell by combining material science, sensor engineering, and machine learning. The promise is compelling—but the bottleneck isn’t the classifier. It’s the data.

Graphene-based sensor arrays produce multichannel resistance time-series whose response and recovery dynamics encode chemo-physical interactions between vapors/odors/compounds and engineered sensing materials. Graphene is especially well-suited here: its 2D carbon surface is fully exposed to the environment, it’s compatible with semiconductor processing, and its surface chemistry can be modified to create cross-reactive arrays with tunable selectivity. The result is a sensing platform that can span the serious (chemical warfare agents, toxic industrial chemicals, VOCs) and the delightfully human (scotch whiskies and essential oils)—all by “reading” how complex mixtures perturb an array over time.

In this talk, I’ll walk through the practical end-to-end workflow for turning these signals into reliable ML systems:

1. The sensor-array concept and why “cross-sensitivity” is a feature, not a bug;
2. Preprocessing and signal features that capture both traditional response metrics (ΔR, sampling/recovery area) and interaction-driven structure (response/recovery fitting coefficients); and
3. Model training and evaluation patterns for compound classification and anomaly detection.

A central theme is the “ImageNet gap” in olfaction: unlike computer vision, there’s no off-the-shelf way to expose sensors to many chemicals/odors in a precise, automated, and reproducible manner while collecting labeled training data at scale. I’ll describe an approach built around automated vapor delivery, synchronized measurement, and web-based collection/model dashboards—enabling hundreds of labeled runs, retraining for new targets, and versioned deployment without changing sensor hardware.

## About the Speaker

<div class="speaker-profile">
    <div class="speaker-profile-headshot">
    <img src="/assets/images/2026/speakers/Eric_Nallon.jpg" alt="Eric Nallon">
  </div>
  <div class="speaker-profile-info">
    <h3>Eric Nallon</h3>
    <p><em>Black Cow Labs</em></p>
    <p>Eric Nallon is an electrical engineer and applied ML practitioner focused on sensors, semiconductors, and data-driven detection systems. He earned a B.S. in Electrical Engineering from Penn State and a Ph.D. from George Mason University, with research centered on graphene-based chemical vapor sensors for electronic-nose applications. He has worked as an engineer and researcher at the U.S. Army Research and Technology Integration organization (formerly NVESD, Fort Belvoir), spanning III–V compound-semiconductor IR detector fabrication and test, and material-based chemical sensing using organic semiconductors, quantum dots, and graphene in both electrical and photoluminescent designs. His work emphasizes sensor characterization, semiconductor processing, automation, and ML-enabled analysis, and he has published in multiple peer-reviewed venues.</p>
  </div>
</div>
