a [[circuit analysis methods|circuit analysis method]].

> [!NOTE] Steps for branch current method
> This method uses [[Kirchhoff's voltage law|KVL]] and [[Kirchoff's current law|KCL]] to form simultaneous equations with branch [[current|currents]] ($I$)as unknown variables.
>
> Step 1: Assign symbols to unknown $I$
>
> - assign direction arbitrarily
> - label polarity of voltage across resistor such that it conforms to direction of current assigned (in the resistor, current MUST flow from positive end to negative end)
> - if value of any $I$ is negative, true direction is opposite to the assigned direction. vice versa.
>
> Step 2: Apply KCL to minimize unknown variables
>
> - i.e. you would only need 2 unknowns for a node with 3 branches (the 3rd is found by applying KCL)
>
> Step 3: Write as many KVL equations as the number of unknowns
>
> Step 4: Find unknowns by solving the simultaneous KVL equations
>
> Step 5: Apply KCL to determine remaining branch currents

# Worked Example

![[Attachments/Pasted image 20260911132052.png|405]]

**Step 1: Assign symbols to unknown $I$**

- assign direction arbitrarily
- label polarity of voltage across resistor such that it conforms to direction of current assigned (in the resistor, current MUST flow from positive end to negative end)
  ![[Attachments/Pasted image 20260911131857.png|380]]

**Step 2: Apply KCL to minimise unknown variables**

$$
I_{3}=I_{1}-I_{2}
$$

**Step 3: Write as many KVL equations as the number of unknowns**

Write KVL for the left loop:

$$
\begin{align}
10-V_{1}-V_{2} & =0 \\
10-(I_{1}\times 10)-(I_{2}\times 10) & =0 \\
10 I_{1}+10 I_{2} & =10
\end{align}
$$

Write KVL for right loop:

$$
\begin{align}
V_{2}-V_{3}-15 & =0 \\
(I_{2}\times 10)-(I_{3}\times 10)-15 & =0 \\ 
(I_{2}\times 10)-((I_{1}-I_{2})\times 10)-15 & =0 \\
-10I_{1}+20I_{2} & =15
\end{align}
$$

**Step 4: Find unknowns by solving the simultaneous equations**

$$
\begin{align}
I_{1} & =\frac{1}{6} \text{ A} \\
I_{2} & =\frac{5}{6} \text{ A} \\
I_{3} & =-\frac{2}{3} \text{ A}
\end{align}
$$

Here, the negative sign of $I_3$ implies that the true direction of current is opposite to what was assigned.
