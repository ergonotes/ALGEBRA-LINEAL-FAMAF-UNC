Matrices con diagonal estrictamente dominante

Supongamos que $A \in \mathbb{R}^{n \times n}$ es tal que:

$$
|A_{ii}| > \sum_{j \neq i} |A_{ij}|, \quad \forall i = 1, \dots, n.
$$

Entonces $A$ es invertible.

Supongamos que $AX = 0$ tiene una solución no trivial $(x_1, \dots, x_n)$. Tomemos $r$: $|x_r| \ge |x_i|$, para todo $i$. Con lo cual $|x_r| > 0$.

Como $(x_1, \dots, x_n)$ es solución del sistema $AX = 0$, por la desigualdad triangular:

$$
|A_{rr}x_r| = \left| \sum_{j \neq r} -A_{rj}x_j \right| \le \sum_{j \neq r} |A_{rj}||x_j| \le \left( \sum_{j \neq r} |A_{rj}| \right) |x_r| < |A_{rr}||x_r|.
$$

De donde: $|A_{rr}| < |A_{rr}|$, lo cual es una contradicción.