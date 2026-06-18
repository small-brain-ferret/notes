There are a few algorithmic differences between the [[Secant Method]] and [[Newton-Raphson Method]]:
diff

1. The secant method needs to start with 2 guesses of the root
   - best to make the guesses fairly close together
   - unlike bracketed methods, the two guesses do not have to bracket the root
2. Secant method uses, approximation of the gradient, Newton method uses analytical gradient
3. In the Secant method, we need to keep track of the previous ($x_{i-1}$),
   current ($x_i$), and new ($x_{i+1}$)estimates of the root and the function at these values, updating these at each iteration

There are some issues affecting the Newton method (see [[Limitation(s) for the Newton-Raphson method]]), yet do not affect the Secant method:

**Item 2: Slow convergence is the root is at a turning point**

- if the root itself is at an extremum (i.e. a [[Local maximum (MVF)]] or  [[Local minimum (MVF)]] of the function), the method may cycle through many iterations before the desired level of precision is reached (i.e. it can be very slow to converge)
- this is not always the case
- depends on the relative value of(x) and f'(x)

**Item 4: Oscillation if the root is at a symmetric point of inflection**

- if the root is at a symmetric point of inflection of the function, then the tangent intersections with the $x$-axis can oscillate about the point of inflection
- This results in poor or non-existent
