> [!NOTE] Electronics - the principle of superposition
> In a linear circuit with a number of [[independent voltage source|independent sources]], the response can be found by summing the responses to each independent source acting alone, with all other independent sources set to 0.

Only applies to [[linear circuit|linear circuits]].

# Application of the principle of superposition

![[Attachments/Pasted image 20260911155817.png|388]]

Applying KCL at node B:

$$
\frac{V_{S_{1}}-V_{b}}{R_{1}}+\frac{V_{S_{2}}-V_{b}}{R_{3}}-\frac{V_{b}}{R_{2}}=0
$$

rearranging to keep known variables and unknown variables on different sides:

$$
\left( \frac{1}{R_{1}}+\frac{1}{R_{2}}+\frac{1}{R_{3}} \right)V_{b}=\frac{1}{R_{1}}V_{S_{1}}+\frac{1}{R_{3}}V_{S_{2}}
$$

Taking $G_{1}=\frac{1}{R_{1}}$, $G_{2}=\frac{1}{R_{2}}$, $G_{1}=\frac{3}{R_{3}}$, solving for node voltage at B:

$$
V_{b}=\frac{G_{1}}{G_{1}+G_{2}+G_{3}}V_{S_{1}}+\frac{G_{3}}{G_{1}+G_{2}+G_{3}}V_{S_{2}}
$$

- The node voltage $V_b$ is the weighted sum of the source voltages, _i.e._ sum of
  source voltage times a constant coefficient.
- The values of the coefficient depend on the values of the resistors only

Thus, if $V_{S_{2}}$ is set to 0, we get the contribution that $V_{S_{1}}$ makes to the node voltage $V_{b}$ , vice versa.

$$
\begin{align}
V_{b, 1} & =\frac{G_{1}}{G_{1}+G_{2}+G_{3}}V_{s_{1}} \\ \\

V_{b, 2} & =\frac{G_{3}}{G_{1}+G_{2}+G_{3}}V_{s_{2}} 
\end{align}
$$

# What does setting a source to 0 mean?

- **Setting a voltage source to zero or "killing" a voltage source**: To keep the voltage across an independent voltage source at zero regardless of the current flowing through it, we can replace it with a **short circuit**.

- **Setting a current source to zero or "killing" a current source**: To make the current through a branch (containing the current source) zero regardless of the voltage across it, replace the current source with an **open circuit**.

# Worked example

Use the principle of superposition to find the current I in the circuit shown.
![[Attachments/Screenshot 2026-09-11 at 16.45.26.png|423]]
**Step 1: Keep the 2A current source and set other source to 0. This leaves us with a basic single-source circuit to find $I_1$.**
![[Attachments/Pasted image 20260911165004.png|402]]

$$
I_{1}=\frac{2\text{ A}}{2}=1.0\text{ A}
$$

**Step 2: Keep the 3V source and set the other source to 0. We can find $I_2$.**
![[Attachments/Pasted image 20260911165323.png|385]]

$$
I_{2}=-\frac{3}{1+1}=-1.5A
$$
