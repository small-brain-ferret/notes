The buckle equation tells us the following:

$$
\begin{align}
L_{e} \to\infty, \ P_{cr}\to 0 \\
L_{e} \to 0, \ P_{cr}\to \infty
\end{align}
$$

The second limit statement is not physically possible. The most a section can carry in compression is its [[squash load]].

Thus, the area enveloped by the curve given by:

- $P_{cr}=\frac{\pi^2EI}{(L_{e})^2}$ (the [[buckle formula for columns with different end restraints|buckling formula]]), that is, $f(x)=\frac{k}{x^2}$, where $k=\pi^2EI$, and
- [[squash load]] $\sigma_{y}A$

gives the safe region.
Load above the [[squash load]] implies a failure mode of [[yielding]].
Load below the [[squash load]] implies a failure mode of [[buckling]].

![[Attachments/Screenshot 2026-06-20 at 14.18.18.png]]

# Example

A pin-ended 200mm $\times$ 1.5mm thick steel circular hollow section is loaded in compression. Assume $E=200000$ MPa, and $\text{yield strength}=250$ MPa.

Plot the compression failure envelope for this member and note where the following two cases lie on this envelope and thus what mode of failure occurs for each.

a) $L_{e}=0.5$m
b)$L_{e}=3$m

##### Step 1: Calculate the [[Second moment of Area (I)- moment of inertia]] and cross-sectional area

$$
\begin{align}
I & =\frac{\pi({r_{0}}^4-{r_{i}}^4)}{4}=\frac{\pi(10^4-8.5^4)}{4}=3754\text{mm}^4 \\ \\
A & =\pi({r_{0}}^2-{r_{i}}^2)=\pi(10^2-8.5^2)=87\text{mm}^2
\end{align}
$$

![[Attachments/Screenshot 2026-06-20 at 15.36.04.png]]

##### Step 2: Observe behaviour of envelope and desired values

a) 0.5: point lies on buckle curve above squash load

- failure mode = yield
- failure load = 22 kN
  b) 3: buckle point lies below squash load
- failure mode = buckling
- buckling load = 0.82 kN

To find length where failure mode changes from yield to buckling, equate squash load to buckle load capacity:

$$
\begin{align}
\sigma_{y}A & =\frac{\pi^2EI}{{L_{e}}^2} \\
250\times87 & =\frac{\pi^2\times200000*3754}{(L_{e})^2} \\
L_{e} & =583\text{ mm}=0.58\text{ m}
\end{align}
$$
