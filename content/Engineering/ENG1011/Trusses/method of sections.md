> [!NOTE]
> A truss in [[equilibrium]] will mean any subset of that system will be in equilibrium.
>
> Thus, we can analyse sections of a truss by cutting through a member and drawing an [[Free-body diagrams|FBD]], then assume that it is in equilibrium.

Using an [[Free-body diagrams|FBD]] to cut through members will expose the internal force as external forces.

Generally, the FBD does not cut through more than 3 members (i.e. 3 unknowns) since we only have 3 [[equilibrium of a rigid body|equations of equilibrium]].

We should be able to apply [[equilibrium of a rigid body|equations of equilibrium]] to solve for unknown forces.

> [!NOTE] General steps for method of sections
>
> 1. draw an FBD that cuts through 3 or less members
> 2. Determine the support reactions if they are involved in the FBD
> 3. Define a coordinate system that is convenient for analysis
> 4. apply the equilibrium equations to determine the unknown forces

# Example

Determine the forces in members BC, CG, and GF using the method of sections and indicate if the members are in tension or compression.
![[Attachments/Screenshot 2026-06-18 at 12.11.37.png]]

##### Step 1: draw an FBD that cuts through 3 or less members

Because our desired members are BC, CG and GF, we will cut through these 3 members.

![[Attachments/Screenshot 2026-06-18 at 12.12.55.png]]

##### Step 2: apply the [[equilibrium of a rigid body|equations of equilibrium]]

$$
\begin{align}
\sum M_{C} & =0 \\
-F_{GF}(2)+1000(4) & =0 \\
F_{GF} & =2000\text{ N} \\
\text{(compression)}
\end{align}
$$

$$
\begin{align}
\sum M_{G} & =0 \\
-F_{BC}(2)+1000(2) & =0 \\
F_{BC} & =1000\text{ N} \\
\text{(tension)}
\end{align}
$$

$$
\begin{align}
\sum F_{y} & =0 \\
F_{GC} \sin(45^{\circ})-1000 & =0 \\
F_{GC} & =1414.214\text{ N} \\
\text{(tension)}
\end{align}
$$

Note: we could've chosen the right side too, but that wold involve support reactions which would be more complicated.
