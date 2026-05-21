---
layout: session-2026
title: "Beyond A/B Testing: Practical Contextual Bandits for Dynamic Pricing in Production"
permalink: /2026/sessions/beyond-ab-testing-practical-contextual-bandits-for-dynamic-pricing-in-production/
youtube_id:
---

# Beyond A/B Testing: Practical Contextual Bandits for Dynamic Pricing in Production

**Friday, April 17, 2026 · 10:20 AM – 10:50 AM · Auditorium 2**

---

Every time you run an A/B test, you're making a quiet bet: that the cost of being wrong for half your users is worth the certainty you'll gain. For low-stakes decisions, that's fine. For pricing millions of consumer subscriptions — where the right price depends on who the customer is, where they came from, and what they're likely to do next — that bet gets expensive fast.

This is the story of how my team at McAfee moved beyond A/B testing and built a contextual bandit system that prices dynamically, learns continuously, and doesn't require you to consciously hurt half your users to figure out what works.
But this isn't a theory talk. I'll spend most of our 30 minutes on the parts that don't make it into research papers: the reward signals that lied to us, the feature pipelines that became bottlenecks, the stakeholders who wanted a control group and wouldn't accept "trust the algorithm," and the offline evaluation tricks that kept us honest before we dared push anything to production. 

Along the way, we'll cover enough of the core concepts — exploration vs. exploitation, Thompson Sampling vs. LinUCB, off-policy evaluation — that you'll leave with a working mental model, not just a reading list. If you've ever suspected that A/B testing is leaving value on the table but weren't sure where to start, this talk is for you. And if you've already started down the bandit path and hit a wall, there's a good chance we hit the same one.

Who this is for: Data scientists and ML engineers comfortable with experimentation and basic modeling concepts. No prior reinforcement learning background needed — but you'll leave wanting to dig deeper.

## About the Speaker

<div class="speaker-profile">
    <div class="speaker-profile-headshot">
    <img src="/assets/images/2026/speakers/Arul_Bharathi.jpg" alt="Arul Bharathi">
  </div>
  <div class="speaker-profile-info">
    <h3>Arul Bharathi</h3>
    <p><em>Senior Manager, Applied AI & ML, McAfee · Fraud, Churn, Pricing, and Personalization</em></p>
    <p>Arul Bharathi is a Senior Manager of AI & Machine Learning at McAfee, where he leads a distributed team of Applied Scientists, and ML engineers across Canada, the United States, and India. With over 12 years of experience building production machine learning systems, he has designed and shipped models across some of the most consequential problems in consumer technology — from fraud detection systems that protect millions of users in real time, to churn prediction models that improved subscriber retention, to personalization engines and contextual bandit-driven dynamic pricing systems that have collectively driven over $100M+ in incremental revenue.
Arul's work sits at the intersection of rigorous ML and real business outcomes. He is particularly interested in the gap between what works in notebooks and what survives contact with production — and in building teams that can close that gap reliably.</p>
  </div>
</div>
