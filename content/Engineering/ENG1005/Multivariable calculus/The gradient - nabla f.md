Useful for finding the [[Directional derivatives]] of MVFs. Related to [[Partial derivatives]].

Useful for finding [[Tangent planes]] and [[Critical points]].

> [!NOTE] Definition
>
> $$
> \nabla f=\begin{pmatrix}\frac{\partial f}{\partial x}\\\frac{\partial f}{\partial y}\end{pmatrix}=\begin{pmatrix}
> {f_{x}(a,b)}\\{f_{y}(a,b)}
> \end{pmatrix}
> $$

> [!NOTE] NOTE
> $|\nabla f|$ is the magnitude of the largest slope.
>
> $\nabla f$ points in the direction of largest slope.
>
> Derivation:
>
> $$
> \begin{align}
> \frac{\partial f}{\partial u} & =\hat{u}\cdot \nabla f \\
>  & =|\hat{u}|\ |\nabla f|\ \cos(\theta) \\
>  & =|\nabla f|\ \cos(\theta)
> \end{align}
> $$
>
> Since the largest possible value of $cos(\theta)$ is 1 (ie. when $\theta=0$), the magnitude of $\nabla f$ is the largest slope of $f(x,y)$ looking in the direction $\hat{u}$.

See [[Question Type - Finding the largest slope of MVFs]]
