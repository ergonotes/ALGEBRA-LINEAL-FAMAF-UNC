
### **Ejemplo de Aplicación**

**Problema:**

Sea $T: \mathbb{R}^3 \to \mathbb{R}^3$ definida como $T(x,y,z) = (3x+y, 2x-y+3z, x)$. Hallar la fórmula explícita del operador adjunto $T^*$.

**Resolución:**

**1. Elegir una base ortonormal:**

La base canónica de $\mathbb{R}^3$, denotada como $E = \{(1,0,0), (0,1,0), (0,0,1)\}$, es una base ortonormal (BON) respecto al producto interno habitual.

Gracias a esto, podemos usar nuestro teorema: $[T^*]_E^E = ([T]_E^E)^t$

**2. Armar la matriz original:**

Calculamos la matriz de $T$ en la base canónica (simplemente tomando los coeficientes de las variables en cada coordenada):

$$[T]_E^E = \begin{pmatrix} 3 & 1 & 0 \\ 2 & -1 & 3 \\ 1 & 0 & 0 \end{pmatrix}$$

**3. Obtener la matriz del adjunto:**

Por el teorema, simplemente trasponemos la matriz (las filas se convierten en columnas):

$$[T^*]_E^E = \begin{pmatrix} 3 & 2 & 1 \\ 1 & -1 & 0 \\ 0 & 3 & 0 \end{pmatrix}$$

**4. Reconstruir la fórmula:**

Multiplicamos esta nueva matriz por un vector genérico columna $(x,y,z)^t$ para recuperar la fórmula de la transformación:

$$T^*(x,y,z) = \begin{pmatrix} 3 & 2 & 1 \\ 1 & -1 & 0 \\ 0 & 3 & 0 \end{pmatrix} \begin{pmatrix} x \\ y \\ z \end{pmatrix} = \begin{pmatrix} 3x + 2y + z \\ x - y + 0z \\ 0x + 3y + 0z \end{pmatrix}$$

Por lo tanto, la fórmula final del operador adjunto es:

$$T^*(x,y,z) = (3x+2y+z, x-y, 3y)$$