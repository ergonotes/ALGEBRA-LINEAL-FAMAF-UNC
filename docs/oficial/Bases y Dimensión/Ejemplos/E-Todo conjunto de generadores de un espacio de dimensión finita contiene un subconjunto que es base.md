**Ejemplo 1.** $S = \{(1, 1, 1), (3, 2, 2)\}$ es L.I. en $\mathbb{R}^3$. Extender a una base de $\mathbb{R}^3$.
*Importante:* identificar cuál es $\langle S \rangle$ para añadir un vector que no haga a $S$ un conjunto LD.

$$
\langle S \rangle = \{c_1(1, 1, 1) + c_2(3, 2, 2) : c_1, c_2 \in \mathbb{R}\} = \left\{ (x, y, z) \in \mathbb{R}^3 \mid \begin{matrix} x = c_1 + 3c_2 \\ y = c_1 + 2c_2 \\ z = c_1 + 2c_2 \end{matrix} \right\}.
$$

¿Cómo identificar con ecuaciones? Miramos el sistema $\begin{pmatrix} 1 & 3 \\ 1 & 2 \\ 1 & 2 \end{pmatrix} \begin{pmatrix} c_1 \\ c_2 \end{pmatrix} = \begin{pmatrix} x \\ y \\ z \end{pmatrix}$.
Entonces
$$
\langle S \rangle = \left\{ (x_1, x_2, x_3) \in \mathbb{R}^3 : A\begin{pmatrix} c_1 \\ c_2 \end{pmatrix} = \begin{pmatrix} x \\ y \\ z \end{pmatrix} \text{ tiene solución} \right\}.
$$
Escalonamos la matriz aumentada:
$$
\left( \begin{matrix} 1 & 3 & x \\ 1 & 2 & y \\ 1 & 2 & z \end{matrix} \right) \xrightarrow{f_1-f_2, f_2-f_3} \left( \begin{matrix} 1 & 3 & x \\ 0 & 1 & x - y \\ 0 & 0 & y - z \end{matrix} \right) \to \left( \begin{matrix} 1 & 0 & x - 3(x - y) \\ 0 & 1 & x - y \\ 0 & 0 & \boxed{y - z} \end{matrix} \right)
$$
La condición para que haya solución es $y - z = 0$.
Por lo tanto $\langle S \rangle = \{(x, y, z) : y = z\}$.
$\Rightarrow$ Por ejemplo, $e_2 = (0, 1, 0) \notin \langle S \rangle$, luego $S \cup \{e_2\}$ es L.I. Como $\dim \mathbb{R}^3 = 3$ y además tenemos 3 vectores, sabemos que también generan (verificar). Por lo tanto
$$
S \cup \{e_2\} = \{(1, 1, 1), (3, 2, 2), (0, 1, 0)\}
$$
es una base de $\mathbb{R}^3$ que contiene a $S$.