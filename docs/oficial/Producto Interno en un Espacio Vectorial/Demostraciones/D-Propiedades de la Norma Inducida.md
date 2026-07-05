**Proposición.** Sea $V$ un espacio vectorial sobre el cuerpo de los números reales $\mathbb{R}$ provisto de un producto interno $\langle \cdot, \cdot \rangle$. Sean $v, w \in V$. Entonces se cumplen las siguientes propiedades:

1. Si $c \in \mathbb{R} \implies \|c \cdot v\| = |c| \cdot \|v\|$ _(Homogeneidad absoluta)_.
    
2. $\|v + w\|^2 = \|v\|^2 + \|w\|^2 + 2\langle v, w \rangle$ _(Desarrollo del binomio para la norma)_.
****
**Demostración.**

**Veamos $\|c \cdot v\| = |c| \cdot \|v\|$**:

Partimos de la definición de la norma al cuadrado:

$$ |c \cdot v|^2 = \langle c \cdot v, c \cdot v \rangle $$

Como estamos en un espacio vectorial real, el producto interno es bilineal. Esto nos permite extraer el escalar $c$ de la primera componente, y luego de la segunda:

$$ \langle c \cdot v, c \cdot v \rangle = c \langle v, c \cdot v \rangle = c \cdot c \langle v, v \rangle = c^2 \langle v, v \rangle $$

Reescribiendo $\langle v, v \rangle$ como la norma al cuadrado del vector original:

$$ |c \cdot v|^2 = c^2 |v|^2 $$

Finalmente, tomando la raíz cuadrada a ambos lados de la ecuación, obtenemos la expresión buscada:

$$ |c \cdot v| = \sqrt{c^2} |v| = |c| \cdot |v| $$

**Veamos $\|v + w\|^2 = \|v\|^2 + \|w\|^2 + 2\langle v, w \rangle$**:

Nuevamente, partimos de la definición de la norma al cuadrado aplicada a la suma de vectores:

$$ |v + w|^2 = \langle v + w, v + w \rangle $$

Aplicamos la propiedad de linealidad (propiedad distributiva del producto interno):

$$ \langle v + w, v + w \rangle = \langle v, v + w \rangle + \langle w, v + w \rangle $$

Y luego distribuyendo la segunda componente en cada término:

$$ = \langle v, v \rangle + \langle v, w \rangle + \langle w, v \rangle + \langle w, w \rangle $$

Al trabajar sobre $\mathbb{R}$, sabemos que el producto interno es simétrico, por lo que $\langle w, v \rangle = \langle v, w \rangle$. Además, reemplazamos $\langle v, v \rangle$ y $\langle w, w \rangle$ por sus respectivas normas al cuadrado:

$$ = |v|^2 + \langle v, w \rangle + \langle v, w \rangle + |w|^2 $$

Y llegamos al resultado final:

$$ \implies |v|^2 + 2\langle v, w \rangle + |w|^2 $$




