**Proposición.** Sea $V$ un espacio vectorial sobre $\mathbb{R}$ provisto de un producto interno. Si $X = \{v_1, \dots, v_r\}$ es un conjunto **ortogonal** de vectores no nulos ($v_i \neq 0$ para todo $i$), entonces el conjunto $X'$ formado por los vectores normalizados:

$$X' = \left\{ \frac{v_1}{\|v_1\|}, \dots, \frac{v_r}{\|v_r\|} \right\}$$

es un conjunto **ortonormal**.
****
**Demostración.** Para demostrar que un conjunto es ortonormal, debemos probar rigurosamente dos cosas sobre los nuevos vectores de $X'$:

1. Que todos tienen norma igual a $1$ (son vectores unitarios).
    
2. Que siguen siendo mutuamente ortogonales entre sí.
    
Para simplificar la notación de la prueba, llamemos $u_i = \frac{v_i}{\|v_i\|}$ a cada nuevo vector de $X'$. Notemos que $\frac{1}{\|v_i\|}$ es simplemente un escalar, ya que la norma es un número.

Tomemos un vector cualquiera $u_i \in X'$ y calculemos su norma:

$$\|u_i\| = \left\| \frac{1}{\|v_i\|} v_i \right\|$$

Por [[D-Propiedades de la Norma Inducida]], sabemos $\|c \cdot v\| = |c| \|v\|$:

$$\|u_i\| = \left| \frac{1}{\|v_i\|} \right| \|v_i\|$$

Como la norma $\|v_i\|$ siempre es un número positivo (porque los vectores son no nulos), su valor absoluto es igual a sí mismo:

$$\|u_i\| = \frac{1}{\|v_i\|} \|v_i\|$$

Simplificando:

$$\|u_i\| = 1$$

_(Esto prueba que todos los vectores del nuevo conjunto tienen longitud unitaria)._

**Ahora veamos que los vectores siguen siendo ortogonales**,

Tomemos dos vectores distintos $u_i, u_j \in X'$ (con $i \neq j$) y calculemos su producto interno:

$$\langle u_i, u_j \rangle = \left\langle \frac{v_i}{\|v_i\|}, \frac{v_j}{\|v_j\|} \right\rangle$$

Escrito en forma de producto por escalar, esto es:

$$\langle u_i, u_j \rangle = \left\langle \left(\frac{1}{\|v_i\|}\right)v_i, \left(\frac{1}{\|v_j\|}\right)v_j \right\rangle$$

Por la propiedad de bilinealidad del producto interno, podemos sacar los escalares hacia afuera multiplicando:

$$\langle u_i, u_j \rangle = \left( \frac{1}{\|v_i\|} \right) \left( \frac{1}{\|v_j\|} \right) \langle v_i, v_j \rangle$$

El conjunto original $X$ era ortogonal. Por lo tanto, el producto interno de dos vectores originales distintos es cero ($\langle v_i, v_j \rangle = 0$). Sustituyendo esto:

$$\langle u_i, u_j \rangle = \left( \frac{1}{\|v_i\| \|v_j\|} \right) \cdot 0$$

$$\langle u_i, u_j \rangle = 0$$

_(Esto prueba que los nuevos vectores siguen siendo ortogonales entre sí)._

