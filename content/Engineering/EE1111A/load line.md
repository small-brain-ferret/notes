> [!NOTE]
> A **load line** shows all possible combinations of element voltage ($V$) and element current ($I$) allowed by the **rest of the circuit**.

For a simple diode-resistor circuit:

$$
V_s = I_d R_s + V_d
$$

Rearrange:

$$
I_d = \frac{V_s - V_d}{R_s}
$$

or

$$
\boxed{I_d = -\frac{1}{R_s}V_d + \frac{V_s}{R_s}}
$$

This is in the form:

$$
y = mx + c
$$

where:

$$
\boxed{m = -\frac{1}{R_s}}
$$

and

$$
\boxed{c = \frac{V_s}{R_s}}
$$

---

## How to Draw the Load Line

### 1. Find the $I_d$-axis intercept

$$
\boxed{\left(0,\frac{V_s}{R_s}\right)}
$$

### 2. Find the ($V_d$)-axis intercept

$$
\boxed{(V_s,0)}
$$

### 3. Connect the two points

The straight line between these two points is the **load line**.

## Effect of Changing ($V_s$)

If (V\_s) increases:

$$
V_s \uparrow
$$

then:

$$
\frac{V_s}{R_s} \uparrow
$$

Both intercepts increase.
The load line shifts outward, but the slope remains:

$$
-\frac{1}{R_s}
$$

> [!note]
> Changing ($V_s$) changes the intercepts, but not the slope.

---

## Effect of Changing (R\_s)

The slope is:

$$
m = -\frac{1}{R_s}
$$

Therefore:

- Larger ($R_s$) → flatter load line
- Smaller ($R_s$) → steeper load line

Also:

$$
I_{\max} = \frac{V_s}{R_s}
$$

So increasing ($R_s$) decreases the maximum possible current.

---

---

## Quick Formula Summary

$$
V_s = I_dR_s + V_d
$$

$$
I_d = \frac{V_s - V_d}{R_s}
$$

$$
I_d = -\frac{1}{R_s}V_d + \frac{V_s}{R_s}
$$

$$
\text{slope} = -\frac{1}{R_s}
$$

$$
I_d\text{-intercept} = \frac{V_s}{R_s}
$$

$$
V_d\text{-intercept} = V_s
$$
