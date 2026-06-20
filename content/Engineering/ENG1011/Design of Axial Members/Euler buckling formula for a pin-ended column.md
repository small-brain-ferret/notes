Derived from the [[Euler-Bernoulli Beam Bending equation]].

> [!NOTE] Euler [[buckling]] formula for a pin-ended column
>
> $$
> \frac{d^2y}{dx^2}=\frac{M}{EI}=-\frac{Py}{EI}
> $$
>
> $$
> P_{cr}=\frac{\pi^2EI}{L^2}
> $$
>
> EI represents the [[bending stiffness]].
>
> y: sideways buckle displacement of the column
> E: [[Young's Modulus E|Modulus of Elasticity]]
> I: [[Second moment of Area (I)- moment of inertia]]
> P: axial load
> L: member length
> ![[Attachments/Screenshot 2026-06-20 at 07.42.51.png]]
>
> [[Dimensional homogeneity]]:
>
> $$
> [N]=\frac{[N]}{[L]^2} [L]^4 \frac{1}{[L]^2}
> $$
>
> 1 MPa = 1 $\frac{\text{N}}{{mm}^2}$

Assumptions when deriving this formula:

- column is initially perfectly straight
- its ends are assumed to be [[pinned support|pinned]]
- its cross-sectional area is uniform throughout its length
- self-weight is ignored
- applied load is concentrically applied
- material is homogeneous and [[isotropic]]
- shortening du to compression is negligible
- failure occurs due to buckling

# Example

A 2.25m long [[pinned support|pin]]-ended  solid steel circular column diameter 45mm is loaded in compression.
a) what's the buckle length?
b) what's the buckle length if it were twice as long?
Assume $E_{\text{steel}}=200000$ MPa, Yield strength $=250$ MPa, and $I=2.01\times 10^5$ mm$^4$.

###### a)

$$
P_{cr}=\frac{\pi^2EI}{L^2}=\frac{\pi^2\times200000*2.01*10^5}{(2250)^2}=78484\text{ N}
$$

###### b)

$$
P_{cr}=\frac{\pi^2EI}{L^2}=\frac{\pi^2\times200000*2.01*10^5}{(4500)^2}=19593\text{ N}
$$
