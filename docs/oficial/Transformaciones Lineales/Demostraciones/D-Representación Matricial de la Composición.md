**Teorema.** Sean $V, W$ y $Z$ espacios vectoriales de dimensión finita sobre un mismo cuerpo $\mathbb{K}$.

Sean $\mathcal{B}, \mathcal{B}'$ y $\mathcal{B}''$ bases ordenadas de $V, W$ y $Z$, respectivamente.

Si $T: V \to W$ y $S: W \to Z$ son transformaciones lineales, entonces la matriz asociada a la transformación composición $S \circ T: V \to Z$ respecto de las bases $\mathcal{B}$ y $\mathcal{B}''$ es igual al producto de la matriz asociada a $S$ (respecto de $\mathcal{B}'$ y $\mathcal{B}''$) por la matriz asociada a $T$ (respecto de $\mathcal{B}$ y $\mathcal{B}'$).
Simbólicamente:   $$[S \circ T]_{\mathcal{B}\mathcal{B}''} = [S]_{\mathcal{B}'\mathcal{B}''} \cdot [T]_{\mathcal{B}\mathcal{B}'}$$
****
**Demostración.**
- Sea $\dim V = n$, con base $\mathcal{B} = \{v_1, \dots, v_n\}$.

- Sea $\dim W = m$, con base $\mathcal{B}' = \{w_1, \dots, w_m\}$.

- Sea $\dim Z = p$, con base $\mathcal{B}'' = \{z_1, \dots, z_p\}$.

Llamemos **$A$** a la matriz $[T]_{\mathcal{B}\mathcal{B}'}$. Esta matriz es de tamaño $m \times n$.
Por definición, al meter el vector $v_k$ en $T$, el resultado se escribe usando la base de $W$:

$$T(v_k) = \sum_{j=1}^m a_{jk} w_j$$

Llamemos **$B$** a la matriz $[S]_{\mathcal{B}'\mathcal{B}''}$. Esta matriz es de tamaño $p \times m$.

Por definición, al meter el vector $w_j$ en $S$, el resultado se escribe usando la base de $Z$:

$$S(w_j) = \sum_{i=1}^p b_{ij} z_i$$

Queremos hallar la matriz de la composición $S \circ T$. La regla no cambia: evaluamos la máquina en el vector $k$-ésimo de la base de entrada ($v_k$):

$$(S \circ T)(v_k) = S(T(v_k))$$

Sustituimos $T(v_k)$ por su sumatoria:

$$= S\left( \sum_{j=1}^m a_{jk} w_j \right)$$

Como $S$ es lineal, extrae las sumas y los escalares $a_{jk}$:

$$= \sum_{j=1}^m a_{jk} S(w_j)$$

Sustituimos $S(w_j)$ por su sumatoria en el universo $Z$:

$$= \sum_{j=1}^m a_{jk} \left( \sum_{i=1}^p b_{ij} z_i \right)$$


Agrupamos los escalares y reordenamos las sumatorias, sacando como factor común a los vectores finales de la base $Z$ ($z_i$).

$$= \sum_{i=1}^p \left( \sum_{j=1}^m b_{ij} a_{jk} \right) z_i$$

Observamos el gran bloque de escalares dentro del paréntesis:

$$c_{ik} = \sum_{j=1}^m b_{ij} a_{jk}$$

Esta es la definición universal del producto de matrices. Representa exactamente el número que va en la fila $i$, columna $k$ al multiplicar una matriz $B$ (de tamaño $p \times m$) por una matriz $A$ (de tamaño $m \times n$).

El límite de la suma interna ($j=1$ hasta $m$) demuestra por qué el número de columnas de la primera matriz debe ser idéntico al número de filas de la segunda matriz para que se puedan multiplicar.

Por lo tanto, la matriz que genera los coeficientes de $(S \circ T)$ es exactamente la matriz producto $B \cdot A$:

$$[S \circ T]_{\mathcal{B}\mathcal{B}''} = [S]_{\mathcal{B}'\mathcal{B}''} \cdot [T]_{\mathcal{B}\mathcal{B}'} \quad \blacksquare$$