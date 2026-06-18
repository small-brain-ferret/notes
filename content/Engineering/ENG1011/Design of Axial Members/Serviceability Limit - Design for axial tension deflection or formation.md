See [[Serviceability Limit State]].

The following three formulae can be combined to yield a convenient single equation to calculate the stretching or squashing of an axially loaded member:

1. [[stress]]:
   $\sigma = \frac{\text{Axial Force, }P}{\text{Cross-sectional area, }A}$
2. [[strain]]:
   $\epsilon=\frac{\text{Change in length, }\Delta L}{\text{Original length, }L}$
3. [[Young's Modulus E]]
   $E=\frac{\text{Stress}}{Strain}=\frac{\sigma}{\epsilon}$

> [!NOTE] Combined Equation - Serviceability Limit
> $\Delta L=\frac{PL}{AE}\leq \text{a given limiting deflection value}$
> We refer to 'AE' as the axial stiffness of a member (geometric stiffness A $\times$ material stiffness E).

# Example

> [!NOTE] Question
> A 2.25m long solid steel circular column of diameter 45mm experiences an axial tension force of 300kN.
>
> a) What is the strength limit state [[Factor of safety]] of this system?
>
> Assume $E_{\text{steel}}$ = 200,000 MPa & Yield strength = 250 MPa.
>
> ## Step 1: Calculate the acting stress using $\sigma=\frac{P}{A}$
>
> $$
> \begin{align}
> \sigma & =\frac{P}{A} \\
>  & =\frac{30000\text{ N}}{\pi(22.5)^2} \\
>   & =188.6\text{ MPa}
> \end{align}
> $$
>
> ## Step 2: Set limit state factor of safety to the maximum allowable stress divided by the applied stress.
>
> $$
> \begin{align}
> SF_{\text{strength}} & =\frac{250}{188.6} \\
>  & =1.32
> \end{align}
> $$

> [!NOTE] Question
> b) The column is not to change in length by more than 0.1%. Is this requirement met? What is the deflection limit state factor of safety here?
>
> ## Step 1: Determine the actual amount of deformation.
>
> $$
> \begin{align}
> \Delta L & =\frac{PL}{AE} \\
>  & = \frac{300000\times_{2250}}{\pi(22.5)^2*200000} \\
>   & =2.122mm
> \end{align}
> $$
>
> ## Step 2: Determine the safety factor
>
> $$
> \begin{align}
> SF & =\frac{\Delta L_{{max}}}{\Delta L} \\ 
>  & =\frac{2.25}{2.122} \\
>   & =1.06
> \end{align}
> $$
