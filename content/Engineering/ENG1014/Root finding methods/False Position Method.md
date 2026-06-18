> [!NOTE] Definition
> A [[Numerical method for root finding]], specifically, a [[Bracketing Method]].
>
> The guess of the root is given by:
>
> $$
> x_{r}=\frac{f(x_{u})x_{l}-f(x_{l})x_{u}}{f(x_{u})-f(x_{l})}
> $$

# Derivation

We draw a chord (linear segment) between the points($x_{l}, f(x_{l})$) and ($x_u, f(x_u)$).
The estimate of the root, $x_r$, is where the chord crosses the x-axis.

![[Attachments/Screenshot 2026-05-27 at 16.41.57.png|338]]

Using similar triangles, the value of $x_r$ can be determined.
![[Attachments/Screenshot 2026-05-27 at 16.44.29.png|345]]

Using the argument of similar triangles, we can say that the gradients are equal:

$$
\frac{{f(x_{u})-0}}{x_{u}-x_{r}}=\frac{0-f(x_{l})}{x_{r}-x_{l}}
$$

Multiplying this out, we get:

$$
\begin{align}
f(x_u)(x_r-x_l) & = -f(x_l)(x_u-x_r) \\
f(x_u)x_r-f(x_u)x_l & = f(x_l)x_r-f(x_l)x_u \\
x_r(f(x_u)-f(x_l)) & = f(x_u)x_r-f(x_l)x_u
\end{align}
$$

Therefore:

$$
x_{r}=\frac{f(x_{u})x_{l}-f(x_{l})x_{u}}{f(x_{u})-f(x_{l})}
$$

The pseudocode for the false position method is the pseudocode for [[Bracketing Method]], with one specification:

- At step 1, the above equation is used to calculate the next guess of the root
