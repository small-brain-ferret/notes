For functions of one variable $f(x)$, the slope at a given point is $\frac{df}{dx}$.

For functions of several variables, the slope depends on which direction we are looking.

The slope "Looking" in the x-direction is called the partial derivative of $f(x,y)$ which respect to x. This is written as:

$$
\frac{\partial f}{\partial x}=\frac{d}{dx}(f(x,y=\text{constant}))
$$

This allows us to find the partial derivatives of multivariable functions.

See: [[Question Type - Finding the partial derivative of multivariable functions]]

This is important to understanding [[Directional derivatives]].

These tell us information about [[The gradient - nabla f]] of a slice of a MVF in the direction of an axis (ie. $x$ or $y$).

> [!NOTE] Higher Order Partial Derivatives
> For a single-variable function $f(x)$:
>
> $$
> \frac{d^2 f}{dx^2}=\frac{d}{dx}\left(\frac{df}{dx}\right)
> $$
>
> For a multivariable function $f(x,y)$:
>
> $$
> \begin{align}
> \frac{\partial^2 f}{\partial x^2}&=\frac{\partial}{\partial x}\left(\frac{\partial f}{\partial x}\right) \quad \text{(second derivative wrt $x$)}\\
> \frac{\partial^2 f}{\partial y \partial x}&=\frac{\partial}{\partial y}\left(\frac{\partial f}{\partial x}\right) \quad \text{(mixed)}\\
> \frac{\partial^2 f}{\partial x \partial y}&=\frac{\partial}{\partial x}\left(\frac{\partial f}{\partial y}\right) \quad \text{(mixed)}\\
> \frac{\partial^2 f}{\partial y^2}&=\frac{\partial}{\partial y}\left(\frac{\partial f}{\partial y}\right) \quad \text{(second derivative wrt $y$)}
> \end{align}
> $$
>
> Notes:
>
> - Mixed partials: $\frac{\partial^2 f}{\partial x \partial y}$ and $\frac{\partial^2 f}{\partial y \partial x}$
