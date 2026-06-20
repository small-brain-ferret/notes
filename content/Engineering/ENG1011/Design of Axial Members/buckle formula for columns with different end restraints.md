---
publish: true
aliases:
  - critical buckle load
created: 2026-06-20T13:48:20.712+10:00
modified: 2026-06-20T14:27:10.844+10:00
---

Derived from the [[Euler-Bernoulli Beam Bending equation]], and similar to the [[Euler buckling formula for a pin-ended column]]:

$$
P_{cr}=\frac{\pi^2EI}{(kL)^2}=\frac{\pi^2EI}{{L_{e}}^2}
$$

where $L_e$ is the effective length of the member, also equal to kL, where k is the effective length factor. It is the distance between points of zero moment, or the distance over which you get a $\frac{1}{2}$ sine curve.

![[Attachments/Screenshot 2026-06-20 at 13.49.58.png]]

# Example

A 2.25m long solid steel circular column of diameter 45mm is loaded in compression. End B of the column is now rigidly connected to a support (i.e. not free to rotate). What is the column buckle strength?
Assume $E_{\text{steel}}=200000$ MPa, yield strength = 250 MPa, and $I_{\text{section}}=2.01\times10^5$ mm$^4$

$$
P_{cr}=\frac{\pi^2EI}{(kL)^2}=\frac{\pi^2\times200000*2.01*10^5}{(0.7\times2250)^2}=159942\text{ N}
$$
