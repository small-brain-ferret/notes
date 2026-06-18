> [!NOTE] Definition
> An [[Open Method(s)]].
>
> Uses a secant between two points to calculate the gradient.
>
> Requires that we have 2 starting points on the function, ($x_{i-1}$, $f(x_{i-1})$)
>
> We can draw a line between these points with a slope, $m_i$, given by:
>
> $$
> m_i=\frac{{f(x_{i})-f(x_{i-1})}}{x_{i}-x_{i-1}}
> $$
>
> Thus:
>
> $$
> x_{i+1}=x_i-\frac{(x_i-x_{i-1})f(x_i)}{f(x_i)-f(x_{i-1})}
> $$

The pseudocode for this method is the pseudocode for [[Open Method(s)]], with a few amendments.

- There is one additional argument, $x_{i-1}$, the previous initial guess
- At step 1, $x_{i+1}$ is calculated using the above equation, which needs both $f(x_{i-1})$ and $f(x_{i})$.
- In step three, $x_i$ is set to $x_{i-1}$.
