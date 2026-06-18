See [[Hyperbolic functions]].

# Example 1: Substitution using $x=\cosh(u)$ since expression contains $\sqrt{x^2-1}$

Evaluate:

$$
\int \frac{1}{\sqrt{x^2-1}} \, dx, \qquad x>1
$$

## Step 1: Choose a hyperbolic substitution

Since the expression contains $\sqrt{x^2-1}$, choose:

$$
x=\cosh(u)
$$

This is useful because:

$$
\cosh^2(u)-1=\sinh^2(u)
$$

## Step 2: Find $dx$

$$
\begin{align}
x &= \cosh(u) \\
\frac{dx}{du} &= \sinh(u) \\
dx &= \sinh(u)\,du
\end{align}
$$

## Step 3: Rewrite $\sqrt{x^2-1}$

$$
\begin{align}
x^2-1
&=\cosh^2(u)-1 \\
&=\sinh^2(u)
\end{align}
$$

Therefore:

$$
\sqrt{x^2-1}=\sqrt{\sinh^2(u)}=\sinh(u)
$$

since $x>1$ implies $u>0$, so $\sinh(u)>0$.

## Step 4: Substitute into the integral

$$
\begin{align}
\int \frac{1}{\sqrt{x^2-1}}\,dx
&=\int \frac{1}{\sinh(u)}\sinh(u)\,du \\
&=\int 1\,du \\
&=u+C
\end{align}
$$

## Step 5: Convert back to $x$

Since:

$$
x=\cosh(u)
$$

we have:

$$
u=\cosh^{-1}(x)
$$

So:

$$
\int \frac{1}{\sqrt{x^2-1}}\,dx
=
\cosh^{-1}(x)+C
$$

Using the identity:

$$
\cosh^{-1}(x)=\log\left(x+\sqrt{x^2-1}\right)
$$

the final answer is:

$$
\boxed{
\int \frac{1}{\sqrt{x^2-1}}\,dx
=
\log\left(x+\sqrt{x^2-1}\right)+C
}
$$
