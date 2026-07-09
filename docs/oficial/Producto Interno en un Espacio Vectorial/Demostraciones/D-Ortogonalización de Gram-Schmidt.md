**Teorema.** Sea $V$ un espacio vectorial sobre $\mathbb{R}$ provisto de un producto interno $\langle \cdot, \cdot \rangle$ y de dimensión finita ($\dim V < \infty$).

Sea $\{v_1, \dots, v_n\}$ una base de $V$.

Entonces, existe una base ortogonal de $V$ formada por los vectores $\{w_1, \dots, w_n\}$, tal que el subespacio generado por los primeros $m$ vectores originales $\{v_1, \dots, v_m\}$ es el mismo que el espacio generado por los nuevos vectores $\{w_1, \dots, w_m\}$ para todo $m = 1, \dots, n$.

Explícitamente, los vectores de esta base están dados por la siguiente construcción recurrente:

$$w_1 = v_1$$

$$w_2 = v_2 - \frac{\langle v_2, w_1 \rangle}{\langle w_1, w_1 \rangle} w_1$$

$$w_3 = v_3 - \frac{\langle v_3, w_1 \rangle}{\langle w_1, w_1 \rangle} w_1 - \frac{\langle v_3, w_2 \rangle}{\langle w_2, w_2 \rangle} w_2 \quad \left(\text{Es decir, } v_3 - \text{proy}_{w_1}(v_3) - \text{proy}_{w_2}(v_3)\right)$$

$$\vdots$$

$$w_n = v_n - \sum_{j=1}^{n-1} \frac{\langle v_n, w_j \rangle}{\langle w_j, w_j \rangle} w_j$$
****
**Demostración.**
La prueba se realiza mediante el principio de **inducción en $n$** (la cantidad de vectores).

**Casos base.**

- Para $n=1$: Es **trivial**, ya que $w_1 = v_1$. El espacio generado es idéntico por definición, y un conjunto de un solo vector no nulo es trivialmente ortogonal.
    
- Para $n=2$: El caso **ya lo hicimos** en la explicación del algoritmo del proceso.

**Paso inductivo.**

Supongamos que el teorema vale para el paso $k-1$. Veamos que también se cumple para el paso $k$.

Es decir, por hipótesis inductiva sabemos que el conjunto $\{w_1, \dots, w_{k-1}\}$ ya es ortogonal y que el espacio generado por $\{v_1, \dots, v_{k-1}\}$ es exactamente el mismo que el espacio generado por $\{w_1, \dots, w_{k-1}\}$.

Sea el nuevo vector $w_k$ definido por nuestra fórmula:

$$w_k = v_k - \sum_{j=1}^{k-1} \frac{\langle v_k, w_j \rangle}{\langle w_j, w_j \rangle} w_j$$

Veamos que este vector cumple la condición requerida: ser ortogonal a todos los vectores anteriores. Debemos probar que $\langle w_k, w_i \rangle = 0$ para cualquier $i = 1, \dots, k-1$.

Tomamos el producto interno sustituyendo la definición de $w_k$:

$$\langle w_k, w_i \rangle = \left\langle v_k - \sum_{j=1}^{k-1} \frac{\langle v_k, w_j \rangle}{\langle w_j, w_j \rangle} w_j \, , \, w_i \right\rangle$$

Por la propiedad de linealidad del producto interno en su primera componente, distribuimos el producto con $w_i$:

$$\langle w_k, w_i \rangle = \langle v_k, w_i \rangle - \sum_{j=1}^{k-1} \frac{\langle v_k, w_j \rangle}{\langle w_j, w_j \rangle} \langle w_j, w_i \rangle$$

Aquí aplicamos nuestra hipótesis inductiva: como el conjunto $\{w_1, \dots, w_{k-1}\}$ es ortogonal, todos los productos cruzados $\langle w_j, w_i \rangle$ valen cero siempre que $j \neq i$.

Por lo tanto, de toda esa suma gigante, el único término que sobrevive es aquel donde el índice $j$ es exactamente igual a $i$:

$$\langle w_k, w_i \rangle = \langle v_k, w_i \rangle - \frac{\langle v_k, w_i \rangle}{\langle w_i, w_i \rangle} \langle w_i, w_i \rangle$$

Podemos simplificar el término $\langle w_i, w_i \rangle$ que está simultáneamente en el numerador y el denominador:

$$\langle w_k, w_i \rangle = \langle v_k, w_i \rangle - \langle v_k, w_i \rangle = 0$$

Al dar como resultado cero, confirmamos que el nuevo vector $w_k$ es efectivamente ortogonal a todos los $w_i$ anteriores.

Como $w_k$ se construye combinando linealmente a $v_k$ con los vectores $w_j$ anteriores, el espacio generado por todo el conjunto se mantiene equivalente, concluyendo la demostración.