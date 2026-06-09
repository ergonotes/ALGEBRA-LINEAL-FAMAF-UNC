**Proposición**. Si $S \subseteq V$ con $S \neq \emptyset$, entonces $\langle S \rangle$ es un subespacio de $V$.
****
**Demostración**.
Como $S \neq \emptyset$, existe al menos un $v \in S$. Como $1 \cdot v = v$, sabemos que $v \in \langle S \rangle$, por lo que $\langle S \rangle \neq \emptyset$.
Ahora veamos el criterio unificado $(u + \alpha w \in \langle S \rangle)$:
Sean $u, w \in \langle S \rangle$ y un escalar cualquiera $\alpha \in K$.
Por definición de espacio generado, ambos vectores se pueden escribir como sumatorias finitas de elementos de $S$:
$$ u = \sum_{i=1}^{n} \lambda_i x_i \quad y \quad w = \sum_{j=1}^{m} \mu_j y_j $$
(Donde $\lambda_i, \mu_j \in K$ y $x_i, y_j \in S$).
Evaluamos la expresión $u + \alpha w$:
$$ u + \alpha w = \sum_{i=1}^{n} \lambda_i x_i + \alpha \left( \sum_{j=1}^{m} \mu_j y_j \right) $$
Introducimos el escalar $\alpha$ dentro de la segunda sumatoria:
$$ u + \alpha w = \sum_{i=1}^{n} \lambda_i x_i + \sum_{j=1}^{m} (\alpha \mu_j) y_j $$
La expresión resultante es la suma de dos combinaciones lineales, lo que genera una única y gran combinación lineal de $n + m$ términos construida exclusivamente con vectores de $S$ y escalares de $K$. Esto implica que:
$$ u + \alpha w \in \langle S \rangle $$