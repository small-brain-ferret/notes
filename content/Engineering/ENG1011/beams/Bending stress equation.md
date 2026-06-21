---
publish: true
aliases:
  - load-carrying capacity of a beam
  - load-carrying strength of a beam
created: 2026-06-21T00:27:11.203+10:00
modified: 2026-06-21T01:01:23.466+10:00
---

Derived from the [[Simple Beam theory]].
Allows us to calculate the load-carrying capacity of the beam.

> [!NOTE] bending stress equation
>
> $$
> \sigma=EKy=E\left( \frac{M}{EI} \right)y=\frac{My}{I}
> $$
>
> where:
> $\sigma=$ the bending stress (MPa (N/mm$^2$))
> $I=$ the [[Second moment of Area (I)- moment of inertia]]
> $y=$ the distance from the [[neutral axis]]
> $M=$ the internal [[load (w), shear force (V), and bending moment (M)|bending moment]] in the [[beam]]
>
> ![[Attachments/Screenshot 2026-06-21 at 00.30.15.png]]
>
> Consider bending stresses not as '+' or '-' but as 'tension' or 'compression'.

> [!NOTE] bending stress beam design
>
> $$
> \sigma=\frac{MY}{I}=\frac{M}{Z}\leq \sigma_{y}
> $$
>
> where
> Z is the elastic section modulus found in the section design tables.

> [!NOTE] Finding max bending stress
>
> 1. look along the beam to find $M_{max}$, which occurs when V=0.
> 2. Substitute $M_{max}$ into the stress equation

# Example

A bridge, made of RHS, is used to support the loading shown. Is the strength of the steel bridge adequate? Assume $\sigma_{y}=250$ MPa.
![[Attachments/Screenshot 2026-06-21 at 00.33.29.png]]

##### Step 1: Find I

$$
I=\left( \frac{b^4}{12} \right)_{\text{outer}}-\left( \frac{b^4}{12} \right)_{\text{inner}}=162.8\times 10^6 \text{mm}^4
$$

##### Step 2: Draw a [[bending moment diagrams]]

2a) Calculate reactions

$$
\begin{align}
\sum M_{A} & =0 \\
-72\times 4-20 \times 12 + B_{y}\times 8 & =0 \\
B_{y} & =66 \text{ kN} \\
 \\
\sum F_{y} & =0 \\
A_{y}+B_{y}-72-20 & =0 \\
A_{y} & =26 \text{ kN} \\
 \\
\sum F_{x} & =0 \\
A_{x} & =0
\end{align}
$$

![[Attachments/Screenshot 2026-06-21 at 00.45.57.png]]
![[Attachments/Screenshot 2026-06-21 at 00.48.32.png]]
$M_{\text{max}}=80$ kNm, $y_{\text{max}}=150$ mm, $I=162.8\times 10^6$ mm$^4$

$$
\begin{align}
\sigma_{comp(max)} \\
 & =\frac{My}{I}=80\times 10^6 \times 150 \times 162.8 \times 10^6 \\
  & =73.7\text{ MPa} \\
   & =\sigma_{tension(max)}
\end{align}
$$

Because our calculated max load is lower than the given yield stress, the beam is adequate.
