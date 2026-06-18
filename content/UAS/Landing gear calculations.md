# Design constraints review

MTOW: 8kg
Box size: 0.9 x 0.5 x 0.5
cruise speed: 25m/s
min stall speed: 13m/s
non-structural mass: 2.5kg

# Deriving the force the gear must survive

When UAV hits ground, theres a downward velocity which gets stopped very suddenly, which creates a force spike much larger than the aircraft's weight.

To find the total landing load, we use:

$$
F_{total}=n*W
$$

Where $n$ is the design load factor. The standard design load factor for a light UAV at the point of touchdown is 3.5$g$, so, with an MTOW of 8kg:

$$
F_{total}=3.5\cdot 8 \ \cdot 9.81 = 274.4\text{N}
$$

For a configuration with 3 wheels, the main two rear gears should carry around 90% of the load, so:

$F_{rear} = 0.9 \times 274.7 \approx 247 \text{ N total, split between two legs}$

$F_{per\ leg} = \frac{247}{2} \approx 124 \text{ N per main gear leg}$

The front gear carries the remaining **10%**:

$F_{front} = 0.1 \times 274.7 \approx 27.5 \text{ N (braking load, acts horizontally)}$

These are the **limit loads**. Applying a safety factor of **1.5**:

$F_{ultimate} = 1.5 \times F_{limit}$

| Location                 | Limit load | Ultimate load |
| ------------------------ | ---------- | ------------- |
| Each rear leg (vertical) | 124 N      | 186 N         |
| front gear               | 28 N       | 42 N          |

FEA should be run on these numbers.
