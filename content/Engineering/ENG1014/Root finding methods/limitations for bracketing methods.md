---
publish: true
aliases:
  - limitation for bracketing methods
created: 2026-05-27T16:50:13.595+10:00
modified: 2026-06-11T15:07:40.490+10:00
---

Some important points about [[Bracketing Method]]:

1. you must "bracket" the root, or else neither the [[Bisection Method]] nor the [[False Position Method]] can make an estimate of the root to begin with.
2. the only difference between the two methods is in how they make their guess:
   - Bisection method always guesses halfway between $x_l$ and $x_u$
   - the false-position method makes a weighted guess, depending on which of $f(x_l)$ and $f(x_u)$ is closer to zero
3. Both methods are guarenteed to find a root.
   - if there is more than one root between the brackets, which root you find is down to luck.
4. In testing for convergence, must use the magnitude: $|f(x_r)|<$ precision.
   - if $f(x_r)$ is negative, it will be less than any precision, but not necessarily close to the root. So finding $f(x_r)<$ precision is not useful.
