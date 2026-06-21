---
publish: true
aliases:
  - limiting yield strength design
created: 2026-05-29T16:01:54.754+10:00
modified: 2026-06-20T16:01:13.818+10:00
---

> [!NOTE] Strength limit
> $\frac{P}{A}\leq \sigma_{y} \implies P_{\text{max}}=\frac{\sigma_{y}\times A}{\text{Factor of safety}}$
> A is cross-sectional Area
> $\sigma_{y}$ is material [[yield stress]].
> See details in [[Determining the maximum load a specimen can carry without failing]]

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

See [[Factor of safety]].
