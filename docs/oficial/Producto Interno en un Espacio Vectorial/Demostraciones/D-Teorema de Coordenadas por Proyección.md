**Teorema (de la Descomposición de Fourier)** Sea $V$ un espacio vectorial provisto de un producto interno.

**a)** Si $B = \{v_1, \dots, v_n\}$ es una **base ortogonal** de $V$, entonces para todo vector $v \in V$ se tiene que:

$$v = \sum_{i=1}^n \frac{\langle v, v_i \rangle}{\langle v_i, v_i \rangle} v_i$$

**b)** Si $B = \{u_1, \dots, u_n\}$ es una **base ortonormal** (BON) de $V$, entonces para todo vector $v \in V$ se tiene que:

$$v = \sum_{i=1}^n \langle v, u_i \rangle u_i$$
****
**Demostración.**
Sea $v$ un vector cualquiera perteneciente a $V$. Como $B = \{v_1, \dots, v_n\}$ es una base del espacio, sabemos por definición que $v$ se puede escribir de manera **única** como una combinación lineal de los elementos de dicha base. Es decir, existen escalares $c_1, \dots, c_n \in \mathbb{R}$ tales que:

$$v = \sum_{j=1}^n c_j v_j = c_1 v_1 + c_2 v_2 + \dots + c_n v_n$$

Tomamos el producto interno del vector original $v$ contra el vector específico $v_i$ de la base:

$$\langle v, v_i \rangle = \left\langle \sum_{j=1}^n c_j v_j \, , \, v_i \right\rangle$$

Por la propiedad de linealidad en la primera componente, podemos reescribir el lado derecho:

$$\langle v, v_i \rangle = \sum_{j=1}^n c_j \langle v_j, v_i \rangle$$

$$\langle v, v_i \rangle = c_1\langle v_1, v_i\rangle + \dots + c_i\langle v_i, v_i\rangle + \dots + c_n\langle v_n, v_i\rangle$$

Aquí interviene la hipótesis fundamental: **la base es ortogonal**. Esto significa que el producto interno entre dos vectores distintos de la base siempre da cero ($\langle v_j, v_i \rangle = 0$ para todo $j \neq i$).

Así, sobrevive únicamente el término donde el subíndice coincide ($j=i$):

$$\langle v, v_i \rangle = c_i \langle v_i, v_i \rangle$$

Como la base está formada por vectores no nulos, sabemos que $\langle v_i, v_i \rangle \neq 0$, por lo que podemos despejar el escalar $c_i$ dividiendo:

$$c_i = \frac{\langle v, v_i \rangle}{\langle v_i, v_i \rangle}$$

Sustituyendo este valor de los coeficientes de vuelta en nuestra combinación lineal original, obtenemos:

$$v = \sum_{i=1}^n \frac{\langle v, v_i \rangle}{\langle v_i, v_i \rangle} v_i$$
****
Veamos **b**).
Esta demostración es un corolario directo del inciso anterior.

Si tenemos una base ortonormal $B = \{u_1, \dots, u_n\}$, por definición cumple dos propiedades:

1. Es ortogonal.
    
2. Todos sus vectores tienen norma igual a $1$ ($\|u_i\| = 1$).

Como es ortogonal, podemos aplicar directamente la fórmula del inciso **a)**:

$$v = \sum_{i=1}^n \frac{\langle v, u_i \rangle}{\langle u_i, u_i \rangle} u_i$$

Pero al ser ortonormal, sabemos que el denominador es siempre la norma al cuadrado del vector unitario:

$$\langle u_i, u_i \rangle = \|u_i\|^2 = 1^2 = 1$$

Sustituyendo el denominador por $1$, la fórmula se simplifica:

$$v = \sum_{i=1}^n \langle v, u_i \rangle u_i$$
