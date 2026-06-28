 $(\Rightarrow)$ Si $B$ es equivalente por filas a $A$ existen operaciones elementales $e_1, \dots, e_k$ tal que $B = e_k(e_{k-1}(\cdots(e_1(A))\cdots))$, más formalmente, si $A_i = e_1(A)$ y $A_i = e_i(A_{i-1}$ para $i = 2, \dots, k$, entonces $e_k(A_{k-1}) = B$.
Sea E_i = e_i(I_m), entonces, por el teorema anterior ([[D-Cualquier operación elemental de fila sobre una matriz equivale a multiplicar esa matriz por una matriz elemental a la izquierda]]) $A_1 = E_1 A$ y $A_i = E_i A_{i-1} (i = 2, \dots, k)$.
Por lo tanto $B = E_k A_{k-1}$, en otras palabras $B = E_k E_{k-1} \cdots E_1 A$, luego $P = E_k E_{k-1} \cdots E_1$.

$(\Leftarrow)$ Si $B = PA$, con $P = E_k E_{k-1} \cdots E_1$ donde $E_i = e_i(I_m)$ es una matriz elemental, entonces $B = PA = E_k E_{k-1} \cdots E_1 A \stackrel{\text{Teorema anterior}}{=} e_k(e_{k-1}(\cdots(e_1(A))\cdots))$.
Por lo tanto, $B$ es equivalente por filas a $A$.
