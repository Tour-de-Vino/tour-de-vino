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

## Building a Content-Based Wine Recommendation Engine

<div style="text-align: center;">
  <img src="basic-recommend.png" alt="Content-based" />
</div>

### Proven Business Impact of Recommender Systems

<ul style="list-style: none; padding: 0;">
  <li style="display: flex; align-items: center; margin-bottom: 10px;">
    <img src="amazon.png" alt="Amazon" style="margin-right: 10px; width: 50px;  border-radius: 0; object-fit: contain;" />
    <span>Contributed to 35% of the company's total revenue.[1]</span>
  </li>
  <li style="display: flex; align-items: center; margin-bottom: 10px;">
    <img src="netflix.png" alt="Netflix" style="margin-right: 10px; width: 50px;" />
    <span>Netflix’s algorithm drives 75% of the content watched on the platform [2]. This system saves the company approximately $1 billion annually.[3]</span>
  </li>
  <li style="display: flex; align-items: center; margin-bottom: 10px;">
    <img src="spotify.png" alt="Spotify" style="margin-right: 10px; width: 50px;" />
    <span>Spotify’s recommendation algorithm boosted its monthly user base by 33%.[4]</span>
  </li>
</ul>

### Basic Approach

<div style="text-align: center;">
  <img src="pca.png" alt="Principal Component Analysis" />
</div>

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

---

### References

[1] Jones, S.S. and Groom, F.M. eds., 2019. Artificial Intelligence and Machine Learning for Business for Non-Engineers. CRC Press, pp. 86

[2] Alex Castrounis, 2019. AI for People and Business. A Framework for Better Human Experiences and Business Success.

[3] Gomez-Uribe, C.A. and Hunt, N., 2015. The netflix recommender system: Algorithms, business value, and innovation. ACM Transactions on Management Information Systems (TMIS), 6(4), pp.1-19.

[4] Leonard, D, 2016. Spotify Is Perfecting the Art of the Playlist on Bloomberg Businessweek
