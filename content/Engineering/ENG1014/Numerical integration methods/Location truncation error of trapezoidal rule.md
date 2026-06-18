---
publish: true
aliases:
  - Location truncation errors of trapezoidal rule
created: 2026-05-28T15:24:36.788+10:00
modified: 2026-06-11T15:10:20.092+10:00
---

See [[Trapezoidal Rules]].

> [!NOTE] Definition
> As the number of segments increase, and the width of segments decrease, the difference  between the area under individual trapezia and the actual function decrease.
>
> This difference is called the **location truncation error**, $E_{T,\ local}$, where:
>
> $$
> E_{T,\ local}=-\frac{1}{12}f''(\xi)\ {h^3}
> $$
>
> - Where $\xi$ is some unknown value within the range $a<\xi<b$, and
> - $h=b-a$ (ie. the width of the trapezoids used to approximate the shape)

> [!NOTE] Scaling
> The local truncation error "scales with $h^3$", that is:
>
> $$
> E_{\text{T, local}}=O(h^3)
> $$
>
> Where O is "order".

i.e.
If the step size if halved in the [[Trapezoidal Rules]], then $E_{\text{T, local}}$ will be $\frac{1}{8}$ its original value.

It step size is tripled, $E_{\text{T, local}}$ will be 27-fold larger.

Note: If a function has a second derivative 0, trapezoidal integration will have 0 error.

> [!NOTE] Convergence
> As the number of individual segments gets larger, and each individual segment becomes smaller, the overall estimate of the integral _converges_ towards the true answer.
>
> If the segments become infinitely small, the limit of the total estimate will be the true value for the integral.
>
> Local truncation error will approach zero.

The [[global truncation error of trapezoidal rules]], $E_{\text{T, global}}$, over the entire integrand is the sum over all of the truncation error.

The local truncation error is also dependent on the nature of the function.

A trapezium will give the exact integral when $f(x)$ is a linear function.

Truncation errors start to appear when the second derivative of the function is non-zero. It becomes worse as the second and higher order derivatives of the function increase in magnitude.

![[Attachments/Screenshot 2026-05-28 at 23.38.25.png]]
