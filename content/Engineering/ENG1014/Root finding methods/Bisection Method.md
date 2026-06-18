> [!NOTE] Definition
> A [[Numerical method for root finding]], specifically, a [[Bracketing Method]].
>
> The guess of the root is the midpoint of the interval, that is:
>
> $$
> x_{r}=\frac{x_{l}+x_{u}}{2}
> $$

The pseudocode for this method is the same as for [[Bracketing Method]], with one specification:

- at step 1, the above equation is used to estimate the next guess of the root.
