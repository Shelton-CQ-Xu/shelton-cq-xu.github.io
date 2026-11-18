---
title: "A Wasserstein Framework for Abnormal Batch Detection in Streaming Data under Distributional Heterogeneity"
collection: publications
category: conferences
permalink: /publication/2026-08-01-wsd-batch-detection
date: 2026-08-01
authors: "<b>Chenqin Xu</b> and Yisha Yao"
venue: "The First Conference on Statistics and Trustworthy AI for Cross-Domain Acceleration (STAI-X 2026)"
paperurl: "https://openreview.net/forum?id=M3O8DiEmqf"
codeurl: "https://github.com/Shelton-CQ-Xu/wsd-batch-detection"
citation: "Xu, C. and Yao, Y. (2026). A Wasserstein framework for abnormal batch detection in streaming data under distributional heterogeneity. <i>The First Conference on Statistics and Trustworthy AI for Cross-Domain Acceleration (STAI-X 2026)</i>."
---

**Abstract.** Data streams are common in online learning and modern AI systems, where the training data arrives in sequential batches. However, abnormal data batches caused by corruption, adversarial manipulation, or annotation errors can degrade model reliability and learning performance. Detecting such abnormal batches is particularly challenging under natural distributional variability, where genuine anomalies are entangled with normal batch-to-batch heterogeneity. Existing methods suffer from major limitations: gradient- and loss-based methods are sensitive to stochastic noise, robust-statistics methods rely on restrictive assumptions, and two-sample testing methods collapse historical batches into a single reference distribution, thereby failing to capture the natural heterogeneity among regular batches. We propose a new framework for abnormal batch detection in streaming data. Unlike existing approaches that operate on Euclidean data points, our method treats data batches as distribution-valued random objects in Wasserstein space. We employ Wasserstein Spatial Depth to quantify batch centrality and further transform the depth values into empirical p-values, yielding a nonparametric and distribution-adaptive measure of abnormality. The resulting procedure offers a statistically interpretable mechanism to detect abnormal batches relative to a population of naturally varying regular batches. Theoretical analysis establishes the p-value interpretation of the proposed measure and its associated two-stream distributional inference framework. Numerical experiments and real-data studies demonstrate that the proposed method consistently outperforms several popular anomaly-detection approaches and can be effectively integrated into online learning procedures such as online stochastic gradient descent.
