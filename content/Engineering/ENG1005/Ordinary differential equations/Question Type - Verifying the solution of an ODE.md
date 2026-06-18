# Example 1

Verify that $y(x)=\sqrt{ 1-x^2 }$ satisfies $\frac{dy}{dx}+\frac{x}{y}=0$.

### Step 1: Evaluate LHS using known $y(x)$

$$
\begin{align}
\frac{dy}{dx} & =\frac{1}{2}(1-x^2)^ {-\frac{1}{2}}(-2x) \\
 & =-\frac{x}{\sqrt{ 1-x^2 }} \\
 \implies \frac{dy}{dx}+\frac{x}{y} & =-\frac{x}{\sqrt{ 1-x^2 }}+\frac{x}{\sqrt{ 1-x^2 }} \\
  & =0
\end{align}
$$

Hence,  $y(x)=\sqrt{ 1-x^2 }$  is a solution.

# Example 2

Show that $y(x)=x^{-3/2}$ is a solution of $4x^2 y''+12xy'+3y=0$ for $x>0$.

### Step 1: Evaluate LHS using known $y(x)$

$$
\begin{align}
y' & = {-\frac{3}{2}}x^{-\frac{5}{2}} \\
y'' & =\left( -\frac{5}{2} \right)\left( -\frac{3}{2} \right)\left( x^{-\frac{7}{2}} \right) \\
 & =\frac{15}{4}x^{-\frac{7}{2}} \\
 \text{LHS} & =4x^2(y'')+12xy'+3y \\
  & =4x^2\left( \frac{15}{4}x^{-\frac{7}{2}} \right)+12x\left( -\frac{3}{2} x^{-\frac{5}{2}}\right)+3x^{-\frac{3}{2}} \\
   & =15x^{-\frac{3}{2}}-18x^{-\frac{3}{2}}+3x^{-\frac{3}{2}} \\
    & =0 \\
	 & =\text{RHS} \\
\end{align}
$$

Hence, $y(x)=x^{-3/2}$ is a solution.
