---
title: KPI's
description: ....
date: "2024-9-18"
categories:
  - sveltekit
  - svelte
published: true
author: Tour de Vino Team
author_image: logo.png
image: kpis.webp
---

# Simulating User Interaction & Recommender KPIs

-----
Breakdown of the Process:
Recommendation Flow:

1. Recommendation Flow:
Click-Through Rate (CTR):
Returning users have a 50% chance of clicking on a recommended wine.
Once clicked, they have a 70% chance of viewing details and a 30% chance of adding to cart.
These probabilities are higher because the system shows wines aligned with the user’s preference, making it more likely that they will engage with the wine.

2. Random Flow:
Click-Through Rate (CTR):
Returning users have only a 5% chance of clicking on a randomly presented wine.
If they do click, they have a 40% chance of viewing details and only a 10% chance of adding to cart.
These lower probabilities reflect that random wines are less likely to match the user's tastes, reducing the chance of engagement.


### Business Impact
- recommended system yields significantly better metrics than showing random wines

By simulating both recommended and random interactions with these probabilities, recommended system yields significantly better metrics than showing random wines, such as:

- Higher CTR: More users click on wines that are recommended (50% vs. 5%).
- Higher Conversion Rate: More users ultimately add to cart and purchase recommended wines (30% after viewing details vs. 10% for random).
- Higher Average Order Value (AOV): Because the recommendation system suggests relevant wines (often in higher price ranges for premium buyers), users are more likely to buy higher-value wines.
- Repeat Purchase Rate: Users who find wines they like via recommendations are more likely to return and buy again.


![](chart.png)