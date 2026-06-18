See [[Critical points]].

# Example 1

What are the critical points of $f(x,y)=1+x^2+y^2$ ?

Step 1: Solve $\nabla f=0$ for $x$ and $y$
$\nabla f=0$

$$
\begin{bmatrix}

\frac{\partial f}{\partial x}\\
\frac{\partial f}{\partial y}\\
\end{bmatrix}=
\begin{bmatrix}
0\\
0
\end{bmatrix}
$$

Step 1a): Solve $\frac{\partial f}{\partial x}=0$.
$\frac{\partial f}{\partial x}\\=2x=0\implies x=0$
Step 1b): Solve $\frac{\partial f}{\partial y}=0$.
$\frac{\partial f}{\partial y}\\=2y=0\implies y=0$
$\therefore (x_{0},y_{0})=(0,0)$

# Example 2

Find the critical points of $f(x,y)=-(x^2-1)(y^2-1)$

Step 1: Solve $\nabla f=0$ for $x$ and $y$

$$
\begin{bmatrix}

\frac{\partial f}{\partial x}\\
\frac{\partial f}{\partial y}\\
\end{bmatrix}=
\begin{bmatrix}
0\\
0
\end{bmatrix}
$$

Step 1a): Solve $\frac{\partial f}{\partial x}=0$.
$\frac{\partial f}{\partial x}\\=-2x(y^2-1)=0$
$\implies\text{either }x=0\text{ or }y^2-1=0\implies y=\pm1$
Step 1b): Solve $\frac{\partial f}{\partial y}=0$.

$$\frac{\partial f}{\partial y}\\=-2y(x^2-1)=0
$$

$$
\implies y=0\text{ or }x^2-1=0\implies x=\pm 1
$$

Step 2: Solve for the corresponding values of each solved value using simultaneous equations.
$\therefore (x,y)=(0,0),\ (1,1),\ (1,-1),\ (-1,1),\ (-1,-1)$

# Example 3

Find all of the critical points for the function
$f(x,y)=4-x^2-y^2$
Step 1: Solve $\nabla f=0$ for $x$ and $y$

$$$\begin{bmatrix}

\frac{\partial f}{\partial x}\\
\frac{\partial f}{\partial y}\\
\end{bmatrix}=
\begin{bmatrix}
0\\
0
\end{bmatrix}$$
Step 1a): Solve $\frac{ \partial f }{ \partial x }=0$.
$$\frac{ \partial f }{ \partial x } =-2x=0
\implies x=0$$
Step 1b): Solve $\frac{ \partial f }{ \partial y }=0$.
$$\frac{ \partial f }{ \partial y }=-2y=0\implies y=0 
$$$

$\therefore (x_{0},y_{0})=(0,0)$

# Example 4

Find all of the critical points for the function
$h(x,y)=x-x^3+y^2$
Step 1: Solve $\nabla f=0$ for x and y

$$$$$\begin{bmatrix}

\frac{\partial f}{\partial x}\\
\frac{\partial f}{\partial y}\\
\end{bmatrix}=
\begin{bmatrix}
0\\
0
\end{bmatrix}$$
Step 1a): Solve $\frac{ \partial f }{ \partial x }=0$.
$$\frac{ \partial f }{ \partial x } =1-3x^2=0
\implies x=\pm \frac{1}{\sqrt{ 3 }}$$
Step 1b): Solve $\frac{ \partial f }{ \partial y }=0$.
$$\frac{ \partial f }{ \partial y }=2y=0\implies y=0 
$$$$\therefore (x,y)= \left( \frac{1}{\sqrt{ 3 }},0 \right),\ \left(  -\frac{1}{\sqrt{ 3 }},0 \right)$$
# Example 5
Find all of the critical points for the function
$$g(x,y)=xye^{-x^2-y^2}$$
Step 1: Solve $\nabla g=0$ for x and y
$$\begin{bmatrix}

\frac{\partial g}{\partial x}\\
\frac{\partial g}{\partial y}\\
\end{bmatrix}=
\begin{bmatrix}
0\\
0
\end{bmatrix}$$
Step 1a): Solve $\frac{ \partial g }{ \partial x }=0$.
$$$$$

\begin{align}
\frac{ \partial g }{ \partial x } & =y(1\cdot e^{-x^2-y^2}+x\cdot-2x\cdot e^{-x^2-y^2})  \\
& =y(e^{-x^2-y^2})(1-2x^2) \\
\frac{ \partial g }{ \partial x } & =0 \\
y(e^{-x^2-y^2})(1-2x^2) & =0 \\
& \implies y =0\ or\ x=\pm \frac{1}{\sqrt{ 2 }}
\end{align}

$$
Step 1b): Solve $\frac{ \partial g }{ \partial y }=0$.
$$

\begin{align}
\frac{ \partial g }{ \partial y } & =y(1\cdot e^{-y^2-x^2}+y\cdot-2y\cdot e^{-y^2-x^2})  \\
& =x(e^{-y^2-x^2})(1-2y^2) \\
\frac{ \partial g }{ \partial y } & =0 \\
y(e^{-y^2-x^2})(1-2y^2) & =0 \\
& \implies x =0\ or\ y=\pm \frac{1}{\sqrt{ 2 }}
\end{align}

$$
Step 2: Solve for the corresponding values of each solved value using simultaneous equations.
$$

\begin{align}
(x\_{1},y\_{1}) & =(0,0) \\
(x\_{2},y\_{2}) & =\left( \frac{1}{\sqrt{ 2 }} , \frac{1}{\sqrt{ 2 }} \right)\\
(x\_{3},y\_{3}) & =\left( \frac{1}{\sqrt{ 2 }} , -\frac{1}{\sqrt{ 2 }} \right)\ \\
(x\_{4},y\_{4}) & =\left( -\frac{1}{\sqrt{ 2 }} , \frac{1}{\sqrt{ 2 }} \right)\ \\
(x\_{5},y\_{5}) & =\left( -\frac{1}{\sqrt{ 2 }} , -\frac{1}{\sqrt{ 2 }} \right)\\
\end{align}

$$
$$
