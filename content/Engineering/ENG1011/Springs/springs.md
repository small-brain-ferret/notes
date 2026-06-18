---
publish: true
aliases:
  - spring
created: 2026-06-11T17:32:03.552+10:00
modified: 2026-06-16T17:30:08.475+10:00
---

> [!NOTE]
> Elastic members that exert a [[force]]/[[torque]] and absorb energy, which are usually stored for later release.
>
> The most common springs are compression and extension springs, which handle compression and tension loads. They restore axial motion.

Usually, but not necessarily made of metal.

Linear springs are governed by [[Hooke's law]].

They are mechanical devices that are an integral part of many mechanisms and machines.

Multiple springs may be connected in series and in parallel. See [[springs in series]] and [[springs in parallel]].

Types of springs:

- [[compression springs|compression]]
- extension
- torsion
- disc
- leaf
- volute

# Example: Spring system problem

A spring with stiffness $k=800$ N/m s supposed to hold a system in [[equilibrium]]. The spring has an unstretched length of 200mm. The cables BC and BD can only support 150 N each. Will this work?
![[Attachments/Screenshot 2026-06-16 at 16.02.23.png|282]]

##### Step 1: establish objectives and constraints.

- Spring and cable arrangement is fixed
- Cables BC and BD can only support 150 N each
- Determine if force in those cables exceed 150 N

##### Step 2: Specify system boundaries, assumptions.

- Entire system is in equilibrium
- Assumptions:
  - ring is modelled as a [[particle models|particle]]
  - cables and the spring are in tension
  - spring has linear behaviour (follows [[Hooke's law]])
  - spring has no limit load capacity (can handle any load)
  - tension force in each cable is uniform
  - ring, spring, and cables have no weight

##### Step 3: Establish the model.

- FBD: ring, cables, spring
- Equilibrium: $\sum F=ma=0$
- Hooke's law: $F_{k}=kx$
- variables: $F_{k}, \ F_{BC}, \ F_{BD}, \ k, x$
  ![[Attachments/Screenshot 2026-06-16 at 16.06.38.png]]

![[Attachments/Screenshot 2026-06-16 at 16.08.16.png]]

##### Step 4: analyse the model

Step 1: Calculate the deformation in the spring

$$
\text{spring extension} = 0.5-0.2=0.3\ \text{m}
$$

Step 2: Calculate the elastic force through Hooke's law

$$
\begin{align}
F_{k} & =kx \\
 & =800(0.3) \\
 & =240\ \text{N}
\end{align}
$$

Step 3: Apply the equilibrium equations to solve for forces
![[Attachments/Screenshot 2026-06-16 at 16.10.52.png]]

##### Step 5: Justify if behaviour is satisfactory

![[Attachments/Screenshot 2026-06-16 at 16.15.49.png]]

- Magnitude of forces are as expected.
- 150 N not exceeded in cable BC.
- 150 NN exceeded in cable BD. (will break)

Hence, arrangement will not work. BD may be replaced with a stronger cable or spring.

# Example: Mixed spring system

![[Attachments/Screenshot 2026-06-16 at 17.18.36.png|210]]

A bar of weight 100 N is supported by 4 springs in the arrangement shown in the figure below. The springs have the same stiffness of $k$. Determine the force carried in each spring.

##### Step 1: Draw a FBD of the bar

![[Attachments/Screenshot 2026-06-16 at 17.24.17.png|221]]
![[Attachments/Screenshot 2026-06-16 at 17.23.59.png|201]]

##### Step 2: Simplify the segment of springs in series into a singular spring with the equivalent $k$

$$
\begin{align}
\frac{1}{k_{e}} & =\frac{1}{k}+\frac{1}{k} \\
 & =\frac{2}{k} \\
 k_{e} & =\frac{k}{2}
\end{align}
$$

##### Step 3: Use equilibrium equations to find the unknown forces

$$
\begin{align}
\sum F_{y} & =0 \\
K_{e} \ x+k\ x+k\ x-100 & =0 \\
\frac{k}{2}x+2k\ x & =100 \\
2.5k\ x & =100 \\
k\ x & =40\text{ N} \\

\end{align}
$$

##### Answer:

$$
\begin{align}
\text{lower springs}=40\text{ N} \\
\text{upper springs}=\frac{k\ x}{2}=20\text{ N}
\end{align}
$$
