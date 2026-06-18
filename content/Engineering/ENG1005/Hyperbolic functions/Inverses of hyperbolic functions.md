see [[Hyperbolic functions]].

> [!NOTE] Derivation of $cosh^{-1}(x)$
> Let:
>
> $$
> \begin{align}
> y &= \cosh(x) \\
> &= \frac{1}{2}(e^x+e^{-x}) \\
> 2y &= e^x+e^{-x} \\
> &\implies e^{2x}-2ye^x+1=0
> \end{align}
> $$
>
> Solving this quadratic with $e^x$ as the variable:
>
> $$
> \begin{align}
> e^x &= \frac{2y\pm\sqrt{(2y)^2-4}}{2} \\
> &= y\pm\sqrt{y^2-1}
> \end{align}
> $$
>
> Solving for $x$ gives:
>
> $$
> \begin{align}
> x &= \log(y\pm\sqrt{y^2-1})
> \end{align}
> $$
>
> Observing the graph of $\cosh(x)$ (see [[Hyperbolic functions]]), we see that for one $y$ value, there are 2 $x$ values with the same magnitude but different signs.
>
> This signals that we can take the $\pm$ out of the $log$.
>
> $$
> \begin{align}
> y-\sqrt{ y^2-1 } & =y-\sqrt{ y^2-1 }\times \frac{y+\sqrt{ y^2-1 }}{y+\sqrt{ y^2-1 }} \\
>  & = \frac{(y-\sqrt{ y^2-1 })(y+\sqrt{ y^2-1 })}{y+\sqrt{ y^2-1 }} \\
>   & =\frac{y^2-(\sqrt{ y^2-1 })^2}{y+\sqrt{ y^2-1 }} \\
>    & =\frac{1}{y+\sqrt{ y^2-1 }}
> \end{align}
> $$
>
> plugging the re-arranged argument back into the log:
>
> $$
> \begin{align}
> x & =\log(y+\sqrt{ y^2-1 })\text{ or } \log\left( \frac{1}{y+\sqrt{ y^2-1 }} \right) \\
>  & =\pm \log(y+\sqrt{ y^2-1 })
> \end{align}
> $$
