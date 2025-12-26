
**Factor Analysis (FA)** explains many observed variables $X_1,\dots,X_p$​ using a small number of **latent factors** $F_1,\dots,F_k$​ (with $k \ll p$):

$$X = \Lambda F + \varepsilon$$

- $\Lambda$ [[factor loadings]] (how strongly each variable relates to each factor)
- $\varepsilon$: **unique/specific** part + noise for each variable

It’s especially useful for surveys/tests where multiple items measure underlying constructs.

Factor analysis isn't the same that [[Principal Component Analysis (PCA)]].

- [[Principal Component Analysis (PCA)]]: finds components that maximize total variance (mainly for compression).
- Factor Analysis: models **shared [[variance]]** (common factors) + **unique [[variance]]** (specific to each variable), closer to “latent constructs.”

If our goal is interpretable latent dimensions, FA is usually the better fit.