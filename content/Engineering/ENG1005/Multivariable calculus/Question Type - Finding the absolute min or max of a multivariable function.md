See [[Absolute maxima and minima of functions]].
[[Lagrange multipliers]] are usually useful in finding maxima and minima subject to constraints. Allows you to find [[Absolute maxima and minima of functions]] with less work.

# Example 1 - Rectangular domain

What are the absolute maximum and minimum of $f(x,y)=-(x^2-1)(y^2-1)$ on the domain $|x|<2$, $|y|<2$.

Step 1: Find the critical points (see [[Question Type - Finding critical points of a multivariable function]] example 2)

Step 2: Characterise the critical points
[[Use of the Hessian in characterising Critical points]]
Minimum at $(0,0)$
Saddle points at $(\pm 1, \pm 1)$

Step 3: Evaluate the value of $f(x,y)$ at all non-saddle critical points (note principle 2 of [[Absolute maxima and minima of functions]])

$$
\begin{align}
f(0,0) & =-(0-1)(0-1) \\
 & =-1 \\
\end{align}
$$

Step 4: On each boundary, reduce the function to a single-variable function, find their respective critical points and evaluate.

Step 4a: For a domain of $a<x<b$, sub the boundary value $x=a$ into $f(x,y)$
For the example $|x|<2$ (ie. $-2<x<2$), plug in $x=-2$:

$$
\begin{align}  
g(y)  
&=f(-2,y) \\  
&=-(4-1)(y^2-1) \\  
&=-3(y^2-1)  
\end{align}  
$$

$$
\begin{align}  
g'(y)&=-6y \\  
-6y&=0 \\  
y&=0  
\end{align}  
$$

$$
\begin{align}  
g(0)  
&=-3(0^2-1) \\  
&=3  
\end{align}  
$$

Step 4b: For a domain of $a<x<b$, sub the boundary value  $x=b$ into $f(x,y)$
Step 4c: For a domain of $c<y<d$, sub the boundary value $y=c$ into $f(x,y)$

$$
\begin{align}  
g(x)  
&=f(x,-2) \\  
&=-(x^2-1)(4-1) \\  
&=-3(x^2-1)  
\end{align}  
$$

$$
\begin{align}  
g'(x)&=-6x \\  
-6x&=0 \\  
x&=0  
\end{align}  
$$

$$
\begin{align}  
g(0)  
&=-3(0^2-1) \\  
&=3  
\end{align}  
$$

Step 4d: For a domain of $c<y<d$, sub the boundary value $y=d$ into $f(x,y)$

> \[!NOTE regarding symmetry]
> Only Steps 4a and 4c are shown in full. The function
>
> $$
> f(x,y)=-(x^2-1)(y^2-1)
> $$
>
> depends only on $x^2$ and $y^2$. Therefore replacing $x$ with $-x$ or replacing $y$ with $-y$ does not change the value of the function. That is, $f(-x,y)=f(x,y)$, $f(x,-y)=f(x,y)$, and $f(-x,-y)=f(x,y)$
> Hence the boundary calculations for:
>
> - $x=-2$ and $x=2$
> - $y=-2$ and $y=2$
>   are identical, so only two boundary calculations are shown. In general, all boundaries should still be checked separately unless this symmetry can be clearly identified.

Step 5: Check the value of $f(x,y)$ of corner points $(a,c),\ (a,d),\  (b,c), \ (b,d)$
In this case, the corners are $(2,2), \ (2, -2), \ (-2, -2), \ (-2, 2)$.

Given the symmetry of the function, all corner points produce the same function value, so only one calculation is required.

$$
\begin{align}  
f(2,2)  
&=-(4-1)(4-1) \\  
&=-9  
\end{align}  
$$

Step 6: Compare all values obtained and reach a conclusion.

- a) interior critical points
  $f(0,0)=-1$

- b) boundary local max/min
  $f(-2,0)=f(2,0)=f(0,-2)=f(0,2)=3$

- c) corner points
  $f(-2,-2)=f(-2,2)=f(2,-2)=f(2,2)=-9$

$\therefore$
absolute maximum = $3$, occurring at $(-2,0), \ (2,0), \ (0,-2), \ (0,2)$
absolute minimum = $-9$, occurring at $(-2,-2), \ (-2,2), \ (2,-2), \ (2,2)$

# Example 2 - circular domain

What are the absolute maximum and minimum of $f(x,y)=-(x^2-1)(y^2-1)$ on the domain $x^2+y^2 \le 4$.

Step 1 to Step 3: See example 1

Step 4: On the boundary, use the boundary constraint to reduce the function to a single-variable function. Then find and evaluate the critical points of the resulting boundary function.

In this case, the boundary is given by (note rearrangement favours substitution into $f(x,y)=-(x^2-1)(y^2-1)$):

$$
\begin{align}
x^2+y^2 & =4 \\
y^2 & =4-x^2 \\
\end{align}
$$

$$
\begin{align}
g(x)
&=-(x^2-1)((4-x^2)-1) \\
&=-(x^2-1)(3-x^2) \\
&=x^4-4x^2+3
\end{align}
$$

$$
\begin{align}
g'(x)
&=4x^3-8x \\
&=4x(x^2-2)
\end{align}
$$

$$
\begin{align}
4x(x^2-2)&=0 \\
x&=0,\ \pm\sqrt{2}
\end{align}
$$

$$
\begin{align}
g(0)
&=0^4-4(0)^2+3 \\
&=3
\end{align}
$$

$$
\begin{align}
g(\pm\sqrt{2})
&=(\sqrt{2})^4-4(\sqrt{2})^2+3 \\
&=4-8+3 \\
&=-1
\end{align}
$$

Since $y^2=4-x^2$:

- when $x=0$, $y=\pm2$
- when $x=\pm\sqrt{2}$, $y=\pm\sqrt{2}$

So the boundary values are:

- $f(0,\pm2)=3$
- $f(\pm\sqrt{2},\pm\sqrt{2})=-1$

Step 5: Check the value of $f(x,y)$ of corner points.
This domain is circular and therefore has no corner points.

Step 6: Compare all values obtained and reach a conclusion.

- a) interior critical points\
  $f(0,0)=-1$

- b) boundary local max/min\
  $f(0,\pm2)=3$\
  $f(\pm\sqrt{2},\pm\sqrt{2})=-1$

- c) corner points\
  None
  $\therefore$
  absolute maximum = $3$, occurring at $(0,2), \ (0,-2)$
  absolute minimum = $-1$, occurring at $(0,0), \ (\sqrt{2},\sqrt{2}), \ (\sqrt{2},-\sqrt{2}), \ (-\sqrt{2},\sqrt{2}), \ (-\sqrt{2},-\sqrt{2})$
