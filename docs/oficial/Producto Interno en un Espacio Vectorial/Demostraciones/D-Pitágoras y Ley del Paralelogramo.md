**Proposición.** Sea $V$ un espacio vectorial sobre $\mathbb{R}$ provisto de un producto interno $\langle \cdot, \cdot \rangle$. Sean $v, w \in V$. Entonces se cumplen las siguientes igualdades:

1. **Teorema de Pitágoras:**
    
    Si $w \perp v \implies \|v + w\|^2 = \|v\|^2 + \|w\|^2$
    
2. **Ley del Paralelogramo:**
    
    $\|v + w\|^2 + \|v - w\|^2 = 2\|v\|^2 + 2\|w\|^2$

****
**Demostración.**
**Parte 1.**

Partimos del desarrollo del binomio para la norma al cuadrado, que ya demostramos en la proposición anterior:

$$ |v + w|^2 = \langle v + w, v + w \rangle = |v|^2 + |w|^2 + 2\langle v, w \rangle $$

Por hipótesis, sabemos que los vectores son ortogonales ($w \perp v$).

$$ |v + w|^2 = |v|^2 + |w|^2 + 2(0) $$

$$ \implies |v + w|^2 = |v|^2 + |w|^2 $$

**Parte 2.**

Comenzamos expresando la suma de las normas al cuadrado mediante la definición del producto interno:

$$ |v + w|^2 + |v - w|^2 = \langle v + w, v + w \rangle + \langle v - w, v - w \rangle $$

A continuación, desarrollamos ambos productos internos distribuyendo por linealidad (tal como se ve en la imagen):

- El primer término se expande como: $\langle v, v \rangle + \langle w, w \rangle + 2\langle v, w \rangle$
    
- El segundo término se expande como: $\langle v, v \rangle + \langle w, w \rangle - 2\langle v, w \rangle$
    

Sumamos ambas expansiones directamente:

$$ = \big( \langle v, v \rangle + \langle w, w \rangle + 2\langle v, w \rangle \big) + \big( \langle v, v \rangle + \langle w, w \rangle - 2\langle v, w \rangle \big) $$

Notamos que los términos cruzados $+2\langle v, w \rangle$ y $-2\langle v, w \rangle$ se cancelan mutuamente al sumarlos. Agrupando los términos restantes nos queda:

$$ = 2\langle v, v \rangle + 2\langle w, w \rangle $$

Finalmente, recordando la definición de norma ($\|v\|^2 = \langle v, v \rangle$), reescribimos el resultado para obtener la expresión buscada:

$$ \implies 2|v|^2 + 2|w|^2 $$



