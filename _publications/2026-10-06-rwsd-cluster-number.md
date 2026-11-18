---
title: "Relative Wasserstein Spatial Depth for Cluster Number Selection in Distributional Data"
collection: publications
category: preprints
permalink: /publication/2026-10-06-rwsd-cluster-number
date: 2026-10-06
authors: "<b>Chenqin Xu</b> and Yisha Yao"
venue: "arXiv:2610.09153"
note: "Under review."
arxivurl: "https://arxiv.org/abs/2610.09153"
citation: "Xu, C. and Yao, Y. (2026). Relative Wasserstein spatial depth for cluster number selection in distributional data. arXiv:2610.09153."
---

**Abstract.** Contemporary data in many scientific domains, such as images, media streams, biomedical omics, are naturally modeled as probability distributions in Wasserstein space instead of points in Euclidean space. Consequently, clustering methods for distributions are in high demand, as they provide exploratory frameworks to group objects with similarity. Clustering distribution-valued data in Wasserstein space often requires choosing the number of clusters in advance. We propose Relative Wasserstein Spatial Depth (RWSD) as a selection criterion for optimal number of clusters. It compares the depth of each distribution in its assigned cluster with its depth in competing clusters. We pair this criterion with Wasserstein K-means or a proposed K-medians algorithm. Under suitable assumptions, we establish consistency of the cluster centers and of the selected optimal number of clusters. We also give an error rate under two-stage sampling and characterize the robustness of RWSD under any fixed partition. In extensive simulations, RWSD selects the intended number of clusters under unequal separations, heterogeneous dispersion, heavy tails, and outliers, where silhouette score or the Davies-Bouldin Index often fails. Applications to MNIST images and flow cytometry data illustrate the practical value of RWSD. In some cases where a cluster is not geodesically convex and lacks a meaningful depth center, the RWSD can fail.
