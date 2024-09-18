---
title: AI Recommendations
description: Leveraging data for personalized wine experiences
date: "2024-9-17"
categories:
  - sveltekit
published: true
author: Tour de Vino Team
author_image: logo.png
image: carrousel-images/boat.jpeg
---

### Proven Business Impact of Recommender Systems

1. **Amazon** is one of the most prominent users and pioneers of recommendation systems. By personalizing the online shopping experience for each customer, these recommendations contribute to **35%** of the company's total revenue.[1].

2. Another well-known example of a recommendation system is **Netflix**’s algorithm. According to **McKinsey**, 75% of the content watched on **Netflix** is driven by its movie recommendations[2]. In the paper “The Netflix Recommender System: Algorithms, Business Value, and Innovation” [3], Netflix executives Carlos A. Gomez-Uribe and Neil Hunt highlight that this system saves the company approximately $1 billion annually.

3. **Spotify** reports that the introduction of its new recommendation algorithm has played a key role in boosting its monthly user base from **75 million to 100 million**. [4].

<div style="display: flex; justify-content: center; align-items: center;">
  <img src="amazon.png" alt="Amazon" style="margin: 0 10px; width: 100px; border-radius: 0; object-fit: contain;" />
  <img src="netflix.png" alt="Netflix" style="margin: 0 10px; width: 100px;" />
  <img src="spotify.png" alt="Spotify" style="margin: 0 10px; width: 100px;" />
</div>

Based on the "Shreya Basu, Personalized product recommendations and firm performance, Electronic Commerce Research and Applications, Volume 48, 2021, 101074", we can see that personalized recommendations can increase sales by 30%.

![30 Percent](30percent.svg)

## Build a content-based recommendation engine using existing wine data

1. Recommedation of **similar wines based on similar features** (i.e. grape variety, producer, etc.)
2. Suggest wines based on their previous preferences and interactions or ratings.

<div style="text-align: center;">
  <img src="basic-recommend.png" alt="Content-based" />
</div>

### Basic Approach

<div style="text-align: center;">
  <img src="PCA.png" alt="Principal Component Analysis" />
  <img src="pca_zoom.png" alt="Principal Component Analysis Zoomed In" width="300"/>
</div>

> We can analyse the _intrinsic characteristics_ of the wines and cluster them into groups based on their similarities. This will allow us to recommend wines that are similar to the ones the user has liked in the past. This following plot healights the first three principal components of the wines, which can be used to cluster them into groups.
> Each component is a linear combination of multiple chacharecteristics of the wines, such as _acidity_, _sweetness_, etc.

### Upgrade Path

![](upgrade-path-v2.png)

<!-- Transitioning to **collaborative filtering** as the data grows and matures will enable more personalized and accurate recomendations.

- Customer Feedback Data Collection Pipelines:
1. **Explicit Feedback**: Gather direct customer inputs through ratings, reviews, and comments. Implement post-purchase surveys or incentivized feedback systems that encourage user participation without being overly intrusive.
2. **Implicit Feedback**: Implement passive data collection through non-intrusive methods such as tracking user interactions with product pages, time spent per page, browsing behavior, cart additions, and purchase frequency.-->

### Key Advantages

- Scalable solution.
- Real time suggestions
- Fully automated
- AI-driven and human expertise independent.

Information about user preferences can be used to recommend wines that similar users have liked in the past.

Interested for more? Check out our dashboard for a live demo of the recommendation engine!
[Dashboard](https://huggingface.co/spaces/TourdeVino/showcase)

![Dashboard Example](dashboard_example.png)

Let's take a look into how to improve wine tourism [Passaport](/passaport-post)

<!--
This leads to:

# Immediate Engagement & Personalization

- Personalized Experience: Even without user data, the content-based recommendation engine provides relevant, personalized suggestions based on wine characteristics. This enhances customer experience immediately.

  - Metric: CTR for recommended wines, engagement on the platform.

# Revenue Growth Potential

# Increasing Conversion Rates

- Increased Sales: With more personalized suggestions, the system improves conversion rates and average order value as users are more likely to discover wines they love or add more bottles to their cart.

  - Metric: Purchase conversion rate, AOV.

# Scalability

# Customer Retention

Long-Term Value:

- Customer Retention and Loyalty: Over time, as more user data is collected, the system will drive repeat purchases by providing even more personalized suggestions. This fosters customer loyalty and increases the lifetime value of each customer.

  - Metric: Repeat purchase rate, user lifetime value (LTV).
-->

---

### References

[1] Jones, S.S. and Groom, F.M. eds., 2019. Artificial Intelligence and Machine Learning for Business for Non-Engineers. CRC Press, pp. 86

[2] Alex Castrounis, 2019. AI for People and Business. A Framework for Better Human Experiences and Business Success.

[3] Gomez-Uribe, C.A. and Hunt, N., 2015. The netflix recommender system: Algorithms, business value, and innovation. ACM Transactions on Management Information Systems (TMIS), 6(4), pp.1-19.

[4] Leonard, D, 2016. Spotify Is Perfecting the Art of the Playlist on Bloomberg Businessweek
