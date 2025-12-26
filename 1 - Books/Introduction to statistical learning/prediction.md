
In many situations, a set of inputs $X$ are readily available, but the output $Y$ cannot be easily obtained. In this setting, since the error term averages to zero, we can predict $Y$ using:
$$\hat{Y}=\hat{f}(X)$$
Where $\hat{f}$ represents our [[estimate]] for $f$, and $\hat{Y}$ represent the resultant **prediction** for $Y$, when we have the **prediction** objective we don't care about the form of $\hat{f}$, just matter that the prediction is accurate. A visual example of this setup are the following figure:

![[Pasted image 20251223101507.png]]

The Accuracy of $\hat{Y}$ as a prediction of $Y$ depends on two quantities which will call the **reducible error** and the **irreducible error**.

The reducible error is the difference between $\hat{f}$ and $f$, this error can be minimized using a potential better [[statistical learning]] technique to [[estimate]] $f$. Now, even if $f = \hat{f}$, by definition $f$ also do not have a perfect fit between $Y$ and $X$, this error ($\epsilon$) is the irreducible error.
