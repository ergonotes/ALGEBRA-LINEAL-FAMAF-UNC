**Corolario**. Si $W$ es un subespacio propio de un espacio vectorial de dimensión finita $V$, entonces $W$ es de dimensión finita y $\dim W < \dim V$.
****
**Demostración**. Si $W = \{0\}$, entonces $\dim W = 0$, como $W \subsetneq V$, tenemos que $V$ es no nulo y por lo tanto $\dim W = 0 < \dim V$.
Si $W \neq \{0\}$, sea $w \in W$, $w \neq 0$. Por el teorema anterior existe una base $\mathcal{B}$ de $W$ que contiene a $w$. Como $\mathcal{B}$ es un conjunto LI en $W$, lo es también en $V$ y debido a que [[D-Un espacio construido con x vectores no puede contener más de x direcciones independientes]], $\dim W = |\mathcal{B}| \le \dim V$.
Como $W$ es un subespacio propio de $V$ existe un vector $v$ en $V$ que no está en $W$. Agregando $v$ a cualquier base de $W$ se obtiene un subconjunto linealmente independiente de $V$ (lema anterior). Así, $\dim W < \dim V$. $\square$

(Cabe aclarar que cuando usamos el término "propio" para describir un subespacio, nos referimos a que un **subespacio propio** $W$ de un espacio vectorial $V$ es aquel que está contenido dentro de $V$, pero que **es estrictamente más pequeño que $V$**).