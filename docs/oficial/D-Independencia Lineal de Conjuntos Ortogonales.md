**Teorema.** Sea $V$ un espacio vectorial sobre $\mathbb{R}$ provisto de un producto interno. Si $X \subseteq V$ es un conjunto ortogonal de vectores no nulos, entonces $X$ es un conjunto linealmente independiente.
****
**Demostración.**
Para demostrar que un conjunto es linealmente independiente, tomamos una cantidad finita de vectores del conjunto $X$, digamos $v_1, v_2, \dots, v_k \in X$, y planteamos una combinación lineal igualada al vector nulo:

$$ a_1 v_1 + a_2 v_2 + \dots + a_k v_k = 0 $$

Nuestro objetivo es demostrar que la única forma de que esta igualdad se cumpla es que la combinación sea trivial, es decir, que todos los escalares ($a_1, a_2, \dots, a_k$) sean estrictamente cero.

Por ser $X$ un conjunto ortogonal formado por vectores no nulos, sabemos dos cosas fundamentales para cualquier par de índices $i, j$:

1. **Ortogonalidad:** $\langle v_i, v_j \rangle = 0$ siempre que $i \neq j$.
    
2. **Vectores no nulos:** $\langle v_j, v_j \rangle \neq 0$.

Elegimos un vector cualquiera de nuestra combinación, digamos $v_j$ (para algún $j$ entre $1$ y $k$), y tomamos el producto interno con $v_j$ a ambos lados de nuestra ecuación:

$$ \langle a_1 v_1 + a_2 v_2 + \dots + a_k v_k , v_j \rangle = \langle 0, v_j \rangle $$

$$ \langle a_1 v_1 + a_2 v_2 + \dots + a_k v_k , v_j \rangle = 0 $$

Aplicamos la propiedad de linealidad en la primera componente para separar la gran suma en productos internos individuales, sacando los escalares hacia afuera:

$$ a_1 \langle v_1, v_j \rangle + a_2 \langle v_2, v_j \rangle + \dots + a_j \langle v_j, v_j \rangle + \dots + a_k \langle v_k, v_j \rangle = 0 $$

Como todos los vectores distintos son ortogonales, cualquier producto interno $\langle v_i, v_j \rangle$ donde $i \neq j$ se vuelve automáticamente cero.

$$ 0 + 0 + \dots + a_j \langle v_j, v_j \rangle + \dots + 0 = 0 $$

$$ a_j \langle v_j, v_j \rangle = 0 $$

Por nuestra segunda hipótesis (vectores no nulos), sabemos con certeza que $\langle v_j, v_j \rangle \neq 0$.

Para que esta multiplicación dé cero, la única opción es que el escalar sea cero:

$$ a_j = 0 $$

Como este procedimiento matemático se puede repetir eligiendo cualquier vector $v_j$ (para todo $j = 1, \dots, k$), la conclusión es que **todos** los coeficientes de la combinación lineal original deben ser nulos ($a_1 = 0, a_2 = 0, \dots, a_k = 0$).

Por definición, esto demuestra que el conjunto de vectores es linealmente independiente. 