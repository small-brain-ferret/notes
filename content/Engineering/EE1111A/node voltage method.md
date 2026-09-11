a [[circuit analysis methods|circuit analysis method]].

> [!NOTE] node voltage method uses [[Kirchoff's current law|KCL]] only
>
> - Unknown variables are [[node voltage|node voltages]]
> - equations are found applying KCL
> - thus branch currents must be expressed using node voltages
>
> $$
> I_{R}=\frac{V_{x}-V_{y}}{R}
> $$
>
> Where $V_x$ is the node voltage at the tail of [[current]] arrow, $V_y$ is at the tip of the current arrow.
>
> Write KCL equations only at nodes where node voltages are not known.
>
> # KCL equations = # unknown node voltages

> [!NOTE] Steps for node voltage analysis
> Step 1: Choose a reference node or ground (where node voltage is 0)
>
> - negative terminal is usually set as this ref node.
>
> Step 2: Label all node voltages (NV), and determine number of unknown NV
>
> Step 3: Apply KCL at nodes whose NV is not known
>
> Step 4: Express the current in each resistor in terms of the adjacent NVs using Ohm's law ($I_{R}=\frac{V_{x}-V_{y}}{R}$)
>
> Step 5: Solve linear equations to find unknown NVs
>
> Step 6: Find branch currents using node voltages and resistor values.

# Worked Example

Step 1: Choose a reference node or ground (where node voltage is 0)

Step 2: Label all node voltages (NV), and determine number of unknown NV
![[Attachments/Pasted image 20260911140350.png]]
Step 3: Apply KCL at nodes whose NV is not known

$$
\begin{align}
V_{a} & =10\text{ V} \\
V_{c} & =15\text{ V}
\end{align}
$$

These voltages are the terminal voltages of the voltages sources. Thus, they are known. $V_b$ is unknown, thus, applying KCL around $V_b$ :

$$
I_{1}+I_{2}-I_{3}=0
$$

Step 4: Express the current in each resistor in terms of the adjacent NVs using Ohm's law ($I_{R}=\frac{V_{x}-V_{y}}{R}$)

$$
\begin{align}
\frac{V_a - V_b}{10} + \frac{V_c - V_b}{10} - \frac{V_b - 0}{10} = 0 \\ \\
\frac{10 - V_b}{10} + \frac{15 - V_b}{10} - \frac{V_b - 0}{10} = 0
\end{align}
$$

Step 5: Solve linear equations to find unknown NVs

$$
V_{b}=\frac{25}{3} \text{ V}
$$

Step 6: Find branch currents using node voltages and resistor values.

$$
\begin{align}

I_{1} & = \frac{V_a - V_b}{10}
     & = \frac{10 - \frac{25}{3}}{10}
	  & = \frac{1}{6} \text{ A} \\ \\

I_{2} & = \frac{V_b - 0}{10}
      &   = \frac{\frac{25}{3} - 0}{10}
      &   = \frac{5}{6} \text{ A} \\ \\

I_{3} & = \frac{V_b - V_c}{10}
     &    = \frac{\frac{25}{3} - 15}{10}
      &   = -\frac{2}{3} \text{ A}

\end{align}
$$
