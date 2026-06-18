Justification & Decision Record
UAV Fuselage Exterior (Shape, Profile, Geometry)

---

## Table of Contents

1. Design Requirements & Constraints
2. Alternatives Considered
3. Chosen Configuration — Justified
4. Nose Section: Power-Law Ogive (n = 0.75)
5. Cylindrical Midsection
6. Tail Taper: Cosine Profile
7. Fineness Ratio Selection
8. Cross-Sectional Shape: Circular
9. Dimensional Summary & Sanity Check
10. Known Trade-offs & Packaging Caution
11. Optimisations Considered
12. Glossary

---

## 1. Design Requirements & Constraints

|                        | Requirement                    | Source                      |
| ---------------------- | ------------------------------ | --------------------------- |
| Total fuselage length  | 900 mm                         | Packaging + tail moment arm |
| Tail-end socket radius | 15 mm                          | Tail boom diameter          |
| Avionics bay minimum   | 60 mm                          | FC + ESC + receiver         |
| Battery (est. 4S LiPo) | 100 mm length                  | Typical component size      |
| Wing spar penetration  | 80 mm deep                     | Structural requirement      |
| Total aircraft mass    | 8 kg MTOW                      | Mission requirement         |
| Speed regime           | Low subsonic (<30 m/s)         | UAV class                   |
| Drag priority          | Minimise parasite drag         | Efficiency / endurance      |
| Manufacturability      | Moderate complexity acceptable | Carbon + glass composite    |

The two most important constraints were **packaging** (fitting real hardware inside) and **aerodynamic drag** because these two goals often pull in opposite directions, so the trade-off between them was considered.

---

## 2. Alternatives Considered

Three main fuselage archetypes were assessed.

### 2.1 Frustum (Straight Taper)

Essentially a truncated cone, a body that tapers at a constant rate from front to back, without any curved profile.

**Pros:**

- Very simple to design and manufacture
- A lot of internal volume
- Easy to analyse structurally

**Cons:**

- Generates significantly more **pressure drag** than a curved body of the same length, because the air flow cannot smoothly follow the sharp angular taper, since it tends to separate from the surface (When air flows around a body, it can flow  smoothly as long as the surface curves _gently_. But if the surface suddenly changes angle, like at the corner of a frustum, the air can't make that sharp turn. Instead of following the surface, it just keeps going straight and **detaches** from it. This is called **flow separation**.
- The front of the body has high pressure (air being pushed out of the way), but now the back has very low pressure (the wake). That **pressure difference between front and back is what we call pressure drag** — it's literally the body being "sucked" backwards by its own wake.
- No continuous curvature at transitions means flow separation is likely at the nose and tail junctions
- Heavier for a given strength compared to circular cross-sections under bending load

Raymer (§4.2) recommends smooth bodies for all subsonic aircraft, this idea was rejected.

---

### 2.2 Pressure Tube (Cylinder with Short Nose + Tail Cones)

A pressure-tube fuselage uses a long constant-diameter cylinder with short nose and tail transitions bolted on. This is common on older general aviation aircraft.

Typical proportions (from Raymer's statistical data):

- Nose/forward section: 1.45–1.75 × fuselage diameter
- Tail/empennage section: 3.0–3.35 × fuselage diameter

**Pros:**

- Circular cross-section distributes internal pressure (and bending loads) very evenly, which is efficient structurally
- Large, usable internal volume in the cylindrical section
- Relatively easy to manufacture the constant-diameter section

**Cons:**

- Short nose means a _blunter_ profile, which creates a larger high-pressure stagnation region at the front → higher **form drag**
- Abrupt nose-to-cylinder transition is aerodynamically harsh
- The long cylindrical section generates significant **skin friction drag** because it exposes a lot of wetted (exposed-to-airflow) surface area at constant diameter

**Verdict: Partially adopted.** The cylindrical midsection concept was retained, but with a much longer and more refined nose and tail. Pure pressure-tube proportions were not used.

---

### 2.3 Tadpole / Streamlined Body of Revolution

A "tadpole" fuselage is a fully contoured shape — typically with a long, pointed nose, a maximum-width station at roughly 30–40% of the total length, and a long smooth taper to the tail. It is the aerodynamically ideal shape at subsonic speeds. The Currawong design uses a version of this.

**Pros:**

- Minimum **wave drag** and **form drag** for a given volume — the smooth curvature allows air to follow the surface without separating
- The gently sloping aft taper reduces **base drag** (the low-pressure wake behind the body)
- Slight nose-down pitch angle in flight reduces the angle of attack of the fuselage relative to the freestream, which reduces **interference drag**

**Cons:**

- More complex to design — requires explicit definition of the profile curves
- Harder and more expensive to manufacture than a simple cylinder
- Requires careful placement of the maximum-width station to balance packaging vs. aerodynamics

**Verdict: Adopted as the primary approach.** The extra design effort is justified by the drag reduction over the mission. All three fuselage sections (nose, cylinder, tail) were designed as smooth, contiguous curves.

---

## 3. Chosen Configuration — Justified

The final fuselage is a **three-section body of revolution** (i.e., a 3D shape formed by rotating a 2D profile around the centreline axis). It consists of:

1. **Power-law ogive nose** — smoothly accelerates airflow from zero at the tip to full fuselage diameter
2. **Short cylindrical midsection** — constant-diameter structural and packaging zone
3. **Cosine taper tail** — smoothly decelerates the flow and closes out to the tail boom socket

This is the same general philosophy as the Currawong fuselage and represents the standard approach for subsonic fixed-wing UAVs.

**Why a body of revolution?**

- Rotationally symmetric bodies are the most structurally efficient shape under bending loads (the dominant load case for a fuselage)
- They are straightforward to manufacture by filament winding or laying fibreglass over a male mould
- They avoid asymmetric aerodynamic forces that would create unwanted rolling or yawing moments
- surface angle changes _gradually_, so the air can keep following it all the way to the tail without separating. The wake is much smaller, so the front-to-back pressure difference is much smaller, so the drag is much lower.)

---

## 4. Nose Section: Power-Law Ogive (n = 0.75)

### What is a power-law ogive?

A power-law ogive is a nose shape defined by:

$R(x) = R_{\max} \cdot \left(\frac{x}{L_{\text{nose}}}\right)^n$

Where:

- $R(x)$ = the radius of the fuselage at position $x$ along the length
- $R_{\max}$ = maximum fuselage radius (80 mm)
- $L_{\text{nose}}$ = total nose section length (277.3 mm)
- $n$ = the _power exponent_ — the number that controls how quickly the nose "opens up"
- $x$ = distance along the nose, measured from the tip

In plain English: start at zero (the sharp tip), and the radius grows as a smooth, mathematically controlled curve until it reaches the full fuselage diameter.

### Why n = 0.75?

The exponent $n$ controls the "pointiness" of the nose:

- **n = 1.0** → perfectly conical nose (straight line — the bluntest option)
- **n = 0.75** → mild ogive — the nose opens up quickly near the tip, then flattens off (recommended for subsonic flow)
- **n = 0.5** → parabolic ogive — even blunter profile, used for very low-speed aircraft

For **subsonic UAVs**, $n = 0.75$ is the standard recommendation (Raymer §4.2, NACA technical notes on fuselage design). It produces the lowest pressure drag in the 10–40 m/s speed range by:

1. Avoiding a sudden blunt face at the nose tip that would create a large stagnation zone
2. Keeping the curvature change (second derivative of the profile) small, so the airflow does not accelerate too rapidly and then have to decelerate, which would promote **boundary layer separation**

### Nose section length — justified

The nose section runs from x = 0 mm to x = 277.3 mm, representing **30.8% of the total fuselage length**.

This was chosen based on Raymer's statistical guidelines, which suggest the nose region should occupy roughly 1.5–2.0 × the maximum fuselage diameter for a clean subsonic design:

- $1.5 \times 160 \text{ mm} = 240 \text{ mm}$
- $2.0 \times 160 \text{ mm} = 320 \text{ mm}$
- **Chosen: 277.3 mm** — falls comfortably within this range

A longer nose would reduce drag further but would eat into the cylindrical packaging zone. A shorter nose would reduce internal space requirements, but would increase the curvature rate of the nose profile, creating a more aggressive pressure gradient and higher drag. **277.3 mm is the optimal compromise.**

---

## 5. Cylindrical Midsection

### What is the cylindrical midsection?

The midsection is a constant-diameter (160 mm) section between x = 277.3 mm and x = 399.1 mm — a length of **121.8 mm**.

### Why include it at all?

A pure tapered body (nose going straight to tail taper) would have _no_ cylindrical section. However, a short cylindrical section is included for several practical reasons:

1. **Wing spar clearance:** The main wing spar must pass through the fuselage at this station. A constant-diameter section provides a clearly defined structural frame for the spar cutout without requiring the spar geometry to match a curved surface.
2. **Avionics packaging:** Flat bulkhead panels (for mounting avionics trays, battery holders, etc.) are easier to design and manufacture against flat circular frames than curved surfaces.
3. **Manufacturing datum:** The cylinder provides a stable reference surface for jig alignment during assembly.

### Drag penalty of the cylindrical section

A cylinder creates **skin friction drag** proportional to its wetted surface area. For the chosen diameter:

$A_{\text{wetted,cyl}} = \pi \times D \times L_{\text{cyl}} = \pi \times 0.16 \times 0.1218 \approx 0.0612 \text{ m}^2$

This is acceptable given the packaging benefits. Extending the cylinder unnecessarily would add wetted area with no aerodynamic benefit, so the **121.8 mm length is the minimum practical value** — it was chosen to satisfy packaging constraints rather than maximise performance.

> ⚠️ **Packaging note:** The spar penetration is ~80 mm deep, using 65.7% of the 121.8 mm cylindrical section. The remaining ~41.8 mm must fit part of the avionics or battery. This is tight. An extension of the cylinder to ~180 mm (by shifting the nose/tail junctions slightly) is recommended if packaging proves infeasible.

---

## 6. Tail Taper: Cosine Profile

### What is the cosine taper?

The tail section runs from x = 399.1 mm (R = 80 mm) to x = 900 mm (R = 15 mm). Rather than tapering in a straight line or using a power-law curve, a **cosine interpolation** was used:

$R(x) = R_{\text{tail}} + \frac{R_{\max} - R_{\text{tail}}}{2} \left(1 + \cos\left(\pi \cdot \frac{x - x_{\text{start}}}{L_{\text{tail}}}\right)\right)$

In plain English: the radius transitions smoothly from 80 mm to 15 mm following the shape of a half-cosine wave — starting and ending with a flat (zero slope) tangent.

### Why cosine rather than linear or power-law?

|Profile type|Slope at start of taper|Slope at tail end|Drag behaviour|
|---|---|---|---|
|Linear (straight)|Discontinuous jump in slope|Discontinuous jump|Flow separation at both ends — poor|
|Power-law|Smooth at start|Slope does not reach zero|Abrupt tail — moderate|
|Cosine|Zero slope (continuous)|Zero slope (continuous)|Smoothest possible transition — best|

The key advantage of the cosine profile is that the **slope is zero at both ends** of the taper. This means the tail profile meets both the cylindrical section and the tail-boom socket _tangentially_ — there is no sudden change in surface angle, so the airflow has the best chance of remaining attached to the surface all the way to the tail. Any kink or discontinuity in slope would create a **separation point** — a region where the airflow leaves the surface and creates a turbulent wake behind the body, significantly increasing drag.

### Tail section length — justified

The tail section spans 500.9 mm — **55.7% of the total fuselage length**.

A long tail taper is aerodynamically beneficial because it reduces the rate at which the cross-section shrinks. A rapidly closing tail forces the airflow to decelerate sharply, creating an **adverse pressure gradient** (pressure increasing rapidly in the downstream direction). When the adverse pressure gradient is too steep, the boundary layer — the thin layer of slow-moving air directly against the surface — cannot keep up with the pressure rise and separates, creating a large turbulent wake. The longer the tail, the more gently the pressure rises and the lower the wake drag.

For subsonic bodies, Hoerner's _Fluid Dynamic Drag_ recommends a tail closure half-angle of no more than ~10–12° for attached flow. The chosen tail geometry closes from 80 mm radius to 15 mm radius over 500.9 mm, giving an average half-angle of:

$\theta = \arctan\left(\frac{80 - 15}{500.9}\right) \approx 7.4°$

This is comfortably within the attached-flow regime. ✓

---

## 7. Fineness Ratio Selection

### What is fineness ratio?

The **fineness ratio** (FR) is the ratio of the total fuselage length to its maximum diameter:

$FR = \frac{L_{\text{fus}}}{D_{\text{fus}}} = \frac{900 \text{ mm}}{160 \text{ mm}} = \mathbf{5.625}$

### Why does fineness ratio matter?

Fineness ratio controls the balance between two competing drag components:

|FR too low (fat body)|FR too high (needle body)|
|---|---|
|Large frontal area → high **form drag**|Small frontal area → low form drag|
|Short body → low **skin friction drag**|Long body → high skin friction drag|

There is an optimal fineness ratio where the sum of form drag and skin friction drag is minimised. For subsonic aircraft at typical UAV speeds (10–40 m/s), this optimum lies between **FR = 3 and FR = 6** (Hoerner, 1965; Raymer, 2012).

The chosen FR of **5.625** falls comfortably within this optimal range, biased toward the upper end to:

1. Provide sufficient internal length for packaging all required components
2. Maximise the tail moment arm (important for pitch/yaw stability — a longer fuselage allows smaller, lighter tail surfaces)

An FR below ~4 would create unacceptably high form drag. An FR above ~7 would add excessive wetted area (skin friction) and structural mass without further drag reduction.

---

## 8. Cross-Sectional Shape: Circular

### Why circular cross-section?

The fuselage uses a **circular cross-section** throughout. Alternatives (elliptical, rectangular, teardrop) were briefly considered.

|Cross-section|Aerodynamic efficiency|Structural efficiency|Manufacturability|
|---|---|---|---|
|**Circular**|Excellent — symmetric, no preferred separation line|Excellent — most efficient shape for bending and internal pressure|Excellent — simple mould, filament wind, or tube|
|Elliptical|Slightly better in one axis if oriented correctly|Good — slightly less efficient than circle|Moderate — requires more complex mould|
|Rectangular|Poor — sharp corners cause flow separation|Poor — corners concentrate stress|Easy — flat panels|

For a body of revolution (spun symmetrically about its centreline), circular cross-section is the natural and optimal choice. There is no aerodynamic reason to deviate from this for a non-futuristic UAV design.

**Structural note:** A circular tube under bending (the dominant load case, with wings pulling upward and the fuselage weight acting downward) is the most structurally efficient shape because the **second moment of area** is maximised for a given perimeter (material used). This means you can use a thinner wall for the same bending stiffness compared to any other cross-section shape.

---

## 9. Dimensional Summary & Sanity Check

|Parameter|Value|Unit|Justification|
|---|---|---|---|
|Total length L\_fus|900|mm|Packaging + tail arm target|
|Max diameter D\_fus|160|mm|2 × 80 mm radius|
|Max radius R\_max|80|mm|Packaging constraint|
|Tail-end radius R\_tail|15|mm|Tail boom socket|
|Nose length L\_nose|277.3|mm|1.73 × D — within Raymer target range|
|Cylinder length L\_cyl|121.8|mm|Minimum for spar + avionics|
|Tail length L\_tail|500.9|mm|Long taper for attached flow|
|**Section sum**|**900.0**|**mm**|✓ Matches L\_fus|
|Nose power exponent n|0.75|—|Optimal for subsonic|
|**Fineness ratio FR**|**5.625**|—|✓ Within optimal range 3–6|
|Frontal area A\_ref|201.1|cm²|π × (80 mm)²|
|Tail half-angle|~7.4°|deg|✓ Below 10–12° separation limit|
|Profile method|Body of revolution|—|Rotated 2D curve → 3D solid|

---

## 10. Known Trade-offs & Packaging Caution

The biggest tension in this design is between **aerodynamic purity** (wanting a long, smooth taper with minimal cylindrical section) and **packaging practicality** (needing internal space for the spar, avionics, and battery).

The current cylindrical section of 121.8 mm is tight:

|Item requiring space in cyl. section|Estimated length|
|---|---|
|Wing spar penetration|~80 mm|
|Avionics tray (FC + ESC + RX)|~60 mm|
|Buffer / fastening clearance|~20 mm|
|**Total demand**|**~160 mm**|
|**Available**|**121.8 mm**|
|**Deficit**|**~38 mm** ⚠️|

**Proposed resolution:** Extend the cylindrical section to ~180 mm by shifting the nose/tail transitions:

- L\_nose: 277.3 → 260 mm (shorten slightly — small drag increase, acceptable)
- L\_cyl: 121.8 → 180 mm (resolve packaging deficit)
- L\_tail: 500.9 → 460 mm (shorten slightly — tail angle increases from 7.4° to ~8.2°, still within the attached-flow limit)

This is flagged as a recommended optimisation but has not yet been implemented in the CAD profile. The current profile (as generated in the `.pts` file) uses the original dimensions and remains aerodynamically sound.

---

## 11. Optimisations Considered

### 11.1 Profile Smoothness — Continuous Curvature

The three sections (nose, cylinder, tail) were designed so that:

- The nose profile **meets the cylinder tangentially** (slope = zero at x = 277.3 mm, since R'(L\_nose) = 0 from the power law)
- The cosine taper **meets the cylinder tangentially** (cosine slope = 0 at its start)
- The cosine taper **meets the tail socket tangentially** (cosine slope = 0 at its end)

This ensures **G1 continuity** (continuous first derivative / slope) at all junctions, meaning the airflow sees no sudden kinks in the surface. This is important for preventing flow separation at the transition points.

### 11.2 Avoiding Fineness Ratio Extremes

An earlier iteration considered a shorter fuselage (700 mm, FR = 4.375) to reduce skin friction. This was rejected because the shorter tail section would have required a steeper closure angle (~12°), pushing the design to the edge of the attached-flow regime and increasing the risk of tail separation at off-design angles of attack.

### 11.3 Alternative Nose Profiles Evaluated

|Nose type|Drag coefficient C\_D (relative)|Used?|
|---|---|---|
|Hemisphere|0.38|No — blunt, large stagnation zone|
|Cone (n=1.0)|~0.24|No — slope discontinuity at base|
|Ogive (n=0.75)|~0.09|**Yes — minimum drag for subsonic**|
|Parabola (n=0.5)|~0.12|No — slightly higher drag than n=0.75|
|Tangent ogive (circular arc)|~0.10|No — marginally worse than power-law at this fineness|

_C\_D values are approximate from Hoerner (1965) for bodies at subsonic speeds. They are for comparison only, not absolute values._

### 11.4 Aft-Fuselage Boattail Angle

A steeper boattail (tail closure) angle reduces the length and hence the skin friction of the tail section, but increases the risk of flow separation and base drag. The 7.4° average angle chosen is a deliberate choice to stay well inside the aerodynamic "safe zone" and guarantee attached flow even at small angles of attack.

---

## Glossary

**Adverse pressure gradient** A condition where air pressure increases in the direction of flow. Airflow moving against a rising pressure "wants" to slow down and reverse — if the gradient is too steep, the boundary layer separates from the surface and creates a wake. Avoiding sharp adverse pressure gradients is one of the central goals of fuselage aerodynamic design.

**Angle of attack (AoA)** The angle between the direction the aircraft is pointing and the actual direction of the airflow. When a fuselage is at a small positive angle of attack (nose slightly up), it generates some lift but also some additional drag.

**Base drag** The drag caused by the low-pressure region directly behind any blunt trailing surface. A tail that closes to a sharp point has zero base drag; a flat-ended fuselage (like a cut tube) has maximum base drag.

**Body of revolution** A 3D shape created by rotating a 2D profile (curve) around a central axis. A sphere, cone, and this fuselage are all bodies of revolution. They are always rotationally symmetric.

**Boundary layer** A very thin region of air immediately against any surface where the air speed transitions from zero (at the surface — the fluid "sticks" to the wall) to the full freestream speed. The boundary layer can either remain smoothly attached to the surface (laminar or turbulent but attached) or separate from the surface (separated), creating a large wake.

**Boattail** The aft (rear) section of a fuselage where it tapers down toward the tail. The name comes from the similar shape seen on the stern of wooden boats. A gradual boattail minimises base drag and wake.

**Cosine taper** A profile that follows the shape of a cosine function, ensuring the slope (rate of radius change) is zero at both ends of the transition. This gives the smoothest possible transition between two different diameters with no kinks.

**Drag** The force that opposes motion through air. For a fuselage, the main contributors are:

- _Form drag_ (pressure drag): caused by the high-pressure region in front and low-pressure wake behind
- _Skin friction drag_: caused by the air "rubbing" against the fuselage surface
- _Interference drag_: caused by interactions between different parts (wing–fuselage junction, tail–boom junction)

**Fineness ratio (FR)** The ratio of a body's total length to its maximum diameter: FR = L / D. An FR between 3 and 6 is optimal for minimising total drag on a subsonic fuselage.

**Form drag (pressure drag)** The component of drag caused by the pressure difference between the front (high pressure, air is pushed aside) and the rear (low pressure, wake) of the body. A streamlined body minimises this by allowing the flow to smoothly rejoin behind the body.

**G1 continuity** A mathematical term meaning that two curves or surfaces meet with the same slope (tangent direction) at their joining point. If two surface sections meet at a kink (different slopes either side), that is only G0 (position continuous but slope discontinuous), and it will cause flow separation at the kink.

**Interference drag** Extra drag generated at the junction between two parts (e.g., wing root meeting the fuselage) because the two separate airflows disturb each other. Smooth fillets at junctions reduce this.

**Ogive** A pointed, rounded nose shape. A "power-law ogive" defines the curvature mathematically using a power function, allowing the profile to be tuned via the exponent n.

**Parasite drag** All drag that exists regardless of whether the aircraft is producing lift. Includes form drag and skin friction drag. Distinct from induced drag (which only exists when lift is being generated).

**Power-law profile** A curve where one variable is proportional to another raised to a power: y = x^n. The exponent n controls the shape — higher n means more pointed/conical, lower n means more blunt/parabolic.

**Separation (flow separation)** When the boundary layer can no longer follow the surface and detaches from it, leaving a large turbulent wake. This dramatically increases drag. Separation is caused by adverse pressure gradients that are too steep.

**Skin friction drag** Drag caused by the viscosity (internal friction) of air "rubbing" against the fuselage surface. Proportional to the total wetted surface area. Turbulent boundary layers generate more skin friction than laminar ones, but are more resistant to separation.

**Stagnation point** The single point on the very front of a body where the airflow comes to a complete stop (velocity = 0). The pressure here is the highest anywhere on the body. For a circular nose, the stagnation point is at the very tip.

**Wetted area** The total surface area of the fuselage that is in contact with the airflow. Higher wetted area = more skin friction drag. Streamlined bodies try to minimise wetted area for a given internal volume.

---

_References: Raymer, D.P. (2012) Aircraft Design: A Conceptual Approach, 5th ed. AIAA. | Hoerner, S.F. (1965) Fluid-Dynamic Drag. | NACA Technical Notes on body-of-revolution drag._
