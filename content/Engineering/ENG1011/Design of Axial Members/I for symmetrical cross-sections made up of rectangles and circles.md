Based the [[I for a Rectangular Section]] and [[I for a circular cross-section]],we can calculate the [[Second moment of Area (I)- moment of inertia]] for any symmetrical shape made up of rectangular and circular section.

$$$
\sum \left( \frac {bd^3}{12} \right)_{i}+\sum(\frac{\pi r^4}{4})_{i}
$$![[Screenshot 2026-06-20 at 07.14.54.png]]

However, the centroid of these parts must lie on the same [[centroidal axis]] line.
![[Screenshot 2026-06-20 at 07.16.23.png]]

# Example
Calculate I of the [[universal beam]] (UB) shown.
![[Screenshot 2026-06-20 at 07.19.47.png|213]]
##### Step 1: Determine a suitable composition of the shape to calculate I from using parts that share a centroidal axis line
A big rectangle minus two small rectangles. 
![[Screenshot 2026-06-20 at 07.21.03.png|269]]

##### Step 2: Calculate
$$$

\begin{align}
I\_{\text{xx}} & =\frac{120+204^3}{12}-\frac{55+180^3}{2}\times 2 \\
& =31.4\*10^6 \text{ mm}^4
\end{align}

$$

Alternatively, the shape can be flipped 90 degrees to be considered as the addition of three rectangles which share a centroidal axis line at the y-axis.
![[Screenshot 2026-06-20 at 07.23.36.png]]
$$
