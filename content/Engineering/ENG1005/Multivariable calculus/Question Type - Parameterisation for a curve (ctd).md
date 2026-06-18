# Example 1

Find a parameterisation for the curve given by the intersection of the plane $x+y+z=0$ and the parabolic cylinder $z=y^2$.

Step 1: Set a parameter
Let
$y=t$

Step 2: Express the other variables in terms of this parameter
$z=y^2=t^2$
$x=-y-z=-t-t^2$

This gives the [[parametric representation]]:

$$
\begin{align}
x(t) & =-t-t^2 \\
y(t) & =t \\
z(t) & =t^2
\end{align}
$$

Step 3: Determine the values the parameter can take
all values

# Example 2

Find a parameterisation for the curve $x=2$, $y^2+2y+z^2=3$.

Step 1: Rewrite as a sum of squares

$$
\begin{align}
y^2+2y+1+z^2 & =4 \\
(y+1)^2+z^2 & =4 \\
\frac{(y+1)^2}{4} +\frac{z^2}{4}  & =1
\end{align}
$$

Step 2: Apply trig identity

$$
\begin{align}
\frac{(y+1)^2}{4} +\frac{z^2}{4}  & =1 \\
\cos^2(t)+\sin^2(t) & =1 \\
\implies\frac{y+1}{2}=\cos(t),\ \frac{z}{2} =\sin(t)
\end{align}
$$

Step 3: Rearrange to get the [[parametric representation]]

$$$
\begin{align}
x(t) & =2 \\
y(t) & =-1+2\cos(t) \\
z(t) & =2\sin(t)
\end{align}
$$Step 4: Determine the values the parameter can take
For this case, it should go one circle.
$0<=t<2\pi$
$$$
