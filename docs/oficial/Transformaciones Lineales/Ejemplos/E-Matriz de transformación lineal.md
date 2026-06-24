**Ejemplo**. Sea $T: \mathbb{R}^3 \to \mathbb{R}^4$ definida
$$
T(x, y, z) = (2x + y, 3y, x + 4z, z).
$$
Sean $\mathcal{B} = \{e_1, e_2, e_3\}$ la base canónica de $\mathbb{R}^3$ y $\mathcal{B}' = \{e_1, e_2, e_3, e_4\}$ la base canónica de $\mathbb{R}^4$. Entonces
$$
\begin{aligned}
T(e_1) &= (2, 0, 1, 0) &= 2e_1 + 0e_2 + e_3 + 0e_4 \\
T(e_2) &= (1, 3, 0, 0) &= e_1 + 3e_2 + 0e_3 + 0e_4 \\
T(e_3) &= (0, 0, 4, 1) &= 0e_1 + 0e_2 + 4e_3 + e_4
\end{aligned}
$$
Por lo tanto
$$
[T]_{\mathcal{B}\mathcal{B}'} = \begin{bmatrix} 2 & 1 & 0 \\ 0 & 3 & 0 \\ 1 & 0 & 4 \\ 0 & 0 & 1 \end{bmatrix}.
$$
Observar que si escribimos los vectores en coordenadas con respecto a las bases canónicas, tenemos que
$$
\begin{bmatrix} 2 & 1 & 0 \\ 0 & 3 & 0 \\ 1 & 0 & 4 \\ 0 & 0 & 1 \end{bmatrix} \begin{bmatrix} x \\ y \\ z \end{bmatrix} = \begin{bmatrix} 2x + y \\ 3y \\ x + 4z \\ z \end{bmatrix}
$$
o más formalmente
$$
[T]_{\mathcal{B}\mathcal{B}'} [v]_{\mathcal{B}} = [T(v)]_{\mathcal{B}'}.
$$
****
Cabe aclarar que no es necesario que se usen las bases canónicas para dar el ejemplo. La matriz de la transformación podría formarse a partir de otras bases del conjunto de salida y de llegada.