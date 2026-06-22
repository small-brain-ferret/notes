---
publish: true
aliases:
  - method of joints
created: 2026-04-16T08:21:01.621+10:00
modified: 2026-06-22T09:21:35.113+10:00
---

> [!NOTE]
> A truss in equilibrium will mean each of its joints is also in equilibrium.
>
> As such, we can analyse free-body diagrams of each joint ([[particle models|particle]]) using equilibrium equations $\sum F_x =0$ and $\sum F_y =0$.

> [!NOTE] General steps for method of joints
>
> 1. Draw the [[Free-body diagrams|FBD]] of a joint having at least one known force and at most two unknown forces
>    if this joint is a [[Supports|support]], then the reaction may need to be calculated first
> 2. Defining a coordinate system convenient for analysis
> 3. Applying the [[equilibrium of a rigid body|equations of equilibrium]] to determine the unknown forces.
>    A member in compression "pushes" on a joint.
>    A member in tension "pulls" on the joint.
> 4. Successively analysing the remaining joints in the system.

# Example

![[Attachments/Screenshot 2026-06-18 at 10.46.45.png]]
Determine the forces in AB and BC using the method of joints.

##### Step 1: draw an FBD at a desired joint

In this case, draw one around joint B.
We assume AB to be in tension (since force is acting away from B), and force in BC to be in compression (since force is acting towards B).
![[Attachments/Screenshot 2026-06-18 at 10.48.45.png]]

> [!IMPORTANT]
> The sense of an unknown member force can be assumed, which can be verified after calculations.
>
> A positive value indicates that the sense is correct, whereas a negative value indicates that the sense shown on the [[Free-body diagrams|FBD]] is opposite.

##### Step 2: Apply equilibrium equations

$$
\begin{align}
\sum F_{x} & =0 \\
-F_{BC}\sin(45^{\circ})+500 & =0 \\
F_{BC} & =707.1068\text{ N}
\end{align}
$$

$$
\begin{align}
\sum F_{y} & =0 \\
-F_{BA}+F_{BC}\cos(45^{\circ}) & =0 \\
F_{BA} & = 500\text{ N}
\end{align}
$$

# Example 1

Determine the forces in each member of the truss using the method of joints and indicate if the members are in tension or compression.
![[Attachments/Screenshot 2026-06-18 at 10.56.07.png]]
Upon inspection, there isn't a joint with 2 or fewer unknowns, thus we need to solve for reactions first.

##### Step 1: Draw an [[Free-body diagrams|FBD]]

![[Attachments/Screenshot 2026-06-18 at 10.57.02.png]]

##### Step 2: Apply [[equilibrium of a rigid body|equations of equilibrium]] to solve for reactions

Preferably start with an equation with only one unknown.

$$
\begin{align}
\sum F_{x} & =0 \\
-C_{x}+600 & =0 \\
C_{x} & =600N
\end{align}
$$

$$
\begin{align}
\sum M_{C} & =0 \\
-A_{Y}(6)+400(3)+600(4) & =0 \\
A_{y} & =600N
\end{align}
$$

$$
\begin{align}
\sum F_{y} & =0 \\
A_{y} -400-C_{y}& =0 \\
C_{y} & =200N
\end{align}
$$

##### Step 3: Perform the method joints

Choose a joint with at least one unknown and at most 2 unknowns.

In this case, that would be joint A or C.
![[Attachments/Screenshot 2026-06-18 at 11.03.15.png]]

$$
\begin{align}
\sum F_{y} & =0 \\
600-F_{AB}\left( \frac{4}{5} \right) & =0 \\
F_{AB} & =750\text{ N}
\end{align}
$$

i.e. 750 N compression

$$
\begin{align}
\sum F_{x} & =0 \\
F_{AD}-F_{AB}\left( \frac{3}{5} \right) & =0 \\
F_{AD} & =750\left( \frac{3}{5} \right) \\
F_{AD} & =450N
\end{align}
$$

i.e. 450 N tension
![[Attachments/Screenshot 2026-06-18 at 11.05.32.png]]

$$
\begin{align}
\sum F_{x} & =0 \\
-450+600+F_{DB}\left( \frac{3}{5} \right) & =0 \\
F_{DB} & =-250\text{ N}
\end{align}
$$

i.e. 250 N tension

$$
\begin{align}
\sum F_{y} & =0 \\
-F_{DB}\left( \frac{4}{5} \right)-F_{DC} & =0 \\
F_{DC} & =-(-250)\left( \frac{4}{5} \right) \\
F_{DC} & =200\text{ N}
\end{align}
$$

i.e. 200 N compression

![[Attachments/Screenshot 2026-06-18 at 11.07.35.png]]

$$
\begin{align}
\sum F_{x} & =0 \\
F_{CB}-600 & =0 \\
F_{CB} & =600\text{ N}
\end{align}
$$

i.e. 600 N compression

equilibrium check in y-direction since we have no unknowns:

$$
\begin{align}
\sum F_{y} & =0 \\
200-200 & =0
\end{align}
$$
