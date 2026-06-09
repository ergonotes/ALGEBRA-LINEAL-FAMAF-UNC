**Definición 1.0.0** Se dice que la matriz $E$ de orden $n$ es una matriz elemental si ella puede obtenerse, a partir de la matriz identidad $I_n$, realizando en esta una operación elemental.
La matriz
$$
\begin{bmatrix}
1 & 0 & 3 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$
es una matriz elemental, pues se obtuvo partiendo de $I_3$, sustituyendo en esta su primera línea por ella misma más tres veces su tercera línea.
A partir de esta definición, podemos intuir los **[[Tipos de Matrices Elementales]]**, según cada operación elemental.
****
#### **Teorema 1.1.0** Sea $e$ una operación elemental por fila y sea $E$ la matriz elemental $E=e(I)$ entonces $e(A)=EA$.
[[D-Cualquier operación elemental de fila sobre una matriz equivale a multiplicar esa matriz por una matriz elemental a la izquierda]].
****
#### **Corolario 1.1.1** Sean $A$ y $B$ matrices $m \times n$. Entonces $B$ es equivalente por filas a $A$ si y sólo si $B=PA$ donde $P$ es producto de matrices elementales. 
Más aún, si $B= c_k(e_{k-1}(\cdots(e_1(A))\cdots)$ con $e_1, e_2, \dots, e_k$ operaciones elementales de fila y $E_i = e_i(I)$ para  $i = 1, \dots, k,$ entonces $B = E_k E_{k-1} \cdots E_1 A$.
[[D-Dos matrices son equivalentes por filas si y solo si una se puede obtener multiplicando la otra por la izquierda por un producto de matrices elementales]]
