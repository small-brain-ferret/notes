A [[Method of joints|method of joints]] analysis of a [[planar truss|truss]] structure yields the internal member force values shown.

a) Choose the most weight-efficient member sizes for all three members based on a [[design for axial tension strength|design for axial tension strength]]. Choose sections from [[CHS]] (circular hollow section tables) based on a minimum strength [[Factor of safety|factor of safety]] of 2.

b) Which member will cause [[design for axial tension strength|limit state strength]] failure of the system if the load increases further, so what will be the overall failure mode of the system?

c) Based on your chosen member sizes, calculate the true horizontal movement at B.

![[Attachments/Screenshot 2026-06-20 at 15.56.28.png]]

##### Step 1: Establish objectives, constraints.

- Determine the lightest weight members from the [[CHS]] ($\sigma_{y}=250$MPa, $E=200000$MPa)
- undertake [[design for axial tension strength]]
- define the limiting member in the system and its failure mode

##### Step 2: Specify system boundaries, assumptions

- system must remain within elastic range
- both [[yielding]] and [[buckling]] must be considered
- apply a [[Factor of safety|FoS]] of 2
- assume axial forces in each member are uniform
- ignore self weight of structure
- only consider in-plane member failure
- assume all member joints are [[pinned support|pins]]
- assume overall system failure is a result of member failure by yield or buckling

##### Step 3: Establish the model

- for [[design for axial tension strength|tension]]: $P_{\text{max}}\leq \sigma _y A$
- for [[Euler buckling formula for a pin-ended column|compression]]: $P=\sigma _y A$ and $P_{b}=\frac{\pi^2EI}{(L_{e})^2}$
- deflection at B using trig and [[serviceability limit design]] equation $\Delta L=\frac{PL}{AE}$

#### Analysis for tension members AB and AC ($\text{F}_{\text{AB}}=\text{F}_{\text{AC}}=150\text{ kN}$)

$$
\begin{align}
P & =FS\times 150=300\text{ kN} \\
\frac{P}{A} & \leq \sigma_{y} \\
\to A_{\text{req}} & \geq \frac{P}{\sigma_{y}}=\frac{300000}{250}=1200\text{ mm}^2
\end{align}
$$

Look in [[CHS]] for a member with a minimal cross-sectional area above $A_{req}$ to maximise weight efficiency.
Choose: 101.6 $\times$ 4 CHS (A = 1230 mm$^2$)
Actual FS = $\frac{\text{capacity}}{\text{actual load}}=\frac{250+1230}{150}=2.05$

#### Analysis for compression member BC ($\text{F}_{\text{BC}}=212.1\text{ kN}$)

$$
\begin{align}
P & =FS*212.1=424.2\text{ kN} \\

\end{align}
$$

Yield check:

$$
\begin{align}
\frac{P}{A} & \leq \sigma_{y} \\
\to A_{\text{req}} & \geq \frac{P}{\sigma_{y}}=\frac{424.2\times10^3}{250}=1696.8\text{ mm}^2
\end{align}
$$

Look in [[CHS]] for a member with a minimal cross-sectional area above $A_{req}$ to maximise weight efficiency.
Choose: 114.3 $\times$ 5.4 CHS (A = 1850 mm$^2$, I = 2.75$\times$ 10$^6$ mm$^4$, w=14.5 kg/m)
FOS yield = $\frac{\text{member capacity load}}{\text{actual load}}=\frac{250\times2120}{212.1\times 10^3}=2.499$

Buckling check:

$$
\begin{align}
P & =\frac{\pi^2EI}{{L_{e}}^2}\geq 424.2\times10^3 \\
I_{req} & =\frac{{424.2\times 10^3\times(4242.64)^2}}{\pi^2\times_{200000}}=3.87\times 10^6\text{ mm}
\end{align}
$$

Look in [[CHS]] for a member with a minimal [[Second moment of Area (I)- moment of inertia]] above $I_{req}$ to maximise weight efficiency.
Choose: 114.3 $\times$ 5.4 CHS (A = 1850 mm$^2$, I = 2.75$\times$ 10$^6$ mm$^4$, w=14.5 kg/m)
Choose: 139.7 $\times$ 5 CHS ($A=2120$mm$^2$, $I=4.8\times 10^6$, $w=16.6$kg/m)
FOS buckling = $\frac{\text{member capacity load}}{\text{actual load}}=\frac{\frac{\pi^2 E\times4.8\times 10^6}{(4242.64)^2}}{212.5\times 10^3}=2.485$

Now we have two to choose from. The one we choose needs to validate the requirements for both checks, thus the bigger and stiffer one out of the two, so the one from the buckling check.

##### Compare factors of safety to determine what will be the failure mode of the truss system

Since the SF for tension members AB and AC = 2.05 is less than the minimum SF for compression member CB = 2.485, the failure will be due to the tension members AB and BC, thus failure mode will be [[yielding]].

##### Finally, calculate actual horizontal movement at joint B

![[Attachments/Screenshot 2026-06-20 at 16.32.44.png]]

##### In conclusion

a) member sizes chosen are as shown![[Attachments/Screenshot 2026-06-20 at 16.33.32.png]]
b) the critical members that would fail first if load was increased are AB and AC that would yield
