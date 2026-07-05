**Corolario**. Sea $A$ una matriz $n \times n$ sobre el cuerpo $K$ y supongamos que los vectores fila de $A$ forman un conjunto L.I. de vectores de $K^n$. Entonces $A$ es invertible.
****
**Demostración.** Sean $v_1, \dots, v_n$ los vectores fila de $A$, $v_i = (A_{i1}, \dots, A_{in})$.
Sea
$$
W = \langle v_1, \dots, v_n \rangle \subset K^n.
$$
Sabemos que $\{v_1, \dots, v_n\}$ es un conjunto L.I. y genera $W$ entonces
$$
\dim W = n = \dim K^n,
$$
por lo tanto $W$ no es propio, es decir, $W = K^n$.
Sea $e_i$ el $i$-ésimo vector de la base canónica de $K^n$, $e_i = (0, \dots, 1, \dots, 0)$. $\Rightarrow \exists$ escalares $B_{ij} \in K$ tales que
$$
e_i = \sum_{j=1}^n B_{ij} v_j.
$$
donde $\{e_1, e_2, \dots, e_n\}$ es la base canónica de $F^n$. Así, para la matriz $B$ de elementos $B_{ij}$ se tiene
$$
BA = I. \ \square
$$