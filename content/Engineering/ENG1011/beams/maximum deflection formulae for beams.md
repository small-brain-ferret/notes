> [!NOTE] maximum [[deflections]] formulae for [[beam]]
> ![[Attachments/Screenshot 2026-06-21 at 15.13.31.png]]

# Example - man on bridge

Loading = 100kg man at midspan
Assume bridge to be weightless
$E_{timber}=10000$ MPa
![[Attachments/Screenshot 2026-06-21 at 15.15.20.png]]
Calculate the [[deflections|deflection]] of the bridge at mid-span and check if it meets the [[Serviceability Limit State]] requirements (deflection < span/250).

##### Step 1: Decide what units to work with

$$
\begin{align}
P & =100\text{kg}=1000\text{N} \\
L & =4000\text{mm} \\
E & =10000\text{MPa}
\end{align}
$$

##### Step 2: calculate the [[Second moment of Area (I)- moment of inertia]]

$$
\begin{align}
I & =\frac{bd^3}{12}  \\
 & = \frac{{200 \times 40^3}}{12} \\
  & =1.067 \times 10^6 \text{mm}^4
\end{align}
$$

##### Step 3: Calculate $y_{\text{max}}$  using appropriate [[maximum deflection formulae for beams]]

$$
\begin{align}
y_{\text{max}} & =-\frac{PL^3}{48EI} \\
 & =\frac{{-1000(4000)^3}}{48\times 10000 \times 1.067 \times 10^6} \\
  & =125\text{ mm}
\end{align}
$$

##### Step 4: do a [[serviceability limit design]]

Maximum deflection = 125mm with full live load.
With [[Serviceability Limit State]] (SLS) loading = DL + 0.7LL, deflection = 87.5mm
allowable deflection = span/250= 4000/250 = 16mm
Thus, the bridge fails [[Serviceability Limit State]] as it deflects too much.
Recommendation is to increase plank size.
