**Ejemplo 2. Con autovalor $0$:**
Sea $A = \begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix}$ y $v = \begin{pmatrix} 1 \\ 0 \end{pmatrix}$. Entonces

$$
Av = \begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix} \begin{pmatrix} 1 \\ 0 \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix} = 0 \cdot v.
$$

Así que $\lambda = 0$ es autovalor con autovector $v = (1, 0)^t$.
****
**Ejemplo 3. La rotación 90°**
Sea $A = \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix} \in \mathbb{R}^{2 \times 2}$ (es una rotación de $90^\circ$).
¿Cuáles son los autovalores de $A$?
Supongamos $Av = \lambda v$ con $v = \begin{pmatrix} x_1 \\ x_2 \end{pmatrix} \neq 0$. Como $Av = \begin{pmatrix} -x_2 \\ x_1 \end{pmatrix}$, queda
$$
-x_2 = \lambda x_1, \quad x_1 = \lambda x_2.
$$
Sustituyendo la 1ra en la 2da: $x_1 = -\lambda^2 x_1$; y sustituyendo la 2da en la 1ra: $-x_2 = \lambda^2 x_2$.
Teniendo en cuenta que $v \neq 0$, resulta que $x_1$ o $x_2$ es no nulo, así que obtenemos que $\lambda^2 = -1$.
Es decir que no hay ningún $\lambda \in \mathbb{R}$ que pueda ser autovalor.
En cambio, si consideramos la misma $A$ sobre $\mathbb{C}^{2 \times 2}$, tanto $i$ como $-i$ son autovalores con respectivos autovectores $\begin{pmatrix} i \\ 1 \end{pmatrix}$ y $\begin{pmatrix} -i \\ 1 \end{pmatrix}$.
