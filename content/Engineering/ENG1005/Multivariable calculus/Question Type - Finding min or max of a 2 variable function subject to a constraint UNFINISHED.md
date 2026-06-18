The [[Absolute maxima and minima of functions]] like f(x,y) subject to a constraint $g(x,y)$ can be found by simultaneously solving:

$$
\nabla f = \lambda \nabla g
$$

and

$$
g(x,y)=c
$$

where:

- $f(x,y)$ is the function being optimised
- $g(x,y)=c$ is the constraint

# Example 1

Minimise $x^2+y^2$ subject to $x+2y=1$.
Step 1: Calculate $\nabla f$
$\nabla f=\begin{bmatrix} 2x \\ 2y \end{bmatrix}$
Step 2: Calculate $\nabla g$
$\nabla g=\begin{bmatrix} 1 \\ 2 \end{bmatrix}$Step 3: Solve $\nabla f = \lambda \nabla g$  and $g(x,y)=c$ simultaneously for $x$ and $y$
$\begin{bmatrix} 2x \\ 2y \end{bmatrix}=\lambda\begin{bmatrix} 1 \\ 2 \end{bmatrix}$

$$
\begin{align}
2x & =\lambda \\
 & \implies x=\frac{\lambda}{2} \\
2y & =2 \lambda \\
 & \implies y=\lambda
\end{align}
$$

$$
\begin{align}
x+2y & =1 \\
\frac{1}{2} \lambda+2 \lambda & =1 \\
\frac{5}{2} \lambda & =1 \\
\implies &  \lambda=\frac{2}{5} \\
\implies &  x=\frac{1}{2} \cdot \frac{2}{5} =\frac{1}{5}, \ y=\frac{2}{5}
\end{align}
$$

Step 4: Plug solved values of $x$ and $y$ back into $f(x,y)$ to determine the minimum/maximum.

$$
\begin{align}
f\left( \frac{1}{5} , \frac{2}{5} \right) & =\left( \frac{1}{5} \right)^2+\left( \frac{2}{5} \right)^2 \\
 & =\frac{1}{25} +\frac{4}{25} \\
  & =\frac{1}{5}
\end{align}
$$

# Example 2
