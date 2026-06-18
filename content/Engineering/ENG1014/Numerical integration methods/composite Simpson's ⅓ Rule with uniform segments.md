> [!NOTE] Definition
> An application of the [[Simpson's ⅓ Rule]].
>
> For uniform segments of width $h$ and $n$ points is:
>
> $$
> I = \frac{h}{3} \left[ 
> f(x_{1})+4\left( \sum _{i=2}^{n-1} f(x_{i}) \right)
> + 2 \left( \sum _{j=3}^{n-2} f(x_{j}) \right)
> + f(x_{n})
>  \right]
> $$
>
> Where $i$ is even, $j$ is odd.
>
> This approach will only work with an odd number of points - thus an even number of segments.

The number of valid points for Simpson's 1/3rd rule starts at a minimum of 3 points, and increments by 2 for each new application.

Some conditions apply:

- to fit a parabola, three points are needed
  - the smallest number of points for this method to work is three, or a minimum of two segments or equal width
- The point between any two neighbouring parabolas is shared between them
  - thus, number of points with increasing number of parabolas is 3, 5, 7, ...

# Pseudocode

![[Attachments/Screenshot 2026-05-29 at 01.04.41.png]]
