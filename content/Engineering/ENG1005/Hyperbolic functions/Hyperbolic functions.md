Complex representation for trigonometric functions. Recalling [[Euler's formula]]:

$$
\begin{align}
e^{ix} & =\cos(x)+i\sin(x) & \dots_{1}\\
e^{-ix} & =\cos(-x)+i\sin(-x) & \dots_{2}\\
 & =\cos (x)-i\sin(x)
\end{align}
$$

Adding the two equations, we get:

$$
\begin{align}
e^{ix}+e^-ix & =2\cos(x) \\
 \implies & \cos(x)=\frac{1}{2} (e^{ix}+e^{-ix})
\end{align}
$$

Subtracting the two equations, we get:

$$
\begin{align}
e^{ix}-e^-ix & =2\sin(x) \\
 \implies & \sin(x)=\frac{1}{2i} (e^{ix}-e^{-ix})
\end{align}
$$

This is important for [[Derivatives of hyperbolic functions]].

Similar to [[trigonometric functions]], hyperbolic functions have certain [[hyperbolic identities]] that are useful for mathematical operations, eg:

$$
\begin{align}
\cosh^2(x)-\sinh^2(x) & =1 \\
\cosh^2(x)+\sinh^2(x) & =\cosh(2x) \\
1-\tanh^2(x) & =\text{sech}^2(x) \\
\coth^2(x)-1 & =\text{cosech}^2(x) \\
\sinh(2x) & =2\cosh(x) \sinh(x)
\end{align}
$$

Hyperbolic functions also have inverse functions. Refer to [[Inverses of hyperbolic functions]].

> [!NOTE] Definition
>
> $$
> \cosh(x)=\frac{1}{2} (e^x+e^{-x})
> $$
>
> intercept at $(0,1)$
> ![[Attachments/Pasted image 20260506080950.png]]

> [!NOTE] Definition
>
> $$
> \sinh(x)=\frac{1}{2} (e^x-e^{-x})
> $$
>
> y-intercept at $(0,0)$
> ![[Attachments/Pasted image 20260506081131.png]]

> [!NOTE] Definition
>
> $$
> \tanh(x)= \frac{\sinh(x)}{\cosh(x)}
> $$
>
> intercept at $(0,0)$
> ![[Attachments/Pasted image 20260506084331.png]]

> [!NOTE] Definition
>
> $$
> \text{sech}(x)= \frac{1}{\cosh(x)}
> $$
>
> intercept at $(0,1)$
> ![[Attachments/Pasted image 20260506084611.png]]

> [!NOTE] Definition
>
> $$
> \text{cosech}(x)= \frac{1}{\sinh(x)}
> $$
>
> ![[Attachments/Pasted image 20260506084756.png]]

> [!NOTE] Definition
>
> $$
> \text{coth}(x)= \frac{\cosh(x)}{\sinh(x)}=\frac{1}{\tanh(x)}
> $$
>
> ![[Attachments/Pasted image 20260506084824.png]]
