> [!NOTE] Definition
> The [[Composite trapezoidal rule]] for uniform segments of width $h$ extends the approach by subdividing the integrand into multiple segments of equal width, $h$.

> [!NOTE] Generalised formula
>
> $$
> \begin{align}
> I & =\frac{h}{2}[f(x_{1})+2f(x_{2})+2f(x_{3})+\dots+2f(x_{n-1})+f(x_{n})] \\
> & =\frac{h}{2}\left[ f(x_{1})+2\left( \sum_{i=2}^{n-1} f(x_{i}) \right) +f(x_{n})\right]
> \end{align}
> $$

![[Attachments/Screenshot 2026-05-28 at 14.16.39.png|319]]

# Pseudocode

![[Attachments/Screenshot 2026-05-28 at 14.22.34.png]]

# Example - 2 segments

These two segments will share a vertex at ($\frac{a+b}{2}$, $f(\frac{a+b}{2})$).

![[Attachments/Screenshot 2026-05-28 at 14.11.23.png|210]]

Since there are 2 segments, the width, $h$, of each segment is $h=\frac{{b-a}}{2}$.

Area of the first segment:

$$
I_{1}=\frac{h}{2} [f(a)+f(a+h)]
$$

Area of second segment:

$$
I_{2}=\frac{h}{2} [f(a+h)+f(b)]
$$

Estimate for integral is the sum of the two segments:

$$
\begin{align}
I & =I_{1}+I_{2} \\
 & =\frac{h}{2}[f(a)+2f(a+h)+f(b)]
\end{align}
$$
