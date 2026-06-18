A [[Numerical method for root finding]].

> [!NOTE] Definition
> Where the search for a particular root is conducted using either one or two starting points that do not need to surround the root.
>
> These methods make use of the gradient of the function (or an approximation to it) in the locality of the current estimate(s) of the root.

This includes the following methods:

- [[Newton-Raphson Method]]
- [[Secant Method]]
- [[Modified Secant Method]]

Note the [[Limitation(s) for open methods]].

> [!NOTE] Mechanism
> We start with an initial guess for the root, $x_i$.
>
> We can find $f(x_i)$ and also the slope of the function, $m_i$ here.
>
> The next guess for the root, $x_{i+1}$, is where the tangent intersects with the $x$-axis.

![[Attachments/Screenshot 2026-05-27 at 17.00.13.png]]

> [!NOTE] Mathematical process for finding $x_{i+1}$
> Using the slope, $m_i$, of a line tangent (or approximately tangent) to our function at the current guess for our root, ($x_{i}$, $f(x_i)$).
> That is:
>
> $$
> m_{i}=\frac{0-f(x_{i})}{x_{i+1}-x_{i}}
> $$
>
> Which gives:
>
> $$
> x_{i+1}=x_i-\frac{f(x_{i})}{m_{i}}
> $$

![[Attachments/Screenshot 2026-05-28 at 09.47.37.png|348]]

# Flowchart

![[Attachments/Screenshot 2026-05-28 at 09.49.12.png]]

# Pseudocode

![[Attachments/Screenshot 2026-05-28 at 09.53.53.png]]
