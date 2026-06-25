**Proposición.** Sean $V, W$ y $Z$ espacios vectoriales sobre el mismo cuerpo $\mathbb{K}$. Si $T: V \to W$ y $S: W \to Z$ son transformaciones lineales, entonces la función compuesta $S \circ T: V \to Z$, definida como $(S \circ T)(v) = S(T(v))$ para todo $v \in V$, es también una transformación lineal.
****
**Demostración.** Tomamos dos vectores genéricos $u, v \in V$. Evaluamos la composición en su suma:

$$(S \circ T)(u + v) = S(T(u + v))$$

Como sabemos por hipótesis que la máquina de adentro ($T$) es lineal, esta separa la suma internamente:

$$= S(T(u) + T(v))$$

Ahora, notemos que $T(u)$ y $T(v)$ son simplemente dos vectores que viven en el espacio intermedio $W$. Como la máquina de afuera ($S$) también es lineal por hipótesis, sabe separar la suma de los vectores que recibe:

$$= S(T(u)) + S(T(v))$$

Finalmente, reescribimos usando la notación de composición para cerrar la igualdad:

$$= (S \circ T)(u) + (S \circ T)(v) \quad \blacksquare$$


Luego tomamos un vector genérico $v \in V$ y un escalar cualquiera $c \in \mathbb{K}$.

$$(S \circ T)(c v) = S(T(c v))$$

Como $T$ es lineal, permite extraer el escalar $c$ hacia afuera de su propia función:

$$= S(c T(v))$$

Nuevamente, $T(v)$ es un vector en $W$. Como $S$ es lineal, el escalar $c$ sigue su camino y sale también hacia el exterior de la segunda máquina:

$$= c S(T(v))$$

Reescribimos con la notación de composición:

$$= c (S \circ T)(v) \quad \blacksquare$$

