> [!NOTE] Definition
> The tangent plane at $(x_0,y_0)$ is:
>
> $$
> \begin{align}
> z  & = f(x_0,y_0) + \nabla f(x_0,y_0)\cdot \begin{pmatrix}x-x_0 \\ y-y_0\end{pmatrix} \\ \\
>
>  & =\begin{pmatrix}
> f_{x}(a,b)\\f_{y}(a,b)\\-1
> \end{pmatrix} \cdot \begin{pmatrix}
> x\\y\\z
> \end{pmatrix} \\ \\
>
>  & =\begin{pmatrix}
> f_{x}(a,b)\\f_{y}(a,b)\\-1
> \end{pmatrix} \cdot \begin{pmatrix}
> a\\b\\f(a,b)
> \end{pmatrix}
> \end{align}
> $$
>
> Meaning:
>
> - The plane **touches the surface** at $(x_0,y_0)$
> - The plane has the **same gradient (slope)** as the surface at that point
>
> Expanded form:
>
> $$
> z = f(x_0,y_0) + f_x(x_0,y_0)(x-x_0) + f_y(x_0,y_0)(y-y_0)
> $$

See [[Question Type - Finding a tangent plane or hyperplane]]

The tangent plane to the surface at P has vector equation:

$$$\begin{pmatrix}
f_{x}(a,b)\\f_{y}(a,b)\\-1
\end{pmatrix} \cdot \begin{pmatrix}
x\\y\\z
\end{pmatrix}=\begin{pmatrix}
f_{x}(a,b)\\f_{y}(a,b)\\-1
\end{pmatrix} \cdot \begin{pmatrix}
a\\b\\f(a,b)
\end{pmatrix}$$ The scalar product of the above equation is:
$$z = f_{x}(a,b) \cdot (x-a) + f_{y}(a,b)\cdot(y-b)+f(a,b) $$
Remember it as:

The partial derivative with respect to $x$ multiplied by $x-a$ plus the partial derivative with respect to $y$ multiplied by $y-b$ +plus the value of $f(a,b)$ 


[[normal line]]

The normal line has direction $\begin{pmatrix}f_{x}(a,b)\\f_{y}(a,b)\\-1\end{pmatrix}$
The equation of a normal line at point P where P is $(a, b, f(a,b))$ is:
$$\begin{pmatrix}x\\y\\z\end{pmatrix} = \begin{pmatrix}a\\b\\f(a,b)\end{pmatrix} +\begin{pmatrix}f_{x}(a,b)\\f_{y}(a,b)\\-1\end{pmatrix}t, t\in \mathbb{R}$$

Remember it as:
The normal line is equal to the x, y, z values of the point plus their respective [[partial derivatives]] (with the exception of z which is -1)
$$$
