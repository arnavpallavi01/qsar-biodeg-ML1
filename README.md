
Dataset & Objective: This project uses the QSAR Biodegradation dataset introduced by Mansouri et al. (2013) containing 1,055 chemicals and 41 molecular descriptors to predict whether a compound is Ready Biodegradable (RB) or Not Ready Biodegradable (NRB).

Connection to the Research Paper: While Mansouri et al. (2013) applied genetic-algorithm feature selection with k-Nearest Neighbors (kNN), PLSDA, and Support Vector Machines (SVM) to achieve 84%–87% accuracy, our workflow tests linear vs. rule-based interpretability using VIF multicollinearity filtering (VIF <= 15), sequential feature selection, Regularized Logistic Regression, and an Entropy-based Decision Tree.

Results & Key Takeaway: Regularized Logistic Regression achieved ~86% test accuracy (F1-score ~0.79), matching the benchmark accuracy of the original study and outperforming the pruned Decision Tree (~81% test accuracy). One key takeaway is that chemical biodegradability is governed by the additive effects of multiple functional groups (such as halogens, nitro groups, and carbonyl oxygens), making regularized linear log-odds modeling more generalizable than rigid single-feature tree splits.

  Citation  - https://doi.org/10.1021/ci4000213 DOI link Mansouri, K., Ringsted, T., Ballabio, D., Todeschini, R., & Consonni, V. (2013). Quantitative Structure–Activity Relationship Models for Ready Biodegradability of Chemicals. Journal of Chemical Information and Modeling, 53(4), 867–878
