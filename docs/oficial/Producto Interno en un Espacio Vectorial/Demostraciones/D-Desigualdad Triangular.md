**Proposición.** Sea $V$ un espacio vectorial sobre los números reales $\mathbb{R}$ provisto de un producto interno $\langle \cdot, \cdot \rangle$. Sean $v, w \in V$. Entonces se cumple la siguiente desigualdad:

$$\|v + w\| \leq \|v\| + \|w\|$$
****
**Demostración.**
Utilizando la propiedad de que la norma al cuadrado de un vector es igual al producto interno del vector consigo mismo, y expandiendo por [[D-Propiedades de la Norma Inducida]], obtenemos:

$$\|v + w\|^2 = \langle v + w, v + w \rangle = \|v\|^2 + \|w\|^2 + 2\langle v, w \rangle$$

Por la [[D-Desigualdad de Cauchy-Schwarz]], sabemos que el valor absoluto del producto interno está acotado por el producto de las normas: $|\langle v, w \rangle| \leq \|v\| \|w\|$.

Cualquier número real es siempre menor o igual a su valor absoluto, por lo que podemos afirmar con total seguridad que:

$$\langle v, w \rangle \leq \|v\| \|w\|$$

Ahora, el lado derecho de la ecuación se volverá inevitablemente mayor o igual:

$$\|v + w\|^2 \leq \|v\|^2 + \|w\|^2 + 2\|v\| \|w\|$$

Si reordenamos un poco los sumandos del lado derecho, es fácil reconocer la estructura del desarrollo de un binomio al cuadrado ($a^2 + 2ab + b^2$):

$$\|v + w\|^2 \leq \|v\|^2 + 2\|v\| \|w\| + \|w\|^2$$

$$\|v + w\|^2 \leq (\|v\| + \|w\|)^2$$

Como tanto $\|v + w\|$ como $(\|v\| + \|w\|)$ son cantidades positivas o nulas, podemos aplicar la raíz cuadrada a ambos lados de la desigualdad sin alterar su sentido, concluyendo finalmente que:

$$\|v + w\| \leq \|v\| + \|w\|$$

