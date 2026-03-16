---
layout: distill
title: AEGIS - Authentic Edge Growth In Sparsity for Link Prediction in Edge-Sparse Bipartite Knowledge Graphs
description:
img: 
category:  Games
related_publications: true
featured: true

authors:
  - name: Hugh Xuechen Liu
    url: 
    affiliations:
      name: Chalmers University of Technology
  - name: Kıvanç Tatar
    url: "https://www.kivanctatar.com"
    affiliations:
      name: Chalmers University of Technology

---
## Abstract

Bipartite knowledge graphs in niche domains are typically data-poor and edge-sparse, which hinders link prediction. We introduce AEGIS (Authentic Edge Growth In Sparsity), an edge-only augmentation framework that resamples existing training edges -either uniformly simple or with inverse-degree bias degree-aware -thereby preserving the original node set and sidestepping fabricated endpoints. To probe authenticity across regimes, we consider naturally sparse graphs (game design pattern's game-pattern network) and induce sparsity in denser benchmarks (Amazon, MovieLens) via high-rate bond percolation. We evaluate augmentations on two complementary metrics: AUC-ROC (higher is better) and the Brier score (lower is better), using two-tailed paired t-tests against sparse baselines. On Amazon and MovieLens, copy-based AEGIS variants match the baseline while the semantic KNN augmentation is the only method that restores AUC and calibration; random and synthetic edges remain detrimental. On the text-rich GDP graph, semantic KNN achieves the largest AUC improvement and Brier score reduction, and simple also lowers the Brier score relative to the sparse control. These findings position authenticity-constrained resampling as a data-efficient strategy for sparse bipartite link prediction, with semantic augmentation providing an additional boost when informative node descriptions are available.

<https://arxiv.org/abs/2509.22017>
