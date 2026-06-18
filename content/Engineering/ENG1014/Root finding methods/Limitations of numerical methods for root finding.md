[[Numerical method for root finding]]

- [[Limitation(s) for open methods]]
- [[limitations for bracketing methods]]

# Limitations relevant to all methods

## Precision

When testing for whether to continue with another iteration, all of the algorithms will test whether the **function value** is close to 0, ie:

$$
f(x_{i+1})<\text{precision}
$$

Oftentimes, we may be more interested in knowing whether the x value ew have estimated is close to the true value of the root.

$$
|x_{\text{estimated}}-x_{\text{true}}|<precision
$$

However, this cannot be calculated exactly without prior knowledge of what the exact root should be (coz if we could why still do this whole process).

# Convergence

- if we repeat the calculation mulitple times, with smaller and smaller values of precision, we expect the answer will eventually become closer to the true value.
- If we find that the answer each time are similar, then we can assume that the answer has converged, and we have a reasonable level fo confidence that this is is the true answer
- At this stage, we no longer need to re-run the process at higher preciiosn.
