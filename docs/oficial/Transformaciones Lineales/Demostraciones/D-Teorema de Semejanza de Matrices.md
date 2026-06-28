**Teorema (Semejanza de Matrices).** Sean $\beta$ y $\beta'$ bases ordenadas de un espacio vectorial $V$ ($\dim V < \infty$), y sea $T: V \to V$ una transformación lineal.

Si definimos nuestra matriz de transición como $P = [\text{Id}]_{\beta'}^{\beta}$ (el traductor de $\beta'$ hacia $\beta$), entonces podemos calcular la matriz de $T$ en la nueva base $\beta'$ mediante la siguiente composición:
$$[T]_{\beta'} = P^{-1} \cdot [T]_{\beta} \cdot P$$
****
**Demostración.**
Por definición, sabemos que $P = [\text{Id}]_{\beta'}^{\beta}$.

Por el corolario anterior, sabemos que su inversa es $P^{-1} = [\text{Id}]_{\beta}^{\beta'}$.

Sustituimos estas matrices en nuestra ecuación $P^{-1} [T]_{\beta} P$:

$$P^{-1} [T]_{\beta} P = [\text{Id}]_{\beta}^{\beta'} \cdot [T]_{\beta}^{\beta} \cdot [\text{Id}]_{\beta'}^{\beta}$$

Aplicamos el **Teorema de la Composición ([[D-Representación Matricial de la Composición]])** leyéndolo de derecha a izquierda (como siempre viajan los vectores):

Al multiplicar las tres matrices, las bases intermedias ($\beta$) se fusionan y desaparecen,

$$= [\text{Id} \circ T \circ \text{Id}]_{\beta'}^{\beta'}$$

Como componer con la Identidad no altera a la función $T$ (ya que $T \circ \text{Id} = T$), simplificamos el interior del corchete:

$$= [T]_{\beta'}^{\beta'}$$

Que, por convención de notación, cuando la base de entrada y salida es la misma, se escribe simplemente como:

$$= [T]_{\beta'}$$

