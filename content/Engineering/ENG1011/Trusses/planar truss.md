---
publish: true
aliases:
  - planar trusses
  - truss
  - trusses
created: 2026-06-17T15:55:54.497+10:00
modified: 2026-06-22T09:24:19.013+10:00
---

> [!NOTE]
> A truss is a structure composed of members joined together at their endpoints.
>
> They are typically made out of wooden [[strut|struts]] or metal bars.
>
> Planar trusses are those that lie on a single plane and are often used to support structures such as bridges.
>
> ![[Engineering/ENG1011/Trusses/images/Screenshot 2026-04-16 at 08.05.08.png]]

## Truss types

![[Engineering/ENG1011/Trusses/images/Screenshot 2026-04-16 at 08.05.50.png]]
Different truss types exist because they are designed to withstand different load types and stresses.

## Truss assumptions

Truss members are [[two-force members]] (undergo tension or compression) because:

- all loadings are applied at the joints
- members are joined together by pins

* Weight of members is generally negligible.
* Trusses generally have [[pinned support|pinned supports]] and [[roller support|roller supports]]
* [[roller supports]] and rockers are used to allow extension under temperature changes.
  ![[Engineering/ENG1011/Trusses/images/Screenshot 2026-04-16 at 08.10.40.png]]

## Truss determinacy

The truss' determinacy can be evaluated by counting the number of two-force members ($m$), the number of joints ($j$), and the number of reactions ($r$).

- A statically determinate truss obeys $m+r=2j$
- A statically indeterminate truss will follow $m+r>2j$ (Excess members or reactions)
- Check stability. If stable, check determinacy.
  ![[Engineering/ENG1011/Trusses/images/Screenshot 2026-04-16 at 08.12.40.png]]

![[Engineering/ENG1011/Trusses/images/Screenshot 2026-04-16 at 08.13.21.png]]
![[Engineering/ENG1011/Trusses/images/Screenshot 2026-04-16 at 08.14.05.png]]

## Example - Reactions

The reactions of a truss can be calculated by drawing a free-body diagram of the truss and replacing the supports with its reactions.

In this example, there is a pin support at point A and a roller support at point C.![[Engineering/ENG1011/Trusses/images/Screenshot 2026-04-16 at 08.15.09.png]]

From this point, we can apply our equilibrium equations:
Forces in x-axis:

$$
\begin{align}
\sum F_{x} & =0 \\
-A_{x}+3 & =0 \\
A_{x} & =3\text{ kN}
\end{align}
$$

Resultant moment at A:

$$
\begin{align}
\sum M_{A} & =0 \\
C_{y}(4)-3(2) & =0 \\
C_{y} & =1.5\text{ kN}
\end{align}
$$

Forces in y-axis:

$$
\begin{align}
\sum F_{y} & =0 \\
-A_{y}+C_{y} & =0 \\
A_{y} & =1.5\text{ kN}
\end{align}
$$

## Example - Reactions

![[Engineering/ENG1011/Trusses/images/Screenshot 2026-04-16 at 08.20.42.png]]

Forces in the x-axis:

$$
\begin{align}
\sum F_{x} & =0 \\
600-C_{x} & =0 \\
C_{x} & =600\text{ N}
\end{align}
$$

Resultant moment at C:

$$
\begin{align}
\sum M_{C} & =0 \\
-A_{y}(6)+400(3)+600(4) & =0 \\
A_{y} & =600\text{ N}
\end{align}
$$

Forces in the y-axis:

$$
\begin{align}
\sum F_{y} & =0 \\
A_{y}-400-C_{y} & =0 \\
C_{y} & =200\text{ N}
\end{align}
$$
