> [!NOTE] Use of [[Diagonalisation(s)]]
> If
>
> $$
> A=VDV^{-1}
> $$
>
> then powers of $A$ can be computed efficiently:
>
> $$
> \begin{align}
> A^{n}
> &= (VDV^{-1})(VDV^{-1})\cdots(VDV^{-1})\\
> &= VD(V^{-1}V)D(V^{-1}V)\cdots DV^{-1}\\
> &= VD^nV^{-1}
> \end{align}
> $$
>
> since (see [[Inverses of matrices]])
>
> $$
> V^{-1}V=I
> $$
>
> If
>
> $$
> D=
> \begin{pmatrix}
> \lambda_1&0&\cdots&0\\
> 0&\lambda_2&\cdots&0\\
> \vdots&\vdots&\ddots&\vdots\\
> 0&0&\cdots&\lambda_n
> \end{pmatrix}
> $$
>
> then
>
> $$
> D^n=
> \begin{pmatrix}
> \lambda_1^n&0&\cdots&0\\
> 0&\lambda_2^n&\cdots&0\\
> \vdots&\vdots&\ddots&\vdots\\
> 0&0&\cdots&\lambda_n^n
> \end{pmatrix}
> $$
>
> so only the diagonal entries need to be raised to the power, making it easy to compute powers of matrices.
