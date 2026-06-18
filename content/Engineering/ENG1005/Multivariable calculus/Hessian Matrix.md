An important tool for [[Characterising critical points]]. See [[Use of the Hessian in characterising Critical points]].

The second directional derivative can be written in matrix form using the Hessian matrix.

Starting from:

$$
\frac{dF}{du} = \hat{u} \cdot \nabla f
$$

the second directional derivative is:

$$
\frac{d^2F}{du^2}
=
\frac{d}{du}\left( \frac{dF}{du} \right)
=
\hat{u} \cdot \nabla\left(\hat{u} \cdot \nabla f\right)
$$

This simplifies to:

$$
\frac{d^2F}{du^2}
=
\hat{u}^T H \hat{u}
$$

where $H$ is the Hessian matrix:

$$
H =
\begin{pmatrix}
\frac{\partial^2 f}{\partial x^2} &
\frac{\partial^2 f}{\partial x \partial y}
\\
\frac{\partial^2 f}{\partial y \partial x} &
\frac{\partial^2 f}{\partial y^2}
\end{pmatrix}
$$
