The diode's I-V relation is nonlinear.
![[Attachments/Pasted image 20260911165743.png|392]]

We need 2 equations to find the values of 2 unknown variables:

$$
\begin{align}
I_{d} & =\frac{V_{S}-V_{d}}{R_{S}} \\
I_{d} & =f(V_{d})
\end{align}
$$

The second equations is a nonlinear (exponential) function.
The I-V characteristics of the curve of the diode (2nd equation) is provided by the manufacturer. If we plot the graph of the first equation, then the point of intersection of the 2 graphs gives the solution.

Rewrite the first equation to express $I_{d}$ as the DV of the IV $V_d$ .

$$
I_{d}=-\frac{1}{R_{S}}V_{d}+\frac{V_{S}}{R_{S}}
$$

This is the [[load line]].

![[Attachments/Pasted image 20260911203355.png|408]]

## Load Line vs Diode I-V Curve

### Load Line

$I_d = \frac{V_s - V_d}{R_s}$

- Describes the **external circuit** - Depends on (V\_s) and (R\_s) - Is a **straight line**

### Diode I-V Characteristic

$I_d = f(V_d)$

- Describes the **diode itself** - Usually nonlinear - Determined by the diode's physical characteristics
