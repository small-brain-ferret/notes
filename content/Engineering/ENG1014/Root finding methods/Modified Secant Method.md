> [!NOTE] Definition
> An [[Open Method(s)]]. Similar to the [[Secant Method]].
>
> Only needs one point, ($x_i,$ $f(x_i$)), and a small increment to $x_i$ we call the perturbation, $\delta$.
>
> We can then approximate the derivative as the slope of the line passing through these points:
>
> $$
> m_i=\frac{f(x_i+\delta)-f(x_i)}{\delta}
> $$
>
> Thus:
>
> $$
> x_{i+1}=x_i-\frac{\delta f(x_{i})}{f(x_i+\delta)-f(x_i)}
> $$

The pseudocode for this method is the same for open methods, with a few amendmments:

- one additional argument, $\delta$, which is the perturbation
- At step one, $x_{i+1}$ is calculated using the equatoin above.
