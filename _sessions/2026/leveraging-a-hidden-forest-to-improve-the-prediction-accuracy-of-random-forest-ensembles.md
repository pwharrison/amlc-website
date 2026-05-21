---
layout: session-2026
title: "Leveraging a Hidden Forest to Improve the Prediction Accuracy of Random Forest Ensembles"
permalink: /2026/sessions/leveraging-a-hidden-forest-to-improve-the-prediction-accuracy-of-random-forest-ensembles/
youtube_id:
---

# Leveraging a Hidden Forest to Improve the Prediction Accuracy of Random Forest Ensembles

**Friday, April 17, 2026 · 1:45 PM – 2:15 PM · Auditorium 4**

---

Random forests are a widely used workhorse for predictive tasks, yet they typically aggregate trees by simple averaging, implicitly treating trees as interchangeable and ignoring how their prediction errors co-move. We introduce peer adjustment, a post-processing methodology that improves random forest predictions by exploiting the correlation structure between the forest average and an internal peer prediction signal derived from the trees’ leaf structure. The method treats each tree as an information source: for a query point, a tree’s terminal leaf defines a neighborhood of training observations it deems similar, and the rest of the forest’s predictions on that neighborhood provide a peer forecast. Peer adjustment then combines the standard forest prediction and this peer signal through a single adjustment parameter selected to minimize out-of-sample error (via cross-validation).

The approach is theoretically grounded in the relevant error-covariance terms that govern optimal combination of dependent forecasts. Exploiting symmetry within random forests, we show that the optimal dependence-aware linear correction collapses to a one-dimensional adjustment, yielding an interpretable "pivoting" mechanism that can either move away from the peer consensus or shrink toward it, depending on whether the discrepancy captures systematic residual structure left by averaging. Because the peer signal is computed from quantities already generated during standard training, peer adjustment is low-cost and immediately deployable, requiring no new data and no changes to the underlying forest training procedure.

Across 11 diverse real-world datasets spanning housing markets, transportation, environmental monitoring, materials science, and consumer products, and 550 experimental configurations, we find consistent improvements: a mean test-set MSE reduction of 6.04%, with 81.6% of settings showing positive gains. Peer adjustment provides a simple, interpretable enhancement to random forests and captures structure not recovered by standard post-hoc fixes such as linear calibration or shrinkage-based regularization.

## About the Speaker

<div class="speaker-profile">
  <div class="speaker-profile-info">
    <h3>Junnan Wang</h3>
    <p><em>Darden Postdoc</em></p>
    <p>Junnan Wang is a postdoctoral researcher in Data Analytics & Decision Sciences at the University of Virginia Darden School of Business. Wang develops methods to improve predictive performance, combining optimization, machine learning, and Bayesian statistics, with a focus on evaluating and aggregating forecasts either from human forecasters or from algorithmic models. In this talk, Wang will introduce a practical “peer adjustment” approach for random forests that leverages information in the forest’s internal structure to refine predictions as a post‑hoc adjustment.</p>
  </div>
</div>
