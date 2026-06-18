---
publish: true
created: 2026-05-28T10:19:53.892+10:00
modified: 2026-05-28T12:58:28.955+10:00
---

There are several problems that could be encountered with the [[Newton-Raphson Method]]. This is an [[Open Method(s)]].

Some of these limitations similarly exist for [[Secant Method]] and [[Modified Secant Method]]. See [[Limitation(s) for open methods]].

1. Gradient at a tested point is zero
   - if the gradient at the latest testing point is 0, then the tangent line will never intersect the $x$-axis, causing a `ZeroDivisionError`.
2. Slow convergence is the root is at a turning point
   - if the root itself is at an extremum (i.e. a [[Local maximum (MVF)]] or  [[Local minimum (MVF)]] of the function), the method may cycle through many iterations before the desired level of precision is reached (i.e. it can be very slow to converge)
   - this is not always the case
   - depends on the relative value of(x) and f'(x)
3. Oscillation around a TP
   - if the initial guess is close to the TPs in the function, then the tangent intersections with the $x$-axis can oscillate about those TPs
   - this results in poor or non-existent convergence because the algorithm may go into an infinite loop
4. Oscillation if the root is at a symmetric point of inflection
   - if the root is at a symmetric point of inflection of the function, then the tangent intersections with the $x$-axis can oscillate about the point of inflection
   - This results in poor or non-existent
     ![[Attachments/Screenshot 2026-05-28 at 10.48.55.png]]
