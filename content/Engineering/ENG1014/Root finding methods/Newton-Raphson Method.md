> [!NOTE] Definition
> An [[Open Method(s)]].
> It uses the exact expression for the derivative, $f'(x_i)$, to determine the estimated slope of the function, $m_i$.
>
> The next guess would be:
>
> $$
> x_{i+1}=x_i-\frac{f(x_{i})}{f'(x_{i})}
> $$

The pseudocode for this method is the same for open methods, with a few amendmments.

At step 1, $x_{i+1}$ is calculated using the above equation.

Thus, $f'(x)$ needs to be specified. It is typically defined as a lambda function before the iterative process starts.
