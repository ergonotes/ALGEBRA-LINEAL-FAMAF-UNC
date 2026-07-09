**Teorema.** Sean $V$ y $W$ espacios vectoriales sobre $\mathbb{R}$ con producto interno y de dimensión finita. Sea $T: V \to W$ una transformación lineal. Entonces, existe una **única** transformación lineal $T^*: W \to V$ (llamada la adjunta de $T$) tal que:

$$\langle T(v), w \rangle = \langle v, T^*(w) \rangle \quad \text{para todo } v \in V \text{ y para todo } w \in W$$
****
**Demostración.**
**Construcción de $T^*$**
Sean $\{v_1, \dots, v_n\}$ una base ortonormal de $V$ y $\{w_1, \dots, w_m\}$ una base ortonormal de $W$.
Si tomamos un vector $w_i$ de la base de $W$ y le aplicamos $T^*$, el resultado será algún vector que vive en el espacio $V$.

Como tenemos una base **ortonormal** de $V$ que es $\{v_1, v_2, \dots, v_n\}$, sabemos que **cualquier** vector de $V$ se puede escribir como combinación lineal de esa base:

$$T^*(w_i) = c_1 v_1 + c_2 v_2 + \dots + c_n v_n = \sum_{j=1}^n c_j v_j$$

Luego, por el [[D-Teorema de Coordenadas por Proyección]], tenemos que
$$c_j = \langle T^*(w_i), v_j \rangle$$

Sustituyendo esto en la suma, tendríamos:

$$T^*(w_i) = \sum_{j=1}^n \langle T^*(w_i), v_j \rangle v_j$$

El problema con esta expresión es que **no conocemos $T^*$**, así que no podemos calcular $\langle T^*(w_i), v_j \rangle$, por lo que vamos a suponer que la igualdad del enunciado es cierta, es decir, si $\langle v, T^*(w) \rangle = \langle T(v), w \rangle$, entonces también:

$$\langle T^*(w_i), v_j \rangle = \langle w_i, T(v_j) \rangle$$


Ahora vamos a definir quién es $T^*$ aplicándolo a los vectores de la base de $W$. Definimos:

$$T^*(w_i) = \sum_{j=1}^n \langle w_i, T(v_j) \rangle v_j \quad \text{para } i=1, \dots, m$$

Ya que [[D-Las imágenes de la base definen a toda la transformación]], sabemos que para definir una transformación lineal basta con definir qué le hace a los vectores de una base y luego "extender por linealidad". Esto nos garantiza que $T^*$ es una transformación lineal válida de $W$ en $V$.

Ahora, comprobemos qué pasa si hacemos el producto interno entre la imagen de $w_i$ y un vector de la base $v_s$:

$$\langle T^*(w_i), v_s \rangle = \left\langle \sum_{j=1}^n \langle w_i, T(v_j) \rangle v_j \, , \, v_s \right\rangle$$

Como $\langle w_i, T(v_j) \rangle$ es un simple número real, por linealidad en la primera componente podemos sacar la sumatoria y el escalar hacia afuera:

$$\langle T^*(w_i), v_s \rangle = \sum_{j=1}^n \langle w_i, T(v_j) \rangle \langle v_j, v_s \rangle$$

Como la base de $V$ es ortonormal, sabemos que $\langle v_j, v_s \rangle = 0$ siempre que $j \neq s$, y vale $1$ si $j = s$. Por lo tanto, toda la sumatoria colapsa a un único término (cuando $j=s$):

$$\langle T^*(w_i), v_s \rangle = \langle w_i, T(v_s) \rangle \cdot 1$$

$$\langle T^*(w_i), v_s \rangle = \langle w_i, T(v_s) \rangle$$

Por la propiedad de simetría del producto interno en $\mathbb{R}$, podemos invertir el orden de ambos lados para que se parezca al enunciado:

$$\langle v_s, T^*(w_i) \rangle = \langle T(v_s), w_i \rangle$$
Hemos probado que la expresión es válida para vectores $v_i$ y $w_j$ de las bases, pero la dimensión de las bases es finita y no estaríamos teniendo en cuenta vectores genéricos de $V$ y $W$. 

Ahora debemos probar que $\langle v, T^*(w) \rangle = \langle T(v), w \rangle$ para vectores genéricos $v \in V$ y $w \in W$.

Como tenemos bases, podemos escribir a $v$ y $w$ como combinaciones lineales:

$$v = \sum_{s=1}^n \alpha_s v_s \quad \text{y} \quad w = \sum_{i=1}^m \beta_i w_i$$

Sustituimos esto en nuestro producto interno $\langle v, T^*(w) \rangle$:

$$\langle v, T^*(w) \rangle = \left\langle \sum_{s=1}^n \alpha_s v_s \, , \, T^*\left( \sum_{i=1}^m \beta_i w_i \right) \right\rangle$$

Como $T^*$ es lineal, los escalares $\beta_i$ y la suma pueden salir de la función:

$$\langle v, T^*(w) \rangle = \left\langle \sum_{s=1}^n \alpha_s v_s \, , \, \sum_{i=1}^m \beta_i T^*(w_i) \right\rangle$$

Usamos la **bilinealidad del producto interno** para extraer todas las sumas y escalares hacia afuera:

$$\langle v, T^*(w) \rangle = \sum_{s=1}^n \sum_{i=1}^m \alpha_s \beta_i \langle v_s, T^*(w_i) \rangle$$

Anteriormente, demostramos que $\langle v_s, T^*(w_i) \rangle = \langle T(v_s), w_i \rangle$. Lo sustituimos:

$$= \sum_{s=1}^n \sum_{i=1}^m \alpha_s \beta_i \langle T(v_s), w_i \rangle$$

Ahora, hacemos el camino inverso. Volvemos a meter los escalares y las sumas dentro del producto interno por bilinealidad, y luego metemos la combinación lineal dentro de $T$ por ser una transformación lineal:

$$= \left\langle \sum_{s=1}^n \alpha_s T(v_s) \, , \, \sum_{i=1}^m \beta_i w_i \right\rangle$$

$$= \left\langle T\left( \sum_{s=1}^n \alpha_s v_s \right) \, , \, \sum_{i=1}^m \beta_i w_i \right\rangle$$

$$= \langle T(v), w \rangle$$

Esto demuestra que la igualdad se cumple para cualquier par de vectores genéricos.

Ahora probaremos la unicidad.

Supongamos que existe otro operador $U: W \to V$ que también cumple la propiedad del teorema, es decir, $\langle T(v), w \rangle = \langle v, U(w) \rangle$.

Si igualamos esto con la propiedad de $T^*$, tenemos que para todo $v \in V$ y $w \in W$:

$$\langle v, T^*(w) \rangle = \langle v, U(w) \rangle$$

$$\langle v, T^*(w) \rangle - \langle v, U(w) \rangle = 0$$

$$\langle v, T^*(w) - U(w) \rangle = 0$$

Como esto debe cumplirse para _cualquier_ vector $v$, podemos elegir astutamente que $v$ sea exactamente el vector resultante de la resta, es decir, elegimos $v = T^*(w) - U(w)$:

$$\langle T^*(w) - U(w) \, , \, T^*(w) - U(w) \rangle = 0$$

Por la propiedad de que los [[1.Productos Internos]] son _definidos positivos_, la única forma de que un vector contra sí mismo dé cero es que el vector sea el nulo:

$$T^*(w) - U(w) = 0 \implies T^*(w) = U(w)$$

Como esto vale para todo $w \in W$, concluimos que $T^* = U$. El operador adjunto es único.