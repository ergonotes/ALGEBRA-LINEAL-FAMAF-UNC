**Teorema.** Sean $V$ y $W$ espacios vectoriales sobre $\mathbb{R}$ provistos de un producto interno. Sean $\beta = \{u_1, \dots, u_n\}$ y $\beta' = \{w_1, \dots, w_m\}$ **bases ortonormales** de $V$ y $W$ respectivamente.

Sea $T: V \to W$ una transformación lineal y sea $A = [T]_{\beta}^{\beta'}$ su matriz asociada en dichas bases.

Entonces, la matriz del operador adjunto $T^*: W \to V$ en las bases $\beta'$ y $\beta$ es exactamente la matriz traspuesta de $A$. Es decir:

$$[T^*]_{\beta'}^{\beta} = A^t$$
****
**Demostración**.
Llamemos $A = [T]_{\beta}^{\beta'}$ a la matriz original. Por definición de matriz asociada a una transformación lineal, la columna $i$-ésima de $A$ contiene las coordenadas del vector $T(u_i)$. Por lo tanto, podemos escribir:

$$T(u_i) = \sum_{k=1}^m A_{ki} w_k$$

Llamemos $B = [T^*]_{\beta'}^{\beta}$ a la matriz del operador adjunto. De la misma manera, su columna $j$-ésima contiene las coordenadas de $T^*(w_j)$, por lo que:

$$T^*(w_j) = \sum_{r=1}^n B_{rj} u_r$$

Tomemos la expresión que acabamos de armar para $T^*(w_j)$ y hagamos el producto interno contra un vector genérico $u_i$ de la base $\beta$:

$$\langle T^*(w_j), u_i \rangle = \left\langle \sum_{r=1}^n B_{rj} u_r \, , \, u_i \right\rangle$$

Por linealidad, sacamos la sumatoria y los escalares afuera:

$$\langle T^*(w_j), u_i \rangle = \sum_{r=1}^n B_{rj} \langle u_r, u_i \rangle$$

Aquí ocurre la magia de la hipótesis: **$\beta$ es una base ortonormal**. Esto significa que $\langle u_r, u_i \rangle = 0$ siempre que $r \neq i$, y vale $1$ únicamente cuando $r = i$. Toda la sumatoria desaparece y solo sobrevive el término donde $r=i$:

$$\langle T^*(w_j), u_i \rangle = B_{ij}$$

Ahora calcularemos el producto interno equivalente del lado de $T$. Tomemos $T(u_i)$ y hagamos producto interno con $w_j$:

$$\langle w_j, T(u_i) \rangle = \left\langle w_j \, , \, \sum_{k=1}^m A_{ki} w_k \right\rangle$$

Sacamos escalares y sumatoria por linealidad en la segunda componente:

$$\langle w_j, T(u_i) \rangle = \sum_{k=1}^m A_{ki} \langle w_j, w_k \rangle$$

Nuevamente, como **$\beta'$ es una base ortonormal**, $\langle w_j, w_k \rangle$ se anula para todo $k \neq j$ y vale $1$ solo cuando $k=j$:

$$\langle w_j, T(u_i) \rangle = A_{ji}$$

Por la definición teórica del operador adjunto, sabemos que para cualquier par de vectores se cumple rigurosamente que:

$$\langle T^*(w_j), u_i \rangle = \langle w_j, T(u_i) \rangle$$

Si sustituimos los resultados, llegamos a que:

$$B_{ij} = A_{ji}$$

Esto significa que el elemento en la fila $i$, columna $j$ de la matriz $B$, es exactamente el mismo número que está en la fila $j$, columna $i$ de la matriz $A$. Por definición, esto significa que $B$ es la matriz traspuesta de $A$:

$$B = A^t$$
