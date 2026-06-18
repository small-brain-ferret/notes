---
publish: true
aliases:
  - equations of equilibrium
created: 2026-06-16T22:13:41.333+10:00
modified: 2026-06-18T10:44:59.370+10:00
---

for a [[Rigid-body model]] to be in [[equilibrium]], it must satisfy both force equilibrium (doesn't translate) and moment equilibrium (doesn't rotate).

> [!NOTE] force and moment equilibrium
>
> $$
> \begin{align}
> F_{R}=\sum F=0\\
> (M_{R})_{O}=\sum Fd=0
> \end{align}
> $$

> [!NOTE]
> If a system is in equilibrium, then any subset of that system will also be in equilibrium.

# Example

Determine $A_y$, $B_x$, and $B_y$ if the beam is in equilibrium.
![[Attachments/Screenshot 2026-06-16 at 22.16.31.png]]

##### Step 1: Analyse resultant force in the horizontal direction

$$
\begin{align}
\sum F_{x} & =0 \\
600 \cos(45^{\circ})-B_{x} & =0 \\
B_{x} & =424.2641\text{ N}
\end{align}
$$

##### Step 2: Analyse resultant moment at a suitable point

$$
\begin{align}
\sum M_{B} & =0 \\
-(A_{y})(7)+(600\sin(45^{\circ})(5)+(100)(2)-(600\cos(45^{\circ}))(0.2) & =0 \\
A_{y}=319.4954 \text{ N}
\end{align}
$$
