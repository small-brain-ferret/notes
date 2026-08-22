See [[Partial derivatives]].
These tell us information about [[The gradient - nabla f]] of a slice of a MVF in a specified direction.

> [!NOTE] Directional Derivative
> The slope of a function $f(x,y)$ in the direction of a unit vector $\hat{u}$ at a point $x=x_0$ is called the **directional derivative**.
>
> $$
> \begin{align}
> \frac{\partial f}{\partial u} & =\mathbf{\hat{u}}\cdot\nabla f\Big|_{x=x_0} \\ \\
>
> D_{\mathbf{u}}f & =\nabla f \cdot \hat{\mathbf{u}}
> \end{align}
> $$
>
> where the gradient vector, of f is
>
> $$
> \nabla f=\begin{pmatrix}\frac{\partial f}{\partial x}\\\frac{\partial f}{\partial y}\end{pmatrix}=\begin{pmatrix}
> f_{x} \\
> f_{y}
> \end{pmatrix}
> $$
>
> and the dot product expands to
>
> $$
> \hat{u}\cdot\nabla f=\begin{pmatrix}\hat{u}_x\\\hat{u}_y\end{pmatrix}\cdot\begin{pmatrix}\frac{\partial f}{\partial x}\\\frac{\partial f}{\partial y}\end{pmatrix}=\hat{u}_x\frac{\partial f}{\partial x}+\hat{u}_y\frac{\partial f}{\partial y}
> $$
>
> Also written as $\nabla_{\hat{u}}f$

See [[Question Type - Finding directional derivatives]].

> [!NOTE] Estimating $|\nabla f|$ from [[Contours]]
> The magnitude of the gradient can be estimated using contour spacing:
>
> $$
> |\nabla f| \approx \frac{\Delta f}{d}
> $$
>
> where:
>
> - $\Delta f$ is the difference between contour values (e.g. $f(x,y)=C_1$ and $f(x,y)=C_2$)
> - $d$ is the distance between those contour lines
>
>   ![[Attachments/Pasted image 20260507034233.png]]
