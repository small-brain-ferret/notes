> [!NOTE]
> As the [[centroidal axis|centroid]] of all the rectangles that make up an asymmetrical section no longer lie on the same axis, we need to determine the [[Second moment of Area (I)- moment of inertia]] about a parallel axis.
>
> $$
> \begin{align}
> I_{\text{N. A}} & =\int_{A} (y_{\text{N.A}})^2\ dA \\
>  & =\int_{A} (y-\text{shift})^2\ dA \\
>   & =I_{\text{z'z'}}+(shift)^2\times A_{i}
> \end{align}
> $$
>
> That axis typically being the [[neutral axis]] of the entire section.
>
> And we introduce a shift term - the distance between the [[centroidal axis|centroid]] of the rectangle being considered and the parallel axis
> ![[Attachments/Screenshot 2026-06-21 at 01.17.14.png]]

# Example

![[Attachments/Screenshot 2026-06-21 at 01.19.51.png]]
$y_{c}=\text{365mm}$, (shift)$_{1}$ = $510 - 365.5 = 144.5$mm,
(shift)$_{2}$ = $365.5 - 250 = 115.5$mm.

$I_{\text{section}}=\sum\left( \frac{bd^3}{12} \right)_{\text{individual rectangles}}+\sum A_{i}\times(shift_{i})^2$

$$
\begin{align}
I & =\frac{{200\times 20^3}}{12}+\frac{{10\times 500^3}}{12} \\
 & +20\times 200 \times (144.5)^2+10 \times 500 \times (115.5)^2 \\
  & =254522250\text{ mm}^4
\end{align}
$$
