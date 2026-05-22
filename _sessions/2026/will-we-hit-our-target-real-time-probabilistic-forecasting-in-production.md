---
layout: session-2026
title: "Will We Hit Our Target? Real-Time Probabilistic Forecasting in Production"
permalink: /2026/sessions/will-we-hit-our-target-real-time-probabilistic-forecasting-in-production/
youtube_id: x5Eluv0qOR8
---

# Will We Hit Our Target? Real-Time Probabilistic Forecasting in Production

**Friday, April 17, 2026 · 3:10 PM – 3:40 PM · Violet Crown Charlottesville**

---

Every month, sales leaders ask: given where we are today, how likely are we to hit our monthly targets? Answering this well turns out to be a surprisingly deep technical problem.

This talk walks through a forecasting system that has run daily for two years at a large consumer goods company, providing probabilistic sales forecasts at dozens of hierarchy levels and giving decision-makers a continuously updated probability of meeting their targets.

I'll cover four technical challenges and the solutions we landed on:

1. Fast, robust daily modeling. The base model operates at daily granularity with day-of-week and day-of-year seasonality. To support the backtesting pipeline downstream, each model must fit quickly. We use Fourier terms for yearly seasonality and weekday indicators, with exponentially decaying weights for trend and seasonal components.

2. Probability distributions over arbitrary horizons. We need the distribution of cumulative rest-of-month sales, a quantity that changes daily. Our approach: conformal backtesting across hundreds of historical windows, collecting forecast errors at every possible number of days remaining to build empirical error distributions with no distributional assumptions.

3. Coherent hierarchical uncertainty. Point forecasts aggregate by summation, but prediction intervals don't. We store signed backtest errors at the most granular level, then re-aggregate and re-estimate error distributions at every hierarchy level, ensuring forecasts add up while preserving valid uncertainty.

4. Living inside Excel. End users work in a shared Excel workbook and are...resistant to change. We pre-compute percentiles into a hidden sheet with interpolation formulas, so users can type any sales target at any hierarchy level and instantly see the probability of exceeding it. I'll share lessons from maintaining this interface over two years, including column name changes breaking the pipeline and other exciting Excel production stories.

I'll close with a reflection on what happened when a separate team built a web app to replace the Excel workflow...and why the executives still prefer the spreadsheet.

## About the Speaker

<div class="speaker-profile">
    <div class="speaker-profile-headshot">
    <img src="/assets/images/2026/speakers/Robert_Robison.jpg" alt="Robert Robison">
  </div>
  <div class="speaker-profile-info">
    <h3>Robert Robison</h3>
    <p><em>Senior Data Scientist, Elder Research</em></p>
    <p>Robert Robison is a Senior Data Scientist at Elder Research, where he builds and deploys forecasting and machine learning systems for clients in consumer goods, financial services, aerospace, and healthcare. His recent work focuses on production time series forecasting, uncertainty quantification, and the practical challenges of delivering statistical models into business workflows. He previously presented the forecasting methodology discussed in this talk at the International Symposium on Forecasting. Robert has published in AIAA and serves as Assistant Editor for Methodology at the American Journal of Emergency Medicine.</p>
  </div>
</div>
