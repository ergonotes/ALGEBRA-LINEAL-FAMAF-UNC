Antes de ver la demostración de forma general, se recomienda ver el ejemplo para casos $2 \times 2$. [[E-Teorema del Determinante respecto a Operaciones Elementales en 2x2]].

**Teorema**. Sea $A \in M_n(\mathbb{K})$ y sean $1 \le r, s \le n$.

1) Sea $c \in \mathbb{K}$ y $B$ la matriz que se obtiene de $A$ multiplicando la fila $r$ por $c$, es decir $A \xrightarrow{cF_r} B$, entonces $\det B = c \det A$.

2) Sea $c \in \mathbb{K}$, $r \neq s$ y $B$ la matriz que se obtiene de $A$ sumando a la fila $r$ la fila $s$ multiplicada por $c$, es decir $A \xrightarrow{F_r+cF_s} B$, entonces $\det B = \det A$.

3) Sea $r \neq s$ y sea $B$ la matriz que se obtiene de $A$ permutando la fila $r$ con la fila $s$, es decir $A \xrightarrow{F_r \leftrightarrow F_s} B$, entonces $\det B = -\det A$.
****
No contento con haber visto el primer ejemplo para $2 \times 2$, también se recomienda ver el ejemplo de [[E-Teorema del Determinante respecto a Operaciones Elementales en 3x3]], para entender la siguiente demostración general. 

**Demostración.** El desarrollo de Laplace es exactamente la generalización de la fórmula explícita del caso $2\times 2$. La idea clave es:

$$\det A = \sum_{j=1}^n a_{rj}, C_{rj}$$

donde el **cofactor** $C_{rj} = (-1)^{r+j}M_{rj}$ **no depende de las entradas de la fila $r$**.

---

### Caso 1. $A \xrightarrow{cF_r} B$

Las entradas de la fila $r$ de $B$ son $b_{rj} = ca_{rj}$. Las demás filas no cambian, por lo que $C_{rj}^B = C_{rj}^A$. Entonces:

$$\det B = \sum_j (ca_{rj}),C_{rj} = c\sum_j a_{rj},C_{rj} = c\det A \quad \blacksquare$$

---

### Caso 3. $A \xrightarrow{F_r \leftrightarrow F_s} B$ (por inducción sobre $n$)

**Caso base** $n=2$: ya demostrado directamente.

**Paso inductivo:** Suponemos el resultado válido para matrices $(n-1)\times(n-1)$. Como $r\neq s$, elegimos una fila $k$ con $k\neq r, s$ (posible para $n\geq 3$) y desarrollamos por esa fila:

$$\det B = \sum_j b_{kj},(-1)^{k+j}M_{kj}^B$$

Como $k\neq r, s$: $b_{kj} = a_{kj}$. Además, el menor $M_{kj}^B$ es el determinante de una submatriz $(n-1)\times(n-1)$ que coincide con la de $A$ salvo que sus filas $r$ y $s$ están permutadas. Por la **hipótesis inductiva**:

$$M_{kj}^B = -M_{kj}^A$$

Por lo tanto:

$$\det B = \sum_j a_{kj},(-1)^{k+j},(-M_{kj}^A) = -\det A \quad \blacksquare$$

> **Corolario.** Si $A$ tiene dos filas iguales, $\det A = 0$. _Prueba:_ permutar esas dos filas da la misma matriz, luego $\det A = -\det A$, así que $\det A = 0$.

---

### Caso 2. $A \xrightarrow{F_r + cF_s} B$

Las entradas de la fila $r$ de $B$ son $b_{rj} = a_{rj} + ca_{sj}$, y las demás filas no cambian, así que $C_{rj}^B = C_{rj}^A$. Desarrollando por la fila $r$:

$$\det B = \sum_j(a_{rj} + ca_{sj}),C_{rj} = \underbrace{\sum_j a_{rj},C_{rj}}_{\det A} + c\underbrace{\sum_j a_{sj},C_{rj}}_{D}$$

$D$ es exactamente el determinante de la matriz $A'$ obtenida reemplazando la fila $r$ de $A$ por la fila $s$. Como $A'$ tiene las filas $r$ y $s$ iguales, por el corolario:

$$D = \det A' = 0$$

Por lo tanto $\det B = \det A \quad \blacksquare$



