# Example 1: Direction of Largest Rate of Increase

What is the direction of the largest rate of increase of $f(x,y,z)=z\cos(x+y)$ at the point $\mathbf{x}=\left(0,\frac{\pi}{2},1\right)$?

## Step 1: Recall the definition of [[The gradient - nabla f]]

The gradient $\nabla f$ points in the direction of the largest rate of increase.

So we need to find $\nabla f$.

## Step 2: Compute the gradient $\nabla f$

$$
\begin{align}
\nabla f
&=
\begin{pmatrix}
\frac{\partial f}{\partial x}\\
\frac{\partial f}{\partial y}\\
\frac{\partial f}{\partial z}
\end{pmatrix} \\
&=
\begin{pmatrix}
-z\sin(x+y)\\
-z\sin(x+y)\\
\cos(x+y)
\end{pmatrix}
\end{align}
$$

## Step 3: Evaluate the gradient at required point

$$
\begin{align}
\nabla f\bigg|_{\left(0,\frac{\pi}{2},1\right)}
&=
\begin{pmatrix}
-1\sin\left(0+\frac{\pi}{2}\right)\\
-1\sin\left(0+\frac{\pi}{2}\right)\\
\cos\left(0+\frac{\pi}{2}\right)
\end{pmatrix} \\
&=
\begin{pmatrix}
-1\\
-1\\
0
\end{pmatrix}
\end{align}
$$

## Step 4: State the direction of largest rate of increase

Therefore, the direction of largest rate of increase is:

$$
\begin{pmatrix}
-1\\
-1\\
0
\end{pmatrix}
$$
