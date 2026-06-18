> [!NOTE] Definition
> One of [[Simpson's Rule(s)]].
>
> Derived from fitting a parabola to three points on a function, $f(x)$.

See [[composite Simpson's ⅓ Rule]].
[[Location truncation error(s) of Simpson's ⅓ rule]].

# Single application of Simpson's 1/3 rule

Consider:
Three equally spaced points ($x_1$, $f(x_1)$), ($x_2$, $f(x_2)$), and ($x_3$, $f(x_3)$), separated by the interval $h=x_{2}-x_1=x_{3}-x_{2}$, are fitted with a parabola.

![[Attachments/Screenshot 2026-05-29 at 00.48.38.png|277]]

The area under the parabola between $x_1$ and $x_3$ is the estimate for the integral of $f(x)$ from $x_1$ to $x_3$.

With the above derivation, it can be shown that Simpson's 1/3 rule for uniform segments of width $h$ is:

$$
I=\frac{h}{3}(f(x_{1})+4f(x_{2})+f(x_{3}))
$$
