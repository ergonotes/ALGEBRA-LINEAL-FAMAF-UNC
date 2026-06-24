Sea $V$ un espacio vectorial sobre un cuerpo $\mathbb{K}$ de dimensión finita. Sean $\mathcal{B}$ y $\mathcal{B}'$ dos bases ordenadas de $V$. Entonces, para todo vector $v \in V$, se cumple la siguiente relación de coordenadas:

$$[v]_{\mathcal{B}'} = [\text{Id}_V]_{\mathcal{B}\mathcal{B}'} [v]_{\mathcal{B}}$$

Donde $\text{Id}_V : V \to V$ es la transformación identidad (definida como $\text{Id}_V(v) = v$ para todo $v \in V$), y a la matriz $[\text{Id}_V]_{\mathcal{B}\mathcal{B}'}$ se le llama **Matriz de Cambio de Base** (o matriz de transición) de la base $\mathcal{B}$ a la base $\mathcal{B}'$.
****
**Demostración.**
Ya que [[D-Aplicar una transformación abstracta en cualquier base del universo es exactamente lo mismo que multiplicar la matriz de la transformación por las coordenadas del vector]], sabemos que para cualquier transformación lineal $T: V \to W$ y bases ordenadas $\mathcal{B}$ (de $V$) y $\mathcal{B}'$ (de $W$), se cumple:
$$[T]_{\mathcal{B}\mathcal{B}'}[v]_{\mathcal{B}} = [T(v)]_{\mathcal{B}'}$$
Consideremos el caso particular donde el espacio de llegada es el mismo que el de partida ($W = V$), y la transformación lineal es la función identidad $T = \text{Id}_V$. Sustituimos esta $T$ en nuestra fórmula general:
$$[\text{Id}_V]_{\mathcal{B}\mathcal{B}'}[v]_{\mathcal{B}} = [\text{Id}_V(v)]_{\mathcal{B}'}$$
Por la definición fundamental de la transformación identidad, sabemos que no altera al vector que recibe, es decir, $\text{Id}_V(v) = v$. Reemplazamos el lado derecho de la ecuación:
$$[\text{Id}_V]_{\mathcal{B}\mathcal{B}'}[v]_{\mathcal{B}} = [v]_{\mathcal{B}'} \quad \blacksquare$$
