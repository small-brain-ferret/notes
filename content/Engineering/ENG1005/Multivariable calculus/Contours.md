A useful tool for the [[Visualisation of multivariable functions (MVFs)]], particularly for 2 variables.

> [!NOTE] Definition
> Contours are curves on which the function $f(x,y)$ has a given constant value. ie. $f(x,y)=c$.

# Example

$f(x,y)=1+x^2+y^2$

![[Attachments/Screenshot 2026-05-06 at 05.47.08.png]]

Contours:
$f(x,y)=1+x^2+y^2=c$
where c is a constant greater than 1.
Rearranged gives us:
$x^2+y^2=c-1$
Which is a circle, centred at (0,0), with radius $\sqrt{c-1}$.

![[Attachments/Screenshot 2026-05-06 at 05.47.38.png]]

With 3 or more variables, we have [[level sets]]. These are surfaces with $f(x,y,z)=c$.

> [!NOTE] Relationship between the contour and [[Directional derivatives]]
> $\nabla f$ is perpendicular to contours.
>
> On a given contour, $f(x,y)$ is constant.
>
> Thus, if we look at the slope pointing along the direction of the contour, then that slope must be zero.
>
> Hence the [[Directional derivatives]] will be equal to zero along a contour, that is:
>
> $$
> \frac{\partial f}{\partial u}=0=\hat{u}\cdot \nabla f
> $$
>
> Hence, $\hat{u}$ is perpendicular to $\nabla f$,
>
> THUS:
> $\nabla f$ is perpendicular to contours.
