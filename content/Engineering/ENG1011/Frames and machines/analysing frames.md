> [!NOTE] general procedure
>
> 1. inspect the [[Frame|frame]] for any [[two-force members]]
> 2. draw [[Free-body diagrams]] of the entire system and of each member
> 3. it is important to note that the interaction forces between the FBD are shown to be equal in magnitude and opposite in direction
> 4. apply [[equilibrium of a rigid body|equations of equilibrium]] to solve for unknown forces
> 5. Once found [[shear force diagrams|SFD]], [[bending moment diagrams|BMD]] and axial forces can be found.
>
>    For a [[Frame]] comprising 'N' members, there will be N+1 sets of [[equilibrium of a rigid body|equations of equilibrium]] and N+1 [[Free-body diagrams|FBDs]].
>
>    If all external reactions in a frame can be determined, then the [[internal member forces]] between members can be determined from either member [[Free-body diagrams|FBD]].
>
>    If the structure is [[static indeterminancy|statically indeterminate]], all unknown forces can be determined using equilibrium when looking at all the FBDs.

# Example - horizontal members only

A [[Frame]] comprises two horizontal members connected by a [[pinned support|pin]] at B.
Determine the reaction forces at A and C and the internal pin forces at B.

Draw a [[shear force diagrams|SFD]] and a [[bending moment diagrams|BMD]] for the frame system.
![[Attachments/Screenshot 2026-06-21 at 16.02.01.png]]

##### Step 1: Inspect the frame for any two-force members

No two-force members. Both members have transverse forces on them.

##### Step 2: FBD

![[Attachments/Screenshot 2026-06-21 at 16.07.39.png]]

$$
\begin{align}
\sum F_{x} & =0 \\
A_{x}-6 & =0 \\
A_{x} & =6\text{ kN} \\
 \\
\sum F_{y} & =0 \\
A_{y}+C_{y}-16 & =0 \\
 \\
\sum M_{A} & =0 \\ 
A_{m}-(8\times 2)-(8\times 5)+6 C_{y} & =0
\end{align}
$$

4 unknowns, but only 3 equilibrium equations.
Thus, we must split our FBD into 2 separate FBDs.
![[Attachments/Screenshot 2026-06-21 at 16.11.09.png]]
Looking at the FBD on the right

$$
\begin{align}
\sum F_{x} & =0 \\
B_{x} & =0 \\
 \\

\end{align}
$$

The system is symmetrical, as the [[concentrated forces|point force]] is applied in the mid-span. Thus:

$$
B_{y}=C_{y}=\frac{8}{2}=4\text{ kN}
$$

Then, we can solve for $A_y$ from the previous equations.

$$
A_{y}=12 \text{kN}
$$

$$
A_{m}=32 \text{kN}
$$

![[Attachments/Pasted image 20260621171527.png]]

# Example - 3 pin arch

A [[three pin arch|3-pin arched 'frame']] comprises two members - one straight, one curved, connected by a pin at B. There are simple [[pinned support|pinned supports]] at A and C. A horizontal load is applied as shown. Assume AB follows the shape of a circular arc. Neglect member self-weight.
a) Confirm which members are [[multi-force members]], and which ones are [[two-force members]]?
b) calculate the [[Supports|support]] reaction forces and the [[internal member forces|internal]] pin forces at B
c) calculate the maximum [[bending]] moment in each member

![[Attachments/Screenshot 2026-06-21 at 17.37.53.png]]

b) use the [[analysing frames]] procedure
![[Attachments/Screenshot 2026-06-21 at 17.39.30.png]]

$$
\begin{align}
\sum M_{A} & =0 \\
-10\times 1.5+C_{x}\times 0+C_{y}\times 7 & =0 \\
C_{y} & =\frac{15}{7}\text{ kN}\approx 2.142\text{ kN} \\
 \\
\sum F_{y} & =0 \\
A_{y}+C_{y} & =0 \\
A_{y} & =-C_{y} \\
 & =-\frac{15}{7}\text{ kN} \\ \\
 \sum F_{x} & =0 \\
 A_{x}+10-C_{x} & =0 \\
 A_{x}-C_{x} & =-10
\end{align}
$$

$A_{y}$ is a negative number, which means $A_y$ should be pointing downwards not upwards like the diagram shows.

![[Attachments/Screenshot 2026-06-21 at 17.45.18.png|223]]![[Attachments/Screenshot 2026-06-21 at 17.45.32.png|259]]

Working with the FBD on the right:

$$
\begin{align}
\sum M_{b} & =0 \\
10\times 1.5 +\frac{15}{7}\times 4-C_{x}\times 3& =0 \\
C_{x} & =7.857\text{ kN}
\end{align}
$$

Now we can find the final unknown:

$$
A_{x}=C_{x}-10=-\frac{15}{7}\text{ kN}
$$

Overall, the reaction forces are:

$$
\begin{align}
C_{x} & =7.857\text{ kN} \\
A_{x} & =-\frac{15}{7}\text{ kN} \\
C_{y} & =\frac{15}{7} \text{ kN} \\
A_{y} & =-\frac{15}{7} \text{ kN}
\end{align}
$$

![[Attachments/Screenshot 2026-06-21 at 17.50.24.png]]

AS FB1 has no applied load, and only reaction forces, the forces at B can be easily calculated, as they will be opposite but equal to the forces at A.
![[Attachments/Screenshot 2026-06-21 at 17.52.15.png]]
Where e is the occuring of maximum [[bending]] moment.
![[Attachments/Screenshot 2026-06-21 at 17.53.25.png]]
e = R - 0.707R.
M = 3.03 e = 2.66 kNm
