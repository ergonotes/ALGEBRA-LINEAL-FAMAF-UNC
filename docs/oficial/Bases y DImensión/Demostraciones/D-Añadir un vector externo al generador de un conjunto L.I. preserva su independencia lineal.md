**Lema.** Sea $S$ un subconjunto L.I. de un espacio vectorial $V$. Supongamos que $w \in V$ no pertenece al subespacio generado por $S$. Entonces $S \cup \{w\}$ es L.I.
****
**Demostración**. Sea $v_1, \dots, v_m \in S$ vectores distintos. Supongamos que
$$
c_1v_1 + \cdots + c_mv_m + c \cdot w = 0.
$$

Si $c \neq 0 \Rightarrow w = \left(-\frac{c_1}{c}\right)v_1 + \cdots + \left(-\frac{c_m}{c}\right)v_m$, luego $w \in \langle S \rangle$. Absurdo. Por lo tanto $c = 0$.
Entonces
$$
c_1v_1 + \cdots + c_mv_m = 0,
$$
como $\{v_1, \dots, v_m\} \subseteq S$ es L.I. resulta $c_1 = \cdots = c_m = 0$.
Es decir que obtenemos
$$
c = 0 \text{ y } c_1 = \cdots = c_m = 0,
$$
lo que implica que $S \cup \{w\}$ es L.I. $\square$