#statistical_learning

**Unsupervised learning** is the set of methods that discover **structure** in data using only inputs $X$ but there is no labeled outcome $Y$, aiming to reveal patterns such as groups, low-dimensional representations, or latent factors.

$$\{x_i\}_{i=1}^n,\quad x_i\in\mathbb{R}^p$$

The objective of unsupervised learning is to learn a representation, partition, or distributional description of $X$:

- [[clusters]] / communities
- [[principal components]]
- density / anomalies
- [[latent variables]]

We use usually use unsupervised learning to **find patterns** we didn’t predefine, **represent data** with fewer dimensions, **create features** for [[Supervised statistical learning]], **group entities** into meaningful [[clusters]], **identify outliers** relative to a learned structure or make [[Exploratory Data Analysis (EDA)]].

In [[Supervised statistical learning]] we have a [[ground truth]], a true valor with which we can fit our models and measure how close are we from this values, we don't have this in unsupervised statistical learning because we don't know the true anwser.

## Main problem families

when we want to assign points to groups with high within-group similarity ([[clustering problem]]) the following models could be useful:

- [[k-means]] (centroid-based; spherical [[clusters]])
- [[Gaussian Mixture Model (GMM)]] (probabilistic; soft clustering)
- [[Hierarchical clustering]] (tree/dendrogram)
- [[DBSCAN]] / [[HDBSCAN]] (density-based; finds arbitrary shapes, handles noise)

Outputs of the models often include:
- cluster labels $c_i$
- cluster probabilities (for [[Gaussian Mixture Model (GMM)]])
- “noise/outlier” labels (for density-based clustering)

For another way, if we want to find low-dimensional [[embeddings]], we should be familiar to:

- [[Principal Component Analysis (PCA)]] (linear variance-maximizing components)
- [[Factor analysis]] (latent factor model)
- [[t-SNE]] / [[UMAP]] (nonlinear embeddings for visualization)
- [[Autoencoders]] (neural representation learning)

If we want to estimate the distribution $p(x)$ that is useful for anomaly detection, simulation, and probabilistic reasoning.

- [[Kernel Density Estimation (KDE)]]
- [[Mixture model]]

Because there’s no ground-truth $Y$, evaluation depends on the objective and the model used.

## Connections
- [[Supervised statistical learning]]
- [[Statistical Learning]]
- [[Dimensionality Reduction]]
- [[Density Estimation]]
- [[Anomaly Detection]]
- [[Curse of Dimensionality]]

## Minimal references
- Hastie, Tibshirani, Friedman — *The Elements of Statistical Learning*
- Murphy — *Machine Learning: A Probabilistic Perspective*
- Bishop — *Pattern Recognition and Machine Learning*
