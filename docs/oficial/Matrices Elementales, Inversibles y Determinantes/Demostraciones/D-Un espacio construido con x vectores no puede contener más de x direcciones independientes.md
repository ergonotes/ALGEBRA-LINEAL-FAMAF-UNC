**TEOREMA**. Sea $V$ un espacio vectorial generado por un conjunto finito de vectores $w_1, \dots, w_m$. Entonces todo conjunto independiente de vectores de $V$ es finito y contiene a lo más $m$ elementos.
****
**Demostración**. Para demostrar este teorema es suficiente ver que todo subconjunto $S$ de $V$ que contiene más de $m$ vectores es linealmente dependiente. 
Sea $S$ un tal conjunto. En $S$ hay vectores diferentes $\alpha_1, \alpha_2, \dots, \alpha_n$, donde $n > m$. 
Como $\beta_1, \dots, \beta_m$ generan $V$, existen escalares $A_{ij}$ en $F$ tales que
$$
\alpha_j = \sum_{i=1}^m A_{ij}\beta_i.
$$
Para cualesquiera $n$ escalares $x_1, x_2, \dots, x_n$, se tiene
$$
\begin{aligned}
x_1\alpha_1 + \dots + x_n\alpha_n &= \sum_{j=1}^n x_j\alpha_j \\
&= \sum_{j=1}^n x_j \sum_{i=1}^m A_{ij}\beta_i \\
&= \sum_{j=1}^n \sum_{i=1}^m (A_{ij}x_j)\beta_i \\
&= \sum_{i=1}^m \left( \sum_{j=1}^n A_{ij}x_j \right)\beta_i.
\end{aligned}
$$
Como $n > m$, y sabemos que **[[1.2.3.D-Siempre que un sistema homogéneo tenga menos ecuaciones que incógnitas, existe una solución distinta de cero]]**, implica que existen escalares $x_1, x_2, \dots, x_n$, no todos $0$, tales que
$$
\sum_{j=1}^n A_{ij}x_j = 0, \quad 1 \le i \le m.
$$
Luego $x_1\alpha_1 + x_2\alpha_2 + \dots + x_n\alpha_n = 0$. Ello demuestra que $S$ es un conjunto linealmente dependiente. $\blacksquare$
****
Es interesante ver que para la demostración se toma $x_1, x_2, \dots, x_n$ como escalares cualquiera al principio, para luego pasar a ser incógnitas de un sistema de ecuaciones. 