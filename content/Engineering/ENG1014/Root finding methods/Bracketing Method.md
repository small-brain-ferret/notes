---
publish: true
aliases:
  - closed method
  - closed methods
  - bracketing methods
created: 2026-05-27T16:18:46.896+10:00
modified: 2026-06-11T15:09:29.154+10:00
---

A [[Numerical method for root finding]].
Note the [[limitations for bracketing methods]].

> [!NOTE] Definition
> Where the search for a particular root is conducted by approaching it from both sides.
>
> Requires the input of two starting points on either side of the root.

These include the following methods:

- [[Bisection Method]]
- [[False Position Method]]

> [!NOTE] Mechanism
> All bracketing methods have the essential starting point of knowing two values of $x$ at which the function has **opposite signs**:
>
> - lower bound $x_l$
> - upper bound $x_u$
>
> **As the function is assumed to be continuous and changes sign in the interval \[$x_l$, $x_u$], there must be at least one root in between.**

![[Attachments/Screenshot 2026-05-27 at 16.25.40.png|309]]

> [!NOTE] Algorithm
> We start by making a guess of the root, $x_r$.
>
> If $f(x_r)=0$, we have found the root.
>
> We need to iterate this process until we find the root.
>
> To perform the new iteration, we get a new interval by replacing $x_l$ or $x_u$ with $x_r$ (this is just another guess, but now we have more info to make it a better guess.)
>
> The bracket that is replaced is chosen based on the function values at $x_r$ and current $x_l$ or $x_u$.
>
> Now we can find the midpoint of the new interval.

# Choosing whether to replace $x_l$ or $x_u$ with $x_r$

Two possible cases:

1. $f(x_l)$ and $f(x_r)$ have the same sign. This implies $f(x_u)$ and $f(x_r)$ have different signs.
   - This is checked with $f(x_l)\times f(x_{r})>0$, which implies that $f(x_u)\times f(x_{r})<0$
   - This means the root must lie between $x_r$ and $x_u$.
   - Thus, we replace $x_l$ with $x_r$.
   - ![[Attachments/Screenshot 2026-05-27 at 16.32.46.png|376]]
2. 1. $f(x_l)$ and $f(x_r)$ have different signs. This implies $f(x_u)$ and $f(x_r)$ have the same sign.
   - This is checked with $f(x_l)\times f(x_{r})<0$, which implies that $f(x_u)\times f(x_{r})>0$
   - This means the root must lie between $x_l$ and $x_u$.
   - Thus, we replace $x_u$ with $x_r$.
   - ![[Attachments/Screenshot 2026-05-27 at 16.33.47.png|385]]

Once we have updated the brackets, we estimate the next guess of the root. Keep iterating until $f(x_{r})$ is close enough to 0.

# Flowchart

![[Attachments/Pasted image 20260527163539.png]]

# Pseudocode for generalised bracketing method

![[Attachments/Screenshot 2026-05-27 at 16.38.19.png]]
