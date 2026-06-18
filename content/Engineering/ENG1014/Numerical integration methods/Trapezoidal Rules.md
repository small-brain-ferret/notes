---
publish: true
aliases:
  - Trapezoidal Rule
created: 2026-05-28T13:57:52.185+10:00
modified: 2026-06-11T15:10:51.275+10:00
---

A [[Numerical integration methods|Numerical integration method]].

Practically, we would never use only a single segment for numerical integration.

A better estimate is given by subdividing the integrand into multiple segments and summing the trapezoilda area of each segment. This is why we use the [[Composite trapezoidal rule]].

# Single application of the trapezoidal rule

The trapezoidal rule is illustrated with a single trapezium spanning the bounds of the integral with limits at ($a$, $f(a)$) and ($b$, $f(b)$).

The area is a crude approximation to the area under the function between $a$ and $b$.

![[Attachments/Screenshot 2026-05-28 at 14.00.09.png|291]]

> [!NOTE]
> The area of the trapezium, and thus, the estimation of the integral, is:
>
> $$
> I = (b-a)\frac{{f(a)+f(b)}}{2}
> $$
