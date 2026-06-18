> [!NOTE] Solving
>
> $$
> \begin{align}
> \frac{dy}{dx} & =f(x)g(y) \\
> f(x) & = \frac{1}{g(y)} \frac{dy}{dx} \\
> \int f(x) \,dx & =\int \frac{1}{g(y)}\,dy
> \end{align}
> $$

See [[Question Type - Solving first order separable ODEs]].

First order separable [[Ordinary differential equation]]s are a [[Classification of ODEs]] in the following form:

$$
\frac{dy}{dx}=f(x)g(y)
$$

Example of separable:

$$
\begin{align}
\frac{dy}{dx}+\frac{x}{y} & =0 \\
\implies \frac{dy}{dx} & =-\frac{x}{y} \\
 & =-x\cdot \frac{1}{y}
\end{align}
$$

Example of not separable:

$$
\frac{dy}{dx}=\cos(xy^2)
$$

Example of separable:

$$
\begin{align}
\cos(x)y^3 \frac{dy}{dx}-2y & =e^xy \\
\cos(x)y^3 \frac{dy}{dx} & =2y+e^xy \\
 & = (2+e^x)y \\
 \implies \frac{dy}{dx} & =\frac{{2+e^x}}{\cos(x)y^2} \\
  & =\frac{{2+e^x}}{\cos(x)}\cdot \frac{1}{y^2}
\end{align}
$$
