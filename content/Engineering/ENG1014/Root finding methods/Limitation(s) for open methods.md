- [[Limitation(s) for the Newton-Raphson method]]
- Note there are differences between the [[Newton-Raphson Method]] and Secant Methods, including [[Secant Method]] and [[Modified Secant Method]]
  - see [[Differences between the Newton-Raphson method and Secant method]].

# Relevant to all methods

There are some issues that affect both types of [[Open Method(s)]]. the [[Secant Method]]  has some issues in common to the [[Limitation(s) for the Newton-Raphson method]]:

**Item 1: Gradient at a tested point is zero**

- if the gradient at the latest testing point is 0, then the tangent line will never intersect the $x$-axis, causing a `ZeroDivisionError`.

**Item 3: Oscillation around a TP**

- if the initial guess is close to the TPs in the function, then the tangent intersections with the $x$-axis can oscillate about those TPs
- this results in poor or non-existent convergence because the algorithm may go into an infinite loop
