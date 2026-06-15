**Proposición.** Sea $V$ un espacio vectorial, y sea $\mathcal{B} = \{w_1, \dots, w_n\}$ una base (finita) de $V$. Entonces para todo $v \in V$ existen únicos escalares $a_1, \dots, a_n$ tales que
$$
v = a_1w_1 + \cdots + a_nw_n \quad \text{(de manera única).}
$$
****
**Demostración**. Como $\langle w_1, \dots, w_n \rangle = V$, todo $v \in V$ es combinación lineal de $w_1, \dots, w_n$, es decir, existen $a_1, \dots, a_n$ tales que $v = \sum_{j=1}^n a_j w_j$.

*Unicidad:* Si $v = a_1w_1 + \cdots + a_nw_n = b_1w_1 + \cdots + b_nw_n$, entonces
$$
0 = v - v = (a_1 - b_1)w_1 + \cdots + (a_n - b_n)w_n.
$$

Como $\{w_i\}$ es L.I., $\Rightarrow a_i - b_i = 0$ para todo $i$, es decir, son únicos. $\square$