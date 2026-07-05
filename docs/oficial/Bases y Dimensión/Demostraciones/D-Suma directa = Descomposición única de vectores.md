**Proposición**. Sea $V$ espacio vectorial y $V_1, V_2$ subespacios vectoriales de $V$. Entonces, $V = V_1 \oplus V_2$ si y sólo si para todo vector $v \in V$ existe únicos $v_1 \in V_1, v_2 \in V_2$ tal que $v = v_1 + v_2$.
****
**Demostración**.
($\Rightarrow$) Sea $v \in V$, como $V = V_1 + V_2$, existen $v_1 \in V_1, v_2 \in V_2$ tal que $v = v_1 + v_2$. Veamos que $v_1$ y $v_2$ son únicos. Sean $v_1' \in V_1, v_2' \in V_2$ tal que $v = v_1' + v_2'$. Por lo tanto $v_1 + v_2 = v_1' + v_2'$. Haciendo pasajes de término obtenemos
$$
v_1 - v_1' = v_2' - v_2.
$$
Sea $v_0 = v_1 - v_1' = v_2' - v_2$. Ahora bien, $v_1 - v_1' \in V_1$, por lo tanto $v_0 = v_1 - v_1' \in V_1$. Análogamente, $v_2' - v_2 \in V_2$, por lo tanto $v_0 = v_2' - v_2 \in V_2$. Es decir, $v_0 \in V_1 \cap V_2 = 0$, luego $v_0 = 0$, por lo tanto $v_1 = v_1'$ y $v_2 = v_2'$.

($\Leftarrow$) Es claro que $V = V_1 + V_2$. Probemos que $V_1 \cap V_2 = 0$. Sea $v \in V_1 \cap V_2$. Por hipótesis, existe únicos $v_1 \in V_1, v_2 \in V_2$ tal que $v = v_1 + v_2$. Podemos escribir entonces
$$
\begin{aligned}
v &= v_1 + v_2, \quad & v_1 \in V_1, \quad & v_2 \in V_2 \\
v &= v + 0, \quad & v \in V_1, \quad & 0 \in V_2 \\
v &= 0 + v, \quad & 0 \in V_1, \quad & v \in V_2.
\end{aligned}
$$
Por la unicidad, resulta que $v_1 = v = 0$ y $v_2 = 0 = v$, es decir $v = 0$. $\square$