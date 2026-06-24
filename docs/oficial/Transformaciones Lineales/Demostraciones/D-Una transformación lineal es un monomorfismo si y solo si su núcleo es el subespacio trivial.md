**Proposición**. Sea $T: V \to W$ una transformación lineal. Entonces $T$ es monomorfismo si y sólo si $\text{Nu}(T) = 0$.
****
**Demostración**. 
($\Rightarrow$) Debemos ver que $\text{Nu}(T) = 0$, es decir que si $T(v) = 0$, entonces $v = 0$. Ahora bien, si $T(v) = 0$, como $T(0) = 0$, tenemos que $T(v) = T(0)$, y como $T$ es inyectiva, implica que $v = 0$.
($\Leftarrow$) Sean $v_1, v_2 \in V$ tal que $T(v_1) = T(v_2)$. Entonces
$$
0 = T(v_1) - T(v_2) = T(v_1 - v_2).
$$
Por lo tanto, $v_1 - v_2 \in \text{Nu}(T)$. Por hipótesis, tenemos que $v_1 - v_2 = 0$, es decir $v_1 = v_2$. $\square$