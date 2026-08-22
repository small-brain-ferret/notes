$$
\begin{align}
z & =f(x,y)
\end{align}
$$

$\frac{dz}{dx}$ does not ignore the dependency on $y$.
Use shorthands $z_x$ or $z_y$.
Double/high-order derivatives:$(z_{x})_{x}$, $(z_{x})_{y}$

Normal vector (tangent planes and normal lines)

$$
\mathbf{n}=
\begin{pmatrix}
f_{x}(a,b)\\
f_{y}(a,b)\\ 
-1
\end{pmatrix}
$$

When $z$ is the subject of the function, the function is explicit.
There are times when $z$ is the function of $x$ and $y$

For implicit surfaces, try not to force $z$ into the subject.
You can try:

1. implicit partial differentiation
2. BIG F TRICK
   $z_x=-\frac{F_{x}}{F_{z}}$,    $z_y=-\frac{F_{y}}{F_{z}}$
   Rewrite the equation to equal 0, make big $F(x,y,z)$
   We temporarily consider all of them as independent variables
   We can now find $F_x$, $F_y$, and $F_z$
   contour curve vs level curve
