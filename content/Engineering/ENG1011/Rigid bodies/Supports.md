---
publish: true
aliases:
  - support
  - supports
  - Support
created: 2026-06-16T21:39:26.258+10:00
modified: 2026-06-17T14:34:46.054+10:00
---

> [!NOTE] Title
> A support prevents the:
>
> - translation of a body in a given direction by exerting a force on the body in the opposite direction
> - rotation of a body in a given direction by exerting a couple moment on the body in the opposite direction
>
> Thus, we can select the support to react against the members, allowing them to only move in certain directions.

Common types include:

- [[fixed support]]
- [[pinned support]]
- [[roller support]]
- [[cable]]

Others include:
![[Attachments/Screenshot 2026-06-16 at 21.48.45.png]]
![[Attachments/Screenshot 2026-06-16 at 21.49.04.png]]

# Example question - support reactions (linked to trusses)

Consider the truss below which is supported on a pin joint at point A and a roller joint at point C. Determine the reaction forces at the supports.

![[Attachments/Screenshot 2026-06-16 at 22.28.07.png]]

##### Step 1: Draw a [[FBDs with support reactions]]

![[Attachments/Screenshot 2026-06-16 at 22.29.23.png]]

##### Step 2: Analyse the resultant force in the $y$ direction

$$
\begin{align}
F_{y} & =0 \\
A_{y}-300-200 & =0 \\
A_{y} & =500\text{ N}
\end{align}
$$

##### Step 3: Analyse resultant moment at a location with a lot of unknowns/forces going through

$$
\begin{align}
\sum M_{A} & =0 \\
-400(2)-C_{x}(2)-200(2) & =0 \\
C_{x} & =-600\text{ N}
\end{align}
$$

##### Step 4: Analyse resultant force in the $x$ direction

$$
\begin{align}
\sum F_{x} & =0 \\
400+C_{x}+A_{x}+250 & =0 \\
A_{x} & =-50\text{ N}
\end{align}
$$

Note: $A_x$ is negative, which is opposite to what we assumed in the FBD. Thus, $A_x$ should act towards the left instead of the right.
