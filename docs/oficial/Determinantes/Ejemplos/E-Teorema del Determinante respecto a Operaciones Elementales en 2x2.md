**Ejemplo**. Veamos, en el caso de una matriz $A = [a_{ij}]$ de orden $2 \times 2$ que ocurre con el determinante cuando hacemos una operación elemental.
(1) Si $c \neq 0$, multiplicar por $c$ la primera fila y multiplicar $c$ por la segunda fila obtenemos, respectivamente,
$$
e(A) = \begin{bmatrix} ca_{11} & ca_{12} \\ a_{21} & a_{22} \end{bmatrix} \  \ \text{ y } \ \ e(A) = \begin{bmatrix} a_{11} & a_{12} \\ ca_{21} & ca_{22} \end{bmatrix},
$$
luego
$$
\det \begin{bmatrix} ca_{11} & ca_{12} \\ a_{21} & a_{22} \end{bmatrix} = ca_{11}a_{22} - ca_{12}a_{21} \text{ y } \det \begin{bmatrix} a_{11} & a_{12} \\ ca_{21} & ca_{22} \end{bmatrix} = ca_{11}a_{22} - ca_{12}a_{21}.
$$
Por lo tanto, en ambos casos, $\det e(A) = c \det A$.
(2) Sea $c \in \mathbb{K}$, si sumamos a la fila 2 la fila 1 multiplicada por $c$ o sumamos a la fila 1 la fila 2 multiplicada por $c$ obtenemos, respectivamente,
$$
e(A) = \begin{bmatrix} a_{11} & a_{12} \\ a_{21} + ca_{11} & a_{22} + ca_{12} \end{bmatrix} \text{ y } e(A) = \begin{bmatrix} a_{11} + ca_{21} & a_{12} + ca_{22} \\ a_{21} & a_{22} \end{bmatrix}.
$$
Por lo tanto,
$$
\begin{aligned}
\det \begin{bmatrix} a_{11} & a_{12} \\ a_{21} + ca_{11} & a_{22} + ca_{12} \end{bmatrix} &= a_{11}(a_{22} + ca_{12}) - a_{12}(a_{21} + ca_{11}) \\
&= a_{11}a_{22} + ca_{11}a_{12} - a_{12}a_{21} - ca_{12}a_{11} \\
&= a_{11}a_{22} - a_{12}a_{21} \\
&= \det A.
\end{aligned}
$$
En el otro caso también se comprueba que $\det e(A) = \det A$.
(3) Finalmente, intercambiando la fila 1 por la fila 2 obtenemos la matriz
$$
e(A) = \begin{bmatrix} a_{21} & a_{22} \\ a_{11} & a_{12} \end{bmatrix},
$$
por lo tanto
$$
\det e(A) = \det \begin{bmatrix} a_{21} & a_{22} \\ a_{11} & a_{12} \end{bmatrix} = a_{21}a_{12} - a_{22}a_{11} = -\det A.
$$
