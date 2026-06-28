**Ejemplo:** $T: \mathbb{R}^2 \to \mathbb{R}^2$, $T(x_1, x_2) = (x_1, 0)$

- $\mathcal{C} = \{e_1, e_2\}$ base canónica
- $\beta = \{w_1 = (1, 1), w_2 = (2, 1)\}$ base de $\mathbb{R}^2$

$[T]_{\mathcal{C}} = \begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix}$

Sea $P$ mat. cambio de $\beta$ a $\mathcal{C} = \begin{pmatrix} 1 & 2 \\ 1 & 1 \end{pmatrix}$

Por teorema, tenemos que $[T]_{\beta} = P^{-1} [T]_{\mathcal{C}} P$; $P^{-1} = \begin{pmatrix} -1 & 2 \\ 1 & -1 \end{pmatrix}$ (verificar)

$[T]_{\beta} = \begin{pmatrix} -1 & 2 \\ 1 & -1 \end{pmatrix} \begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix} \begin{pmatrix} 1 & 2 \\ 1 & 1 \end{pmatrix} = \begin{pmatrix} -1 & -2 \\ 1 & 2 \end{pmatrix}$

En particular $T(w_1) = ?$ 
$[T(w_1)]_{\beta} = (-1, 1) = 1^{\circ}$ columna de $[T]_{\beta}$
$\Rightarrow T(w_1) = -1w_1 + 1w_2 = -(1, 1) + (2, 1) = (1, 0)$

$T(w_2) = ?$
$[T(w_2)]_{\beta} = (-2, 2)$
$\Rightarrow T(w_2) = -2w_1 + 2w_2 = (2, 0)$