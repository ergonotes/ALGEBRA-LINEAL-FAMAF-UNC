**Corolario.** Sea $V$ un espacio vectorial de dimensión finita sobre un cuerpo $\mathbb{K}$ y sea $\mathcal{B}$ una base ordenada de $V$.

Si $T, S \in \text{End}(V)$ (es decir, $T$ y $S$ son operadores lineales de $V$ en $V$), entonces la matriz de la composición respecto a la base $\mathcal{B}$ es el producto de sus respectivas matrices asociadas en dicha base.

Simbólicamente:

$$[S \circ T]_{\mathcal{B}} = [S]_{\mathcal{B}} \cdot [T]_{\mathcal{B}}$$
****
**Demostración.** Sea $V$ un espacio vectorial de dimensión $n$ con una base ordenada $\mathcal{B} = \{v_1, v_2, \dots, v_n\}$.

Sean $T: V \to V$ y $S: V \to V$ dos transformaciones lineales.

Definamos sus matrices asociadas para no arrastrar tanta notación:
Llamemos **$A$** a la matriz de $T$, es decir: $A = [T]_{\mathcal{B}}$. Sus componentes individuales serán $a_{ij}$.

Llamemos **$B$** a la matriz de $S$, es decir: $B = [S]_{\mathcal{B}}$. Sus componentes individuales serán $b_{ij}$.
La máquina $T$ transforma el vector $v_k$ así:
  $$T(v_k) = \sum_{j=1}^n a_{jk} v_j$$
La máquina $S$ transforma el vector $v_j$ así:
  $$S(v_j) = \sum_{i=1}^n b_{ij} v_i$$
Queremos encontrar la matriz de $S \circ T$. 

Metamos el vector genérico $v_k$ en la mega-máquina:

$$(S \circ T)(v_k) = S(T(v_k))$$

Sustituimos $T(v_k)$ por su receta:

$$= S\left( \sum_{j=1}^n a_{jk} v_j \right)$$

Como $S$ es una transformación lineal:

$$= \sum_{j=1}^n a_{jk} S(v_j)$$

Sustituimos $S(v_j)$:

$$= \sum_{j=1}^n a_{jk} \left( \sum_{i=1}^n b_{ij} v_i \right)$$

Juntamos los escalares ($b_{ij}$ y $a_{jk}$) y agrupamos todo en torno a los vectores de salida $v_i$:

$$= \sum_{i=1}^n \left( \sum_{j=1}^n b_{ij} a_{jk} \right) v_i$$

Veamos bien lo que nos quedó adentro del gran paréntesis:

$$\sum_{j=1}^n b_{ij} a_{jk}$$

Si desarrollamos esa suma para un $i$ y un $k$ específicos, se ve así:

$$b_{i1}a_{1k} + b_{i2}a_{2k} + \dots + b_{in}a_{nk}$$

**Es exactamente la definición de multiplicar la fila $i$ de la matriz $B$ por la columna $k$ de la matriz $A$**

Por lo tanto, el gran paréntesis es simplemente el número que se encuentra en la posición $(i, k)$ de la nueva matriz producto $B \cdot A$. Llamemos $c_{ik}$ a ese número. La ecuación nos queda:

$$(S \circ T)(v_k) = \sum_{i=1}^n c_{ik} v_i$$

Las coordenadas del destino del vector $v_k$ bajo la transformación $S \circ T$ son exactamente las columnas de la matriz obtenida al multiplicar $B \cdot A$.

Sustituyendo nuestras definiciones iniciales ($B = [S]_{\mathcal{B}}$ y $A = [T]_{\mathcal{B}}$):

$$[S \circ T]_{\mathcal{B}} = [S]_{\mathcal{B}} \cdot [T]_{\mathcal{B}} \quad \blacksquare$$

