**Corolario.** Sea $V$ un espacio vectorial de dimensión finita provisto de un producto interno. Si $W \subseteq V$ es un subespacio vectorial de $V$, entonces se cumplen las siguientes dos propiedades:

1. $\dim V = \dim W + \dim W^\perp$
    
2. $(W^\perp)^\perp = W$
****
**Demostración.** Esta primera parte es una consecuencia **directa del teorema anterior ([[D-Descomposición Ortogonal]])**.
En el mismo llegamos a que:

$$V = W \oplus W^\perp$$

Por un teorema clásico visto anteriormente ([[D-Dimensión de la suma, suma las partes, resta la intersección]]), sabemos que si un espacio es la suma directa de dos subespacios, la dimensión del espacio total es exactamente igual a la suma de las dimensiones de esos subespacios (ya que su intersección es solo el $\{0\}$ y no hay vectores "*repetidos*").

Se deduce inmediatamente que:

$$\dim V = \dim W + \dim W^\perp$$

Ahora, para demostrar que dos subespacios son iguales, veremos que uno está contenido en el otro y que ambos tienen exactamente la misma dimensión.

**Demostrar la contención $W \subseteq (W^\perp)^\perp$.**

Recordemos una propiedad general: para cualquier conjunto $X \neq \emptyset$, se cumple que $X \subseteq (X^\perp)^\perp$.

_(Si tomamos un vector $x \in X$, por definición es ortogonal a todos los vectores de $X^\perp$. Y el conjunto de todos los vectores que son ortogonales a $X^\perp$ es precisamente $(X^\perp)^\perp$. Por ende, $x \in (X^\perp)^\perp$)._

Aplicando esta propiedad general a nuestro subespacio $W$, obtenemos directamente nuestra primera condición:

$$W \subseteq (W^\perp)^\perp$$

**Igualar las dimensiones.**

Ahora usaremos la propiedad 1 (que acabamos de demostrar) de forma estratégica, aplicándola a dos subespacios distintos:

- Primero, la aplicamos al subespacio $W$:
    $$\dim V = \dim W + \dim W^\perp$$
    
- Y como $W^\perp$ también es un subespacio vectorial de $V$, podemos aplicarle la misma fórmula (reemplazando $W$ por $W^\perp$):
    $$\dim V = \dim W^\perp + \dim((W^\perp)^\perp)$$

Como ambas expresiones son iguales a $\dim V$, podemos igualarlas entre sí:

$$\dim W + \dim W^\perp = \dim W^\perp + \dim((W^\perp)^\perp)$$

Dado que estamos trabajando en dimensión finita, $\dim W^\perp$ es un número real finito. Podemos cancelarlo restándolo a ambos lados de la ecuación, obteniendo:

$$\dim W = \dim((W^\perp)^\perp)$$

Hemos demostrado simultáneamente dos cosas:

1. El subespacio $W$ está contenido dentro del subespacio $(W^\perp)^\perp$.
    
2. Ambos subespacios tienen exactamente la misma dimensión.

Como vimos en los corolarios consecuencia de [[D-Subespacio propio, dimensión menor]], si un subespacio está contenido dentro de otro y ambos tienen la misma dimensión finita, son el **mismo** espacio. Por lo tanto:

$$W = (W^\perp)^\perp$$

