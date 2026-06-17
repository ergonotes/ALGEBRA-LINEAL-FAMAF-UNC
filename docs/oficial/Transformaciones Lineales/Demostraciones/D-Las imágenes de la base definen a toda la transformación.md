**Teorema.** Sea $V$ un espacio vectorial de dimensión finita sobre el cuerpo $F$, sea $\{\alpha_1, \dots, \alpha_n\}$ una base ordenada de $V$. Sean $W$ un espacio vectorial sobre el mismo cuerpo $F$ y $\beta_1, \dots, \beta_n$ vectores cualesquiera de $W$. Entonces existe una única transformación lineal $T$ de $V$ en $W$ tal que
$$
T\alpha_j = \beta_j, \quad j = 1, \dots, n.
$$
****
**Demostración.** Para demostrar que existe una transformación lineal $T$ tal que $T\alpha_j = \beta_j$ se procede como sigue. Dado $\alpha$ de $V$, existe una única $n$-tuple $(x_1, \dots, x_n)$ tal que
$$
\alpha = x_1\alpha_1 + \dots + x_n\alpha_n.
$$
Para ese vector $\alpha$ se define
$$
T\alpha = x_1\beta_1 + \dots + x_n\beta_n.
$$
Entonces, $T$ es una correspondencia bien definida que asocia a cada vector $\alpha$ de $V$ un vector $T\alpha$ de $W$. De la definición queda claro que $T\alpha_j = \beta_j$ para cada $j$. Para ver que $T$ es lineal, sea
$$
\beta = y_1\alpha_1 + \dots + y_n\alpha_n
$$
de $V$ y sea $c$ cualquier escalar. Ahora
$$
c\alpha + \beta = (cx_1 + y_1)\alpha_1 + \dots + (cx_n + y_n)\alpha_n
$$
con lo que, por definición,
$$
T(c\alpha + \beta) = (cx_1 + y_1)\beta_1 + \dots + (cx_n + y_n)\beta_n.
$$
Por otra parte,
$$
\begin{aligned}
c(T\alpha) + T\beta &= c \sum_{i=1}^n x_i\beta_i + \sum_{i=1}^n y_i\beta_i \\
&= \sum_{i=1}^n (cx_i + y_i)\beta_i
\end{aligned}
$$
Y así
$$
T(c\alpha + \beta) = c(T\alpha) + T\beta.
$$
Si $U$ es una transformación lineal de $V$ en $W$ con $U\alpha_j = \beta_j$, $j = 1, \dots, n$, entonces para el vector $\alpha = \sum_{i=1}^n x_i\alpha_i$ se tiene
$$
\begin{aligned}
U\alpha &= U\left( \sum_{i=1}^n x_i\alpha_i \right) \\
&= \sum_{i=1}^n x_i(U\alpha_i) \\
&= \sum_{i=1}^n x_i\beta_i
\end{aligned}
$$
con lo que $U$ es exactamente la misma correspondencia $T$ que se definió antes, lo que demuestra que la transformación lineal $T$ con $T\alpha_j = \beta_j$ es única. $\blacksquare$