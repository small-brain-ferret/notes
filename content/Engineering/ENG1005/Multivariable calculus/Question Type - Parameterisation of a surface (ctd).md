Finding a parameterisation given an implicit or explicit representation.

# Example 2 - parameterisation of an ellipsoid

Find a parameterisation for $x^2+\frac{1}{4} y^2+\frac{1}{9} z^2=1$ (ellipsoid).

Step 1: Split the equation using $\sin^2(s)+\cos^2(s)=1$

Write the $z$-term as the $\sin^2(s)$ part, and the $x,y$ terms as the $\cos^2(s)$ part:

$$
\begin{align}
x^2+\frac{1}{4}y^2 &= \cos^2(s) \\
\frac{1}{9}z^2 &= \sin^2(s)
\end{align}
$$

From the second equation:

$$
\begin{align}
\frac{1}{9}z^2 &= \sin^2(s) \\
z^2 &= 9\sin^2(s) \\
z &= 3\sin(s)
\end{align}
$$

Step 2: Parametrise the $x,y$ part using $\cos^2(t)+\sin^2(t)=1$
Since

$$
x^2+\frac{1}{4}y^2=\cos^2(s)
$$

and
$\cos^2(s)\cos^2(t)+\cos^2(s)\sin^2(t)=\cos^2(s)$
split the two terms as:

$$
\begin{align}
x^2 &= \cos^2(s)\cos^2(t) \\
\frac{1}{4}y^2 &= \cos^2(s)\sin^2(t)
\end{align}
$$

Therefore:

$$
\begin{align}
x &= \cos(s)\cos(t) \\
y &= 2\cos(s)\sin(t)
\end{align}
$$

Step 3: Write the final parametrisation

$$
\begin{align}
x(s,t) &= \cos(s)\cos(t) \\
y(s,t) &= 2\cos(s)\sin(t) \\
z(s,t) &= 3\sin(s)
\end{align}
$$

with parameter ranges:

$$
\begin{align}
s &\in [-\pi,\pi] \\
t &\in [0,2\pi)
\end{align}
$$

Bonus: Checking

$$
\begin{align}
x^2+\frac{1}{4}y^2+\frac{1}{9}z^2
&= \cos^2(s)\cos^2(t)+\frac{1}{4}\left(2\cos(s)\sin(t)\right)^2+\frac{1}{9}\left(3\sin(s)\right)^2 \\
&= \cos^2(s)\cos^2(t)+\cos^2(s)\sin^2(t)+\sin^2(s) \\
&= \cos^2(s)\left(\cos^2(t)+\sin^2(t)\right)+\sin^2(s) \\
&= \cos^2(s)+\sin^2(s) \\
&=1
\end{align}
$$
