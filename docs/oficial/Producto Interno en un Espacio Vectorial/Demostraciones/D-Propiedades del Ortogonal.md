**Proposición.** Sea $V$ un espacio vectorial provisto de un producto interno. Sea $X \subseteq V$ un subconjunto no vacío ($X \neq \emptyset$). Entonces se cumplen las siguientes propiedades:

**a)** $X^\perp$ es un subespacio vectorial de $V$.

**b)** Si $X \subseteq Y \implies Y^\perp \subseteq X^\perp$ _(La inclusión se invierte al pasar a los ortogonales)_.

**c)** $X \cap X^\perp = \{0\}$ siempre que $X$ sea un subespacio vectorial.

**d)** $X^\perp = (\text{esp.gen}(X))^\perp$
****
**Demostración.** 
Para probar que $X^\perp$ es un subespacio, debemos verificar las tres condiciones clásicas:

1. **El vector nulo pertenece:** Para cualquier $x \in X$, sabemos que $\langle 0, x \rangle = 0$. Por lo tanto, el vector $0$ pertenece a $X^\perp$.
    
2. **Cerradura bajo la suma:** Sean $u, v \in X^\perp$. Por definición, $\langle u, x \rangle = 0$ y $\langle v, x \rangle = 0$ para todo $x \in X$. Si tomamos la suma y aplicamos linealidad:
    
    $$\langle u + v, x \rangle = \langle u, x \rangle + \langle v, x \rangle = 0 + 0 = 0$$
    
    Como $(u+v)$ es ortogonal a todo $x \in X$, entonces $(u+v) \in X^\perp$.
    
3. **Cerradura bajo producto por escalar:** Sea $u \in X^\perp$ y un escalar $\alpha$.
    
    $$\langle \alpha u, x \rangle = \alpha \langle u, x \rangle = \alpha \cdot 0 = 0$$
    
    Por lo tanto, $\alpha u \in X^\perp$.
    
    Al cumplirse las tres condiciones, $X^\perp$ es un subespacio vectorial.
****
Veamos (**b**).
_(Nota: Mientras más grande es un conjunto, más difícil es ser ortogonal a TODOS sus elementos, por lo que su conjunto ortogonal se vuelve más pequeño)._

Supongamos que $X \subseteq Y$. Queremos demostrar que cualquier elemento que esté en $Y^\perp$ también debe estar en $X^\perp$.

Sea $v \in Y^\perp$. Por definición, $v$ es ortogonal a todos los elementos de $Y$ ($\langle v, y \rangle = 0, \forall y \in Y$).

Como $X$ está contenido en $Y$, todo elemento $x \in X$ es también un elemento de $Y$.

En consecuencia, el vector $v$ será ortogonal a todos los elementos $x \in X$.

Esto significa, por definición, que $v \in X^\perp$. Luego, razonando como en la *nota*, $X^\perp$ es seguramente más grande o igual que $Y^\perp$.   
****
Veamos (**c**) $X \cap X^\perp = \{0\}$ si $X$ es subespacio.

Supongamos que $X$ es un subespacio vectorial. 

Sea $v \in X \cap X^\perp$.

Esto significa que $v \in X$ y también que $v \in X^\perp$.

Como $v \in X^\perp$, sabemos que $\langle v, x \rangle = 0$ para cualquier vector $x \in X$.

Como $v \in X$, podemos elegir evaluar el producto interno del vector consigo mismo (es decir, tomar $x = v$):

$$\langle v, v \rangle = 0$$

Por el axioma de que el producto interno es _definido positivo_ ([[1.Productos Internos]], definición), la única forma de que la norma al cuadrado de un vector sea cero, es que el vector sea el vector nulo.

$$\implies v = 0$$

Por lo tanto, el único elemento en la intersección es el $\{0\}$.
****
Veamos **(d)**
Para demostrar una igualdad de conjuntos, debemos probar la doble inclusión. 

**Parte 1: $(\text{esp.gen}(X))^\perp \subseteq X^\perp$**

Sabemos por definición básica que cualquier conjunto está contenido dentro del espacio que genera:

$$X \subseteq \text{esp.gen}(X) = \{\text{C.L. de elementos de } X\}$$

Si aplicamos la propiedad **b)** que acabamos de demostrar (donde $Y$ es el $\text{esp.gen}(X)$), la relación de contención se invierte:

$$(b) \implies (\text{esp.gen}(X))^\perp \subseteq X^\perp$$

**Parte 2: $X^\perp \subseteq (\text{esp.gen}(X))^\perp$**

Sea $v \in X^\perp$. Esto significa que $v$ es ortogonal a $x_1, \dots, x_n \in X$.

Queremos ver qué pasa si tomamos cualquier elemento del espacio generado. Un elemento $w \in \text{esp.gen}(X)$ se escribe como una Combinación Lineal (C.L.) de vectores de $X$:

$$w = c_1 x_1 + \dots + c_n x_n$$

Si hacemos el producto interno de nuestro vector $v$ contra este elemento $w$, y expandimos por linealidad:

$$\langle v, w \rangle = \langle v, c_1 x_1 + \dots + c_n x_n \rangle = c_1\langle v, x_1\rangle + \dots + c_n\langle v, x_n\rangle$$

Como $v \in X^\perp$, cada producto interno $\langle v, x_i \rangle$ vale exactamente $0$:

$$\langle v, w \rangle = c_1(0) + \dots + c_n(0) = 0$$

Hemos demostrado que si $v$ es ortogonal a los elementos base de $X$, entonces $v$ es ortogonal a **cualquier** Combinación Lineal de $x_1, \dots, x_n$.

$$\therefore v \in (\text{esp.gen}(X))^\perp$$

Al haberse probado ambas contenciones mutuamente, queda demostrada la igualdad $X^\perp = (\text{esp.gen}(X))^\perp$. 