Used for finding maxima and minima subject to constraints. Used for finding [[Absolute maxima and minima of functions]] with less work. See [[Question Type - Finding min or max of a 2 variable function subject to a constraint UNFINISHED]]

![[Attachments/Pasted image 20260506055700.png]]

Without constraints, extrema occur when:

$$
\nabla f = 0 
$$

However, with a constraint, we are restricted to moving only along a curve or surface.

At a constrained maximum/minimum:

- we cannot move further uphill/downhill while remaining on the constraint
- the constraint curve becomes tangent to a contour of $f(x,y)$

For a level curve: $f(x,y)=\text{constant}$, the gradient vector $\nabla f$ is perpendicular to the contour (see [[Properties of nabla f]]).

Similarly, for the constraint $g(x,y)=$constant, the gradient vector $\nabla g$ is perpendicular to the constraint curve.

At the touching point:

- the contour of $f(x,y)$
- and the constraint curve
  are tangent.

Therefore their perpendicular vectors are parallel:

$$
\nabla f \parallel \nabla g
$$

Hence:

$$
\nabla f = \lambda \nabla g
$$

where $\lambda$ is the Lagrange multiplier.
