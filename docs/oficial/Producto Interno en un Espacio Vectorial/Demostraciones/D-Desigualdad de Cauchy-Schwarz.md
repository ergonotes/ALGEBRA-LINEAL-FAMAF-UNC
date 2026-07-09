**Proposición.** Sea $V$ un espacio vectorial sobre $\mathbb{R}$ provisto de un producto interno $\langle \cdot, \cdot \rangle$. Sean $v, w \in V$. Entonces se cumple que:

$$|\langle v, w \rangle| \leq \|v\| \cdot \|w\|$$

Además, la igualdad vale ($\langle v, w \rangle| = \|v\| \cdot \|w\|$) si y solo si $v$ y $w$ son múltiplos entre sí (es decir, son linealmente dependientes).
****
**Demostración.**
Supongamos que $v = 0$. En ese caso, $\langle 0, w \rangle = 0$ y $\|0\| = 0$. La desigualdad nos quedaría $0 \leq 0$, lo cual es trivialmente cierto.

A partir de ahora, supondremos que $v \neq 0$, lo que nos garantiza que $\|v\|^2 > 0$.

Definimos el escalar $\alpha$ asociado a la proyección ortogonal de $w$ sobre $v$:

$$\alpha = \frac{\langle v, w \rangle}{\langle v, v \rangle} = \frac{\langle v, w \rangle}{\|v\|^2}$$

Por lo que vimos en la [[D-Proyección Ortogonal de un vector sobre otro]], sabemos que el vector $(w - \alpha v)$ es ortogonal a $v$. Al ser ortogonal a $v$, también es ortogonal a cualquier múltiplo de $v$. Es decir:

$$(w - \alpha v) \perp \alpha v$$

Podemos reescribir el vector $w$ de la forma:

$$w = (w - \alpha v) + \alpha v$$

Observa que hemos expresado $w$ como la suma de dos vectores que son ortogonales entre sí. Y como son ortogonales, podemos aplicar el **Teorema de Pitágoras** ([[D-Pitágoras y Ley del Paralelogramo]]) a sus normas al cuadrado:

$$\|w\|^2 = \|w - \alpha v\|^2 + \|\alpha v\|^2$$

Sabemos que $\|w - \alpha v\|^2 \geq 0$.

Y si en nuestra ecuación anterior eliminamos ese término positivo del lado derecho, el valor resultante será inevitablemente menor (o igual). Obtenemos así:

$$\|w\|^2 \geq \|\alpha v\|^2$$

Extraemos la raíz cuadrada a ambos lados. Al sacar la constante de la norma, recordamos usar el valor absoluto:

$$\|w\| \geq |\alpha| \cdot \|v\|$$

Ahora, sustituimos $\alpha$ por su valor original:

$$\|w\| \geq \left| \frac{\langle v, w \rangle}{\|v\|^2} \right| \cdot \|v\|$$

Como la norma al cuadrado en el denominador ya es positiva, podemos reescribirlo así:

$$\|w\| \geq \frac{|\langle v, w \rangle|}{\|v\|^2} \cdot \|v\|$$

Simplificamos :

$$\|w\| \geq \frac{|\langle v, w \rangle|}{\|v\|}$$

Finalmente, como $\|v\| > 0$, pasamos multiplicando la norma al otro lado sin alterar la desigualdad:

$$\|v\| \|w\| \geq |\langle v, w \rangle|$$

Reordenando, llegamos a la expresión clásica:

$$|\langle v, w \rangle| \leq \|v\| \|w\|$$
****
### **Demostración de la Condición de Igualdad**

¿Qué tiene que pasar para que la desigualdad se convierta en una igualdad exacta ($=$)?

El único momento donde generamos la desigualdad fue al afirmar que $\|w\|^2 \geq \|\alpha v\|^2$ tras quitar el término $\|w - \alpha v\|^2$.

Para que se mantenga la igualdad, ese término que quitamos tenía que valer exactamente cero:

$$\|w - \alpha v\|^2 = 0$$

Por el axioma de la norma (la única norma cero es la del vector nulo), esto implica que:

$$w - \alpha v = 0$$

$$\implies w = \alpha v$$

Esto demuestra que la igualdad se cumple **si y solo si** $w$ es un múltiplo escalar de $v$ (es decir, $w$ y $v$ apuntan en la misma línea).