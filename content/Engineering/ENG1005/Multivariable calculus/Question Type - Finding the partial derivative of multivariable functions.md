See [[Partial derivatives]].

# Example 1

$f(x,y)=1+x^2+y^2$

$$
\begin{align}
\frac{\partial f}{\partial x} & =\frac{d}{dx}(f(x,y=y_{0})) \\
 & =\frac{d}{dx} (1+x^2+{y_{0}}^2) \\
  & =\frac{d}{dx}(1)+\frac{d}{dx}(x^2)+\frac{d}{dx}({y_{0}}^2) \\
   & =2x
\end{align}
$$

# Example 2

$f(x,y)=x y$

$$
\begin{align}
\frac{\partial f}{\partial x} & =\frac{d}{dx}(f(x,y_{0})) \\
 & =\frac{d}{dx}(x y_{0}) \\
  & =y_{0} \\
\end{align}
$$

We write $\frac{\partial f}{\partial x} =y$.

# Example 3: What is usually written

$f(x,y)=e^{x^2 y}cos(x+y)$

$$
\begin{align}
\frac{\partial f}{\partial x} & =\frac{\partial}{\partial x} (e^{x^2 y}cos(x+y)) \\
 & =\frac{\partial}{\partial x} (e^{x^2 y})\ cos(x+y)+(e^{x^2 y})\frac{\partial}{\partial x}(\cos(x+y)) \\
  & =2xye^{x^2y}\cos(x+y)+e^{x^2y}(-\sin(x+y))
\end{align}
$$

# Mr Fang's example

![[Attachments/Screenshot 2026-08-20 at 09.10.46.png]]
When there's a mixed partial derivative, look for non-single-variable expressions - these will not disappear. the rest will.

$$
f_{yx}=(e^{2y}\ln(x))_{yx}-\frac{2e^{2y}}{x}
$$
