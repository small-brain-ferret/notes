See [[Bending stress equation]].
When finding the values of the maximum tension or compression, we must look for a combination of $M_{\text{max}}\times y_{\text{max}}$, not just $M_{\text{max}}$.

# Example

A cantilever [[beam]] with the T-section shown, supports a uniformly [[distributed loads|distributed load]] and a [[concentrated forces|point load]] at its tip. It is made of cast iron, which is much stronger in compression than in tension. What are the maximum tension and compression bending stresses and where do they occur?

![[Attachments/Screenshot 2026-06-21 at 12.25.16.png]]

![[Attachments/Screenshot 2026-06-21 at 12.25.59.png]]

See [[neutral axis]] for how the centroid and [[Second moment of Area (I)- moment of inertia]] is calculated. From this we know:
$y_c=365.5$mm, $I=254.52\times 10^6$mm$^4$.

##### Step 1: draw the [[bending moment diagrams|BMD]]

Finding reactions: $A_{y}=30$kN, $M_{a}=25$kNm
Draw an [[shear force diagrams|SFD]], then based on that, draw the BMD. Remembering [[sign convention for internal axial forces]].
![[Attachments/Screenshot 2026-06-21 at 12.52.02.png]]

##### Step 2: Use the [[Bending stress equation]] to find bending stresses

At minimum bending moment:

$$
\begin{align}
M & =-25\text{ kNm} \\
y_{\text{tension}} & =154.5\text{ mm} \text{ occurs at the top}\\
y_{\text{comp}} & =365.5 \text{ mm} \\
\sigma_{\text{comp}} & =\frac{{25\times 10^6\times 365.5}}{I} \\
 & =26.1\text{ mPa} \\
\sigma_{\text{tension}} & =\frac{{25\times 10^6\times 154.5}}{I} \\
 & =15.2 \text{ mPa}
\end{align}
$$

At maximum bending moment

$$
\begin{align}
M & =20\text{ kNm} \\
y_{\text{tension}} & =364.5\text{ mm} \text{ occurs at the bottom}\\
y_{\text{comp}} & =154.5\text{ mm} \\
\sigma_{\text{comp}} & =\frac{{20\times 10^6\times 154.5}}{I} \\
 & =12.1\text{ mPa} \\
\sigma_{\text{tension}} & =\frac{{20\times 10^6\times 365.5}}{I} \\
 & =28.7 \text{ mPa}
\end{align}
$$
