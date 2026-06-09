#### **Teorema 1.1** Sea $e$ una operación elemental por fila y sea $E$ la matriz elemental $E=e(I)$ entonces $e(A)=EA$.

**DEMOSTRACIÓN**. Hagamos la prueba para matrices $2 \times 2$. La prueba en general es similar, pero requiere de un complicado manejo de índices.
(1) Si $c \ne 0$, multiplicar $I_2$ por $c$ la primera fila resulta en la matriz elemental
$$\begin{bmatrix}
c & 0 \\
0 & 1
\end{bmatrix}$$
Luego
$$\begin{bmatrix}
c & 0 \\
0 & 1
\end{bmatrix}
\begin{bmatrix}
a_{11} & a_{12} \\
a_{21} & a_{22}
\end{bmatrix}
=
\begin{bmatrix}
c \cdot a_{11} + 0 \cdot a_{21} & c \cdot a_{12} + 0 \cdot a_{22} \\
0 \cdot a_{11} + 1 \cdot a_{21} & 0 \cdot a_{12} + 1 \cdot a_{22}
\end{bmatrix}
=
\begin{bmatrix}
c \cdot a_{11} & c \cdot a_{12} \\
a_{21} & a_{22}
\end{bmatrix}
= e(A).$$
De forma análoga se demuestra en el caso que la operación elemental sea multiplicar la segunda fila por $c$.
****
(2) Si $c \in \mathbb{K}$, cambiar en $I_2$ la fila 2 por la fila 1 multiplicada por $c$ resulta en la matriz elemental$$\begin{bmatrix}
    1 & 0 \\
    c & 1
    \end{bmatrix}$$ Luego$$\begin{bmatrix}
    1 & 0 \\
    c & 1
    \end{bmatrix}
    \begin{bmatrix}
    a_{11} & a_{12} \\
    a_{21} & a_{22}
    \end{bmatrix}
    =
    \begin{bmatrix}
    a_{11} & a_{12} \\
    c \cdot a_{11} + a_{21} & c \cdot a_{12} + a_{22}
    \end{bmatrix}
    = e(A)$$
La demostración es análoga si la operación elemental es cambiar la fila 1 por la fila 2 multiplicada por $c$.
****
(3) Finalmente, si intercambiamos en $I_2$ la fila 1 por la fila 2 obtenemos la matriz elemental$$\begin{bmatrix}
    0 & 1 \\
    1 & 0
    \end{bmatrix} \\
$$Luego$$
    \begin{bmatrix}
    0 & 1 \\
    1 & 0
    \end{bmatrix}
    \begin{bmatrix}
    a_{11} & a_{12} \\
    a_{21} & a_{22}
    \end{bmatrix}
    =
    \begin{bmatrix}
    a_{21} & a_{22} \\
    a_{11} & a_{12}
    \end{bmatrix}
    = e(A).
$$