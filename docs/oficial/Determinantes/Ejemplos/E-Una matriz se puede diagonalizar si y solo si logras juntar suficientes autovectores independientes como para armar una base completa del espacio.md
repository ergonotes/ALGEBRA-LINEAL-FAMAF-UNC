**Ejemplo 1**. Consideremos la transformación lineal de $\mathbb{R}^3$ en $\mathbb{R}^3$ definida por la matriz $A$ a la izquierda, es decir (con abuso de notación incluido)
$$
\begin{bmatrix}
10 & -10 & 6 \\
8 & -8 & 6 \\
-5 & 5 & -3
\end{bmatrix} \begin{bmatrix} x \\ y \\ z \end{bmatrix} = \begin{bmatrix} 10x - 10y + 6z \\ 8x - 8y + 6z \\ -5x + 5y - 3z \end{bmatrix}.
$$

Ya vimos que el polinomio característico de esta aplicación es
$$
\chi_A(x) = -x(x - 2)(x + 3).
$$

Luego, por el [[D-Criterio del Determinante para Autovalores]], los autovalores de $A$ son $0, 2$ y $-3$. Debido a que [[D-Autovalores distintos producen autovectores linealmente independientes]], existe una base de autovectores de $A$. Veamos cuales son. Si $\lambda$ autovalor de $A$, para encontrar los autovectores con autovalor $\lambda$ debemos resolver la ecuación $Av - \lambda v = 0$, en este caso sería

$$
\begin{bmatrix}
10 - \lambda & -10 & 6 \\
8 & -8 - \lambda & 6 \\
-5 & 5 & -3 - \lambda
\end{bmatrix}
\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}
=
\begin{bmatrix}
0 \\
0 \\
0
\end{bmatrix},
$$

para $\lambda = 0, 2, -3$. Resolviendo estos tres sistemas, obtenemos que
$$
V_0 = \{(y, y, 0) : y \in \mathbb{R}\}, \quad V_2 = \{(-2z, -z, z) : z \in \mathbb{R}\}, \quad V_{-3} = \{(-2z, -2z, z) : z \in \mathbb{R}\}.
$$
Por lo tanto, $\{(1, 1, 0), (-2, -1, 1), (-2, -2, 1)\}$ es una base de autovectores de la transformación lineal.
****
Chequeemos ahora que la matriz de la transformación en esta nueva base es, efectivamente, **diagonal**.

Llamemos $\beta = \{v_1, v_2, v_3\}$ a nuestra nueva base de autovectores, donde $v_1 = (1, 1, 0)$, $v_2 = (-2, -1, 1)$ y $v_3 = (-2, -2, 1)$. Para construir la matriz de la transformación en la base $\beta$, a la cual denotaremos como $[T]_\beta$, debemos aplicar la transformación (representada por la matriz original $A$) a cada vector de la base y luego expresar el resultado como una combinación lineal de esos mismos vectores de $\beta$.

Aplicamos la matriz $A$ a cada autovector:

**Para $v_1$ (asociado a $\lambda = 0$):**

$$Av_1 = \begin{bmatrix} 10 & -10 & 6 \\ 8 & -8 & 6 \\ -5 & 5 & -3 \end{bmatrix} \begin{bmatrix} 1 \\ 1 \\ 0 \end{bmatrix} = \begin{bmatrix} 10 - 10 + 0 \\ 8 - 8 + 0 \\ -5 + 5 - 0 \end{bmatrix} = \begin{bmatrix} 0 \\ 0 \\ 0 \end{bmatrix} $$

Expresado en la base $\beta$, este vector es $0 \cdot v_1 + 0 \cdot v_2 + 0 \cdot v_3$.

**Para $v_2$ (asociado a $\lambda = 2$):**

$$Av_2 = \begin{bmatrix} 10 & -10 & 6 \\ 8 & -8 & 6 \\ -5 & 5 & -3 \end{bmatrix} \begin{bmatrix} -2 \\ -1 \\ 1 \end{bmatrix} = \begin{bmatrix} -20 + 10 + 6 \\ -16 + 8 + 6 \\ 10 - 5 - 3 \end{bmatrix} = \begin{bmatrix} -4 \\ -2 \\ 2 \end{bmatrix} $$

Podemos notar fácilmente que el resultado es el doble de $v_2$. Expresado en la base $\beta$, este vector es $0 \cdot v_1 + 2 \cdot v_2 + 0 \cdot v_3$.

**Para $v_3$ (asociado a $\lambda = -3$):**

$$Av_3 = \begin{bmatrix} 10 & -10 & 6 \\ 8 & -8 & 6 \\ -5 & 5 & -3 \end{bmatrix} \begin{bmatrix} -2 \\ -2 \\ 1 \end{bmatrix} = \begin{bmatrix} -20 + 20 + 6 \\ -16 + 16 + 6 \\ 10 - 10 - 3 \end{bmatrix} = \begin{bmatrix} 6 \\ 6 \\ -3 \end{bmatrix} $$

Nuevamente, vemos que el resultado es igual a multiplicar $v_3$ por su autovalor. Expresado en la base $\beta$, este vector es $0 \cdot v_1 + 0 \cdot v_2 - 3 \cdot v_3$.

Las coordenadas de estos tres vectores transformados conformarán, de manera respectiva, las columnas de nuestra nueva matriz.

$$[T]_\beta = \begin{bmatrix} 0 & 0 & 0 \\ 0 & 2 & 0 \\ 0 & 0 & -3 \end{bmatrix}$$

Como podemos observar, la matriz de la transformación lineal expresada en la base de sus autovectores es estrictamente diagonal. Además, queda en evidencia cómo los elementos de su diagonal principal corresponden exactamente a los autovalores $0, 2$ y $-3$, posicionados en el mismo orden que los autovectores en nuestra base $\beta$.