> [!NOTE] Thevenin equivalent
> The behaviour of any arbitrary linear circuit, with respect to a pair of open terminals can be represented with a Thevenin equivalent model with a **single ideal voltage source in series with a single resistor**.
>
> ![[Attachments/Pasted image 20260911204837.png]]

> [!NOTE] Finding $R_{Th}$ in circuit diagrams
> $R_{Th}$ can be found by killing the independent sources and finding the equivalent resistance seen between the terminals.
> ![[Attachments/Pasted image 20260911223530.png|300]]
>
> After killing the independent sources, the circuit is only left with resistors.
> ![[Attachments/Pasted image 20260911223548.png|300]]
>
> $$
> R_{Th} = (2 \text{ k}\Omega )||(3 \text{ k}\Omega )=1.2\text{ k}\Omega 
> $$

> [!NOTE] Finding the Thevenin equivalent - method 1
> a) and b) have the same load line. By connecting 2 separate values of load resistor and measuring the voltage ($V_L$) using an ideal voltmeter, we can find the equation of the load line:
>
> ![[Attachments/Pasted image 20260911220449.png]]
>
> $$
> V_{L}=\frac{R_{L}}{R_{Th}+R_{L}}V_{Th}
> $$
>
> As we take the measurements for two different values of $R_{L}$, we get:
>
> $$
> \begin{align}
> V_{L_{1}} & =\frac{R_{L_{1}}}{R_{Th}+R_{L_{1}}}V_{Th} \\ \\
>
> V_{L_{2}} & =\frac{R_{L_{2}}}{R_{Th}+R_{L_{2}}}V_{Th}
> \end{align}
> $$
>
> Solving these simultaneously gives $V_{Th}$ and $R_{Th}$.
>
> Alternatively, we can measure the current $I_{L}$ in addition to the measurements of $V_{L}$. In that case we express the loop equation as:
>
> $$
> V_{L}=V_{Th}-R_{Th}I_{L}
> $$
>
> For 2 different values of the load resistor:
>
> $$
> \begin{align}
> V_{L_{1}} & =V_{Th}-R_{Th}I_{L_{1}} \\ \\
>
> V_{L_{2}} & =V_{Th}-R_{Th}I_{L_{2}}
> \end{align}
> $$
>
> Solving these simultaneously gives $V_{Th}$ and $R_{Th}$.

> [!NOTE] Finding the Thevenin equivalent - method 2
>
> Step 1: Leave terminals open and measure $V_{OC}$, as $V_{Th}=V_{OC}$
> Step 2: Short the terminals and measure $I_{SC}$
> Step 3: Calculate $R_{Th}=\frac{V_{OC}}{I_{SC}}$
>
> Derivation:
> The open circuit voltage ($V_{OC}$) and the short circuit current ($I_{SC}$) are the intersections of the straight line with $V_{L_{1}}  =V_{Th}-R_{Th}I_{L_{1}}$ with the horizontal axis and the vertical axis respectively.
>
> When we measure the open circuit voltage, $I_L=0$, so $V_{Th}=V_{OC}$.
>
> ![[Attachments/Pasted image 20260911220632.png]]
>
> When we measure the short circuit current, $V_L=0$ and
>
> $$
> \begin{align}
> I_{SC} & =\frac{V_{Th}}{R_{Th}} \\ \\
>
> R_{Th} & =\frac{V_{Th}}{I_{SC}}
> \end{align}
> $$

> [!NOTE] Ideal Meter Assumptions
> If the voltmeter has very high internal resistance (approaching an ideal meter), the voltage it measures when connected directly across the open terminals approximates the open-circuit voltage.
>
> If the ammeter has very low internal resistance (approaching an ideal meter), the current it measures when connected directly across the open terminals approximates the short-circuit current.

> [!NOTE] Limitations of Short-Circuit Current Measurement
> However, measuring the short-circuit current may not be practical always.
> For example:
>
> - a system may have over-current protection circuitry that prevents large short-circuit currents from flowing.

In addition:

> - the device or the measuring instrument may be damaged due to the large current.
