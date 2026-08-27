> [!NOTE] double integral
> The double integral of $f(x,y)$ over a region $D$ is commonly denoted by:
>
> $$
> \int_{D} \int f(x,y)\ dA
> $$
>
> Here, $dA$ means integrating over an area, so $dA$ is $dxdy$.

> [!NOTE] area differential conversion
> $dA=dx\ dy=dy\ dx=r\ dr\ \theta$

> [!NOTE] double integrals
>
> General form:
>
> $$
> \int \int_{D}^{}  f(x,y)\, dA 
> $$
>
> area of region $D$.

For $z=f(x,y)>0$, defined over a rectangular domain $D={(x,y): a\leq x\leq b,\ c\leq y\leq d}$

> The volume under the [[surfaces|surface]] is given by either of the following iterated integrals:
>
> $$
> \int _{a}^b \int_{c}^df(x,y)\ dydx
> $$
>
> $$
> \int _{c}^d \int_{a}^bf(x,y)\ dxdy
> $$

> [!NOTE] computing double integrals
> To find $\int _{a}^b \int_{c}^df(x,y)\ dydx$ we first calculate the "inner integral" $\int_{c}^df(x,y)\ dy$ with respect to $y$, holding $x$ constant. This gives a function of $x$, say $\int _c^df(x,y)\ dy=g(x)$ Then, $\int _{a}^b \int_{c}^df(x,y)\ dydx=\int _{a}^bg(x)\ dx$

> [!NOTE] property for continuous functions
> Let $f$ be a continuous function defined on the rectangular domain ${(x,y): a\leq x\leq b, c\leq y\leq d}$.
> Then:
>
> $$
> \int _{a}^b \int_{c}^df(x,y)\ dydx=\int _{c}^d \int_{a}^bf(x,y)\ dxdy
> $$

> [!NOTE] Special case in the form $a(x)b(y)$
>
> $$
> \int _a^b \int _{c}^d f(x,y)\ dydx=\left( \int _{a}^ba(x)\ dx \right)\left( \int_{c}^d b(y) \ dx \right)
> $$

> [!NOTE] iterated integral for a [[type I region|type I domain]]
>
> {$(x,y): x\leq x\leq b,\ g(x)\leq y\leq h(x)$}
>
> $$
> \begin{align}
> \int _{D} \int f(x,y)\ dA = \int_{a}^b \int _{g(x)}^{h(x)}f(x,y)\ dydx
> \end{align}
> $$
>
> ![[Attachments/0e20ef3521af507eda7be7ffe2dc1de7.jpg]]

# Worked example - iterated integral or a type I domain

Find $\int _D \int x y^2\ dA$, where $D$ is the region in the first quadrant bounded by the curves $y=x^3$ and $y=\sqrt{ x }$.

## Step 1: Draw the region D

![[Attachments/28000f37678a2ef6729f43005240b6b4.jpg|221]]

And determine the point of intersection using simultaneous equations.

# Step 2: Set up double integral for type I region

$$
\begin{align}
\int _{a}^b \int_{g(x)}^{h(x)}f(x,y)\ dydx & =\int_{D}\int xy^2\ dA \\
 & =\int_{0}^1\int _{x^3}^\sqrt{ x }xy^2\ dy & dx \\
  & =\int_{0}^1x\left( \int_{x^3}^\sqrt{ x }y^2 dy \right) & dx \\
   & =\int_{0}^{1} x \left( \left[ \frac{y^3}{3} \right] \right)_{x^3}^\sqrt{ x }  & \, dx  \\
    & =\frac{5}{77}
\end{align}
$$

> [!NOTE] iterated integral for a [[type II region|type II domain]]
> {$(x,y): c\leq y\leq d,\ g(y)\leq x\leq h(y)$}
>
> $$
> \int _{c}^d \int _{g(y)}^h(y)f(x,y)\ dxdy
> $$
>
> ![[Attachments/0a97f417bdf89a4b40a7f6f9f598d0be.jpg]]

# Worked example - volume of a solid bounded by a surface

Find the volume of the solid bounded by the surface $z=9x^2y^2+3$ defined over the region ${(x,y):-1\leq x\leq{1},\ 0\leq y\leq{2}}$.

The required volume = $\int_{-1}^1 \int_{0}^2(9x^2y^2+3)\ dydx$ or $\int_{0}^2 \int_{-1}^1(9x^2y^2+3)\ dxdy$.

In this case, there isn't one with a calculation advantage. Thus, pick either.

$$
\begin{align}
I  & = \int_{-1}^1 \int_{0}^2(9x^2y^2+3)\ dy & dx \\
 & =\int_{-1}^1\left[ 9x^2 \frac{y^3}{3}+3y \right]_{0}^2 & dx \\
  & =\int_{-1}^124x^2+6 & dx \\
   & =[8x^3+6x]_{-1}^1 \\
    & =28
\end{align}
$$
