See [[First order separable ODEs]].

> [!NOTE] Solving
>
> $$
> \begin{align}
> \frac{dy}{dx} & =f(x)g(y) \\
> f(x) & = \frac{1}{g(y)} \frac{dy}{dx} \\
> \int f(x) \,dx & =\int \frac{1}{g(y)}\,dy
> \end{align}
> $$

# Example 1

Water drains from a tank at the rate $\frac{dV}{dt} =-k\sqrt{ V }$. We know that $V=V_0$ at $t=0$.

### Step 1: Do separation of variables

$$
\begin{align}
\int \frac{1}{\sqrt{ V }}\,dV & =-\int \text{k} \,dt \\
\implies 2V^{1/2} & =-\text{k}\, t+C \\
\end{align}
$$

### Step 2: Consider boundary conditions

Considering  $V=V_0$ at $t=0$, we get:

$$
\begin{align}
2V_{0}^{\frac{1}{2}} & =-k\cdot 0 + C \\
C & =2V_{0}^{\frac{1}{2}} \\
\implies{2}V^{\frac{1}{2}} & =-\text{k}t+2V_{0}^{\frac{1}{2}} \\
\implies V & =\left( V_{0}^{\frac{1}{2}}-\frac{1}{2} \text{k}t \right)^2
\end{align}
$$

# Example 2

Find the general solution of the separable ODE $\frac{dy}{dx}=2xy$.

### Step 1: Do separation of variables

$$
\begin{align}
\frac{dy}{dx} & =2xy \\
\int \frac{1}{y}\,dy & =\int 2x \,dx \\
\log_{e}(y) & =x^2+C \\
y & =e^{x^2+C} \\
y & =Ae^{x^2}
\end{align}
$$

# Example 3

Find the general solution to the separable ODE $y \frac{dy}{dx}+\sin(x)=0$.

### Step 1: Do separation of variables

$$
\begin{align}
y \frac{dy}{dx}+\sin(x) & =0 \\
y \frac{dy}{dx} & =-\sin(x) \\
\int y\,dy & =\int-\sin(x)\,dx \\
\frac{1}{2}y^2 & =\cos(x)+C_{1} \\
y^2 & =2\cos(x) +C_{2} \\
y & =\pm \sqrt{ 2\cos(x) +C }
\end{align}
$$

## Example 4

Find the general solution for $\sin(x)\frac{dy}{dx}+y\cos(x)=2\cos(x)$

### Step 1: Separation of variables

$$
\begin{align}
\frac{\sin(x)}{\cos(x)}\frac{dy}{dx}+\frac{y\cos(x)}{\cos(x)} & =\frac{2\cos(x)}{\cos(x)} \\
\tan(x)\frac{dy}{dx}+y & =2 \\
\tan(x) \frac{dy}{dx} & =2-y \\
\int \frac{1}{2-y}\,dy=\int \cot(x)\,dx \\
\end{align}
$$

### Step 1a: evaluate RHS

See [[Integral of cot(x)]].
