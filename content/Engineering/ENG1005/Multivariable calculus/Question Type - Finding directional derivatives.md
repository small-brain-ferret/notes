See [[Directional derivatives]].

# Example 1

Find the directional derivative of $f(x,y)=1+x^2+y^2$ at $\mathbf{x}=(0,1)$ in the direction

$$
\frac{1}{\sqrt{5}}\begin{bmatrix}1\\2\end{bmatrix}
$$

## Step 1: Identify the unit direction vector

$$
\hat{u}=\frac{1}{\sqrt{5}}\begin{bmatrix}1\\2\end{bmatrix}
$$

## Step 2: Compute the gradient

$$
\begin{align}
\nabla f
&=\begin{pmatrix}\frac{\partial f}{\partial x}\\\frac{\partial f}{\partial y}\end{pmatrix} \\
&=\begin{pmatrix}2x\\2y\end{pmatrix}
\end{align}
$$

## Step 3: Evaluate the gradient at  the required point

$$
\begin{align}
\nabla f\big|_{(0,1)}
&=\begin{pmatrix}2(0)\\2(1)\end{pmatrix} \\
&=\begin{pmatrix}0\\2\end{pmatrix}
\end{align}
$$

## Step 4: Plug values into $\frac{\partial f}{\partial u}=\hat{u}\cdot\nabla f$ to find the required directional derivative.

$$
\begin{align}
\frac{\partial f}{\partial u}
&=\hat{u}\cdot\nabla f \\
&=\frac{1}{\sqrt{5}}\begin{pmatrix}1\\2\end{pmatrix}\cdot\begin{pmatrix}0\\2\end{pmatrix} \\
&=\frac{1}{\sqrt{5}}(1\cdot0+2\cdot2) \\
&=\frac{4}{\sqrt{5}}
\end{align}
$$
