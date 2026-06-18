> [!NOTE]
> For a function $f(\mathbf{x})$ at a point $\mathbf{x}_0$:
>
> $$
> \text{tangent approximation}=f(\mathbf{x}_0)+(\mathbf{x}-\mathbf{x}_0)\cdot\nabla f\big|_{\mathbf{x}=\mathbf{x}_0}
> $$
>
> For $z=f(x,y)$, this gives a tangent plane.
>
> For higher-dimensional functions, this gives a tangent hyperplane.

# Example 1: Tangent Plane

Find the tangent plane of $f(x,y)=xy^2$ at $\mathbf{x}=(0,-1)$.

## Step 1: Find the value of the function at the given point

$$
\begin{align}
f(0,-1)&=0(-1)^2\\
&=0
\end{align}
$$

## Step 2: Find  [[The gradient - nabla f]]

$$
\begin{align}
\nabla f
&=\begin{pmatrix}f_x\\f_y\end{pmatrix}\\
&=\begin{pmatrix}y^2\\2xy\end{pmatrix}
\end{align}
$$

## Step 3: Evaluate the gradient at the given point

$$
\begin{align}
\nabla f\big|_{(0,-1)}
&=\begin{pmatrix}(-1)^2\\2(0)(-1)\end{pmatrix}\\
&=\begin{pmatrix}1\\0\end{pmatrix}
\end{align}
$$

## Step 4: Find the displacement vector from the given point

$$
\begin{align}
\mathbf{x}-\mathbf{x}_0
&=\begin{pmatrix}x\\y\end{pmatrix}-\begin{pmatrix}0\\-1\end{pmatrix}\\
&=\begin{pmatrix}x\\y+1\end{pmatrix}
\end{align}
$$

## Step 5: Substitute into the tangent plane formula

$$
\begin{align}
z&=f(x_0,y_0)+(\mathbf{x}-\mathbf{x}_0)\cdot\nabla f\big|_{\mathbf{x}=\mathbf{x}_0}\\
&=0+\begin{pmatrix}x\\y+1\end{pmatrix}\cdot\begin{pmatrix}1\\0\end{pmatrix}\\
&=x
\end{align}
$$

Therefore, the tangent plane is $z=x$.

# Example 2: Tangent Hyperplane

Find the tangent hyperplane of $f(w,x,y,z)=(x^2+3wz)y$ at $\mathbf{x}=(1,1,1,1)$.

## Step 1: Find the value of the function at the given point

$$
\begin{align}
f(1,1,1,1)&=(1^2+3(1)(1))(1)\\
&=4
\end{align}
$$

## Step 2: Find the gradient

$$
\begin{align}
\nabla f
&=\begin{pmatrix}f_w\\f_x\\f_y\\f_z\end{pmatrix}\\
&=\begin{pmatrix}3zy\\2xy\\x^2+3wz\\3wy\end{pmatrix}
\end{align}
$$

## Step 3: Evaluate the gradient at the given point

$$
\begin{align}
\nabla f\big|_{(1,1,1,1)}
&=\begin{pmatrix}3(1)(1)\\2(1)(1)\\1^2+3(1)(1)\\3(1)(1)\end{pmatrix}\\
&=\begin{pmatrix}3\\2\\4\\3\end{pmatrix}
\end{align}
$$

## Step 4: Find the displacement vector from the given point

$$
\begin{align}
\mathbf{x}-\mathbf{x}_0
&=\begin{pmatrix}w\\x\\y\\z\end{pmatrix}-\begin{pmatrix}1\\1\\1\\1\end{pmatrix}\\
&=\begin{pmatrix}w-1\\x-1\\y-1\\z-1\end{pmatrix}
\end{align}
$$

## Step 5: Substitute into the tangent hyperplane formula

$$
\begin{align}
\zeta
&=f(\mathbf{x}_0)+(\mathbf{x}-\mathbf{x}_0)\cdot\nabla f\big|_{\mathbf{x}=\mathbf{x}_0}\\
&=4+\begin{pmatrix}w-1\\x-1\\y-1\\z-1\end{pmatrix}\cdot\begin{pmatrix}3\\2\\4\\3\end{pmatrix}\\
&=4+3(w-1)+2(x-1)+4(y-1)+3(z-1)
\end{align}
$$

Therefore, the tangent hyperplane is:

$$
\zeta=4+3(w-1)+2(x-1)+4(y-1)+3(z-1)
$$
