**Teorema.** Sea $V$ un espacio vectorial sobre $\mathbb{R}$ provisto de un producto interno. Si $\beta$ y $\beta'$ son dos bases ortonormales (BON) de $V$, entonces la matriz de cambio de base $P$ de $\beta$ a $\beta'$ satisface que:

$$P^{-1} = P^t$$
****
**Demostración.**
Consideremos la transformación lineal Identidad $Id: V \to V$.

La matriz de cambio de base de $\beta$ a $\beta'$ no es otra cosa que la matriz asociada a la transformación identidad tomando $\beta$ como base de entrada y $\beta'$ como base de salida. La llamaremos $P$:

$$P = [Id]_{\beta'}^{\beta}$$

Por propiedades básicas de las matrices de cambio de base, sabemos que [[D-Toda matriz de transición entre dos bases de un espacio de dimensión finita es invertible, y su inversa equivale a la inversión geométrica del sentido del cambio de base]]. En notación:

$$P^{-1} = [Id]_{\beta}^{\beta'}$$

Ahora, por [[D-Propiedades del Operador Adjunto]]. Sabemos que el operador adjunto de la identidad es la identidad misma ($(Id)^* = Id$).

Por lo tanto, podemos reescribir nuestra matriz $P^{-1}$:

$$[Id]_{\beta}^{\beta'} = [Id^*]_{\beta}^{\beta'}$$

Y, por la [[D-Representación Matricial del Operador Adjunto]], tenemos $[T^*]_{\beta}^{\beta'} = ([T]_{\beta'}^{\beta})^t$.

Aplicando esta regla a nuestro operador $Id^*$:

$$[Id]_{\beta}^{\beta'} = [Id^*]_{\beta}^{\beta'} = ([Id]_{\beta'}^{\beta})^t$$

Igualando ambos extremos, llegamos a la conclusión directa:

$$P^{-1} = P^t$$

