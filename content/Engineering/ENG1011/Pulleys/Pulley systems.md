---
publish: true
aliases:
  - pulley system
  - pulley systems
created: 2026-06-16T16:17:41.726+10:00
modified: 2026-06-16T18:22:14.025+10:00
---

A pulley system is a mechanical device that uses a wheel with a grooved rim and a rope or [[cable]] to transmit force and motion.

The wheel is called a [[pulley]] which can be fixed or moveable.

A pulley system is typically designed to make the work _feel_ easier by changing the direction and/or magnitude of the input force required to achieve the output force.

![[Attachments/Screenshot 2026-06-16 at 16.24.19.png]]

Image 1: Input force = Load
Image 2: Input force < Load

This can be described by the system's [[mechanical advantage]].

# FBDs of pulley systems

[[Free-body diagrams|FBDs]] can be used to analyse the forces in the components of pulley systems.
![[Attachments/Screenshot 2026-06-16 at 16.42.21.png]]

## Example - crate and pulley B

Forces:

- weight of the crate (mg)
- tension force ($T_1$) in the cable connected to pulley B
  ![[Attachments/Screenshot 2026-06-16 at 16.42.53.png]]

$T_1$ is shown twice because the boundary cuts through the cable twice, which exposes 2 tension forces.

## Example - crate, pulleys B and C

![[Attachments/Screenshot 2026-06-16 at 16.44.09.png]]

## Example - pulley D and top pulley

![[Attachments/Screenshot 2026-06-16 at 16.44.41.png]]

# Example question

Determine the force $F$ required to keep block $A$ stationary if it weighs 50 kg.

Also, calculate the [[mechanical advantage]] in this system and the distance the [[cable]] needs to be pulled down to raise block $A$ by 1 m. Assume $g=9.8$ m/s$^2$.

![[Attachments/Screenshot 2026-06-16 at 16.46.44.png]]

##### Step 1: Draw and analyse an FBD of the block and forces directly acting on it.

![[Attachments/Screenshot 2026-06-16 at 16.48.28.png]]

#### Step 2: Draw and analyse an FBD of the hand.

![[Attachments/Screenshot 2026-06-16 at 16.50.07.png]]

##### Step 3: calculate MA

$$
\begin{align}
\text{MA} & =\frac{F_{\text{load}}}{F_{\text{input}}} \\
 & =\frac{mg}{F} \\
  & =\frac{50(9.8)}{122.5} \\
   & =4
\end{align}
$$

##### Step 4: Use the MA to find $d_{\text{input}}$

$$
\begin{align}
\text{MA} & =\frac{d_{\text{load}}}{d_{\text{input}}} \\
 d_{\text{input}} & =MA(d_{\text{output}}) \\
  & =4(1) \\
   & = 4\text{ m}
\end{align}
$$

This means that to raise the block up by 1m, we need to pull the cable down by 4m.

# Example - applying the problem solving procedure

The pulley system below needs to support a 100kg load in equilibrium. Four motors are available with a pulling force of 100N, 200N, 300N, and 400N.

The cost of the motors increase with increased pulling force capacity. Determine the cheapest motor that would service this pulley system. Assume $g=9.8$ m/s$^2$.

##### Step 1: Establish objectives, constraints

- Pulley system arrangement is fixed
- Determine the cheapest motor for the pulley system
- Determine the tension force in the cable at point A

##### Step 2: Specify system boundaries, assumptions

- Entire system will be in equillbrium
- Assumptions:
  - Cables are in tension
  - tension forces in each cable is uniform
  - pulleys and cables have no weight
  - weight of the crate acts at the centre of gravity

##### Step 3: Establish the model

- FBDs: various
- equilibrium: $\sum F=ma=0$
- variables: $T_{1}$, $T_2$, $T_3$, $W_{\text{crate}}=mg$

##### Step 4: Analysis/design

![[Attachments/Screenshot 2026-06-16 at 17.07.30.png|187]]

$$
\begin{align}
\sum F_{y} & =0 \\
2T_{1}-mg & =0 \\ \\
T_{1} & =\frac{mg}{2} \\
 & =\frac{100(9.8)}{2} \\
  & =490\text{ N}
\end{align}
$$

![[Attachments/Screenshot 2026-06-16 at 17.09.33.png|186]]

$$
\begin{align}
\sum F_{y} & =0 \\
2T_{2}-T_{1} & =0 \\ \\
T_{2} & =\frac{T_{1}}{2} \\
 & =\frac{490}{2} \\
  & =245\text{ N}
\end{align}
$$

![[Attachments/Screenshot 2026-06-16 at 17.10.56.png]]

$$
\begin{align}
\sum F_{y} & =0 \\
2T_{3}-T_{2} & =0 \\ \\
T_{3} & =\frac{T_{2}}{2} \\
 & =\frac{245}{2} \\
  & =122.5\text{ N}
\end{align}
$$

![[Attachments/Screenshot 2026-06-16 at 17.12.03.png|238]]

$$
\begin{align}
\sum F_{y} & =0 \\
T_{3}-F & =0 \\
F & =122.5N
\end{align}
$$

##### Step 5: Behaviour satisfactory?

- cable forces are positive (indicating tension as per force direction assumption)
- successive halving of tension in cables
- magnitude of cable forces are as expected
- suitable motor exists to handle F

##### Step 6: complete

200N motor should be purchased to fulfil requirements.
An additional pulley could be used to decrease the tension, which would allow the purchase of the 100N motor.

# Example

![[Attachments/Screenshot 2026-06-16 at 17.29.39.png]]
![[Attachments/Screenshot 2026-06-16 at 17.30.36.png]]
Consider the pulley system above. A freight elevator is lifted using a pulley system and a motor. If the elevator and cargo weigh a combined total of 1000 kg, then determine the required tension in the cable connected to the motor to keep it in equilibrium. Also, determine the tension in the cable connected to the pulley fixed to the ceiling.

##### Step 1: draw a FBD of the desired system

![[Attachments/Screenshot 2026-06-16 at 17.33.39.png]]![[Attachments/Screenshot 2026-06-16 at 17.33.50.png]]

##### Step 2: Use equilibrium equations to solve for unknown forces

$$
\begin{align}
\sum F_{y} & =0 \\
3T_{1}-mg & =0 \\
T_{1} & =\frac{mg}{3} \\
T_{1} & =3266.6667 \text{ N}
\end{align}
$$

![[Attachments/Screenshot 2026-06-16 at 18.21.13.png]]

$$
\begin{align}
\sum F_{y} & =0 \\
T_{2}-2T_{1} & =0 \\
T_{2} & =2T_{1} \\
T_{2} & =6533.3333\text{ N}
\end{align}
$$
