> [!NOTE] internal member forces in general
> For a [[planar truss|truss]] member (or a [[cable]] or rope), there are only [[axially loaded member|axial]] forces, H.
>
> ![[Attachments/Screenshot 2026-06-20 at 22.05.18.png]]
>
> If the cut is at an 'internal' pin connecting two members, then M$_\text{@pin}=0$, and thus there are two potential actions, H and [[shear]] forces V.
>
> ![[Attachments/Screenshot 2026-06-20 at 22.05.33.png]]
>
> If the cut is through a beam, there are three potential actions, V, H, and [[bending]] moment M.
>
> ![[Attachments/Screenshot 2026-06-20 at 22.05.55.png]]
>
> Three unknowns occur at the cut for a beam and we have three [[equilibrium of a rigid body|equations of equilibrium]] to solve.
>
> ![[Attachments/Screenshot 2026-06-20 at 22.09.22.png]]

![[Attachments/Screenshot 2026-06-20 at 22.15.12.png]]

> [!NOTE] General procedure for deriving internal forces at a point in a beam
> To find the **axial force, H**, use $\sum F_{x}=0$
> If **axial force = 0**, no external horizontal forces act on the beam.
> To find the **shear force, V**, use $\sum F_{y}=0$
> To find the **bending moment, M**, use $\sum M_{z}=0$

# Example

Determine the internal forces (H, V, M) 6m right of point A.
![[Attachments/Screenshot 2026-06-20 at 22.17.12.png]]
![[Attachments/Screenshot 2026-06-20 at 22.17.35.png]]

##### Step 1: calculate reaction forces

$$
\begin{align}
\sum M_{A} & =0 \\ 
-30\times 4-80\times 6+B_{y}\times 8 & =0 \\
B_{y} & =75 \text{ kN} \\
 \\
\sum F_{y} & =0 \\
A_{y} & =35\text{ kN} \\
 \\
\sum F_{x} & =0 \\
A_{x} & =-10\text{ kN}
\end{align}
$$

##### Step 2: Draw [[Free-body diagrams|FBDs]] and analyse

![[Attachments/Screenshot 2026-06-20 at 22.20.40.png]]\$\$
\begin{align}
\sum F\_{x} & =0 \\
H-10 & =0 \\
H=10\text{ kN} \\
\\
\sum F\_{y} & =0 \\
35-30-(20\times 2)-V & =0 \\
V & =-35 \text{ kN} \\
\\
\sum M\_{\text{@ cut}} & =0 \\
M-35\times 6+30\times 2+(20\times{2})\times{1} & =0 \\
M & =110\text{ kNm}
\end{align}

$$

![[Screenshot 2026-06-20 at 22.24.00.png]]
$$
