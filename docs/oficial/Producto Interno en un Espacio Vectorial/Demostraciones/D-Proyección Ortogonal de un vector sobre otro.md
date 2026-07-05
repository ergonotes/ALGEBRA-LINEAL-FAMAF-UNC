**Observación.** Sea $V$ un espacio vectorial sobre $\mathbb{R}$ provisto de un producto interno $\langle \cdot, \cdot \rangle$. Sean $u, v \in V$, con $v \neq 0$. La **proyección ortogonal** de $u$ sobre la dirección de $v$, denotada como $\text{proy}_v(u)$, se define como el único vector $p$ que satisface simultáneamente dos condiciones:

1. **Colinealidad:** El vector $p$ pertenece a la recta generada por $v$. Es decir, es un múltiplo escalar de $v$:
    $$p = \alpha v \quad \text{para algún } \alpha \in \mathbb{R}$$
    
2. **Ortogonalidad:** El vector diferencia (o vector "error") formado por $u - p$ es ortogonal al vector $v$. Es decir:
    $$\langle u - p, v \rangle = 0$$

La fórmula final para calcular esta proyección es:

$$ \text{proy}_v(u) = \frac{\langle u, v \rangle}{|v|^2} v $$
****
**Demostración.**
Por la segunda condición de nuestra definición, sabemos que el vector diferencia $u - p$ debe ser ortogonal a $v$. Por la definición de **ortogonalidad**, su producto interno debe ser cero:

$$ \langle u - p, v \rangle = 0 $$

Como sabemos por la primera condición que $p = \alpha v$, sustituimos $p$ en la ecuación:

$$ \langle u - \alpha v, v \rangle = 0 $$

Utilizamos la propiedad de linealidad en la primera componente (distributiva) para separar la expresión:

$$ \langle u, v \rangle - \langle \alpha v, v \rangle = 0 $$
Luego
$$ \langle u, v \rangle - \alpha \langle v, v \rangle = 0 $$

$$ \langle u, v \rangle = \alpha \langle v, v \rangle $$

El producto interno de un vector consigo mismo es su norma al cuadrado ($\langle v, v \rangle = \|v\|^2$):

$$ \langle u, v \rangle = \alpha |v|^2 $$

Como $v \neq 0$, sabemos que $\|v\|^2 > 0$, por lo que podemos dividir sin problemas para despejar $\alpha$:

$$ \alpha = \frac{\langle u, v \rangle}{|v|^2} $$


Ya descubrimos quién es el escalar $\alpha$. Ahora simplemente lo sustituimos de vuelta en nuestra fórmula original $p = \alpha v$:

$$ p = \frac{\langle u, v \rangle}{|v|^2} v $$

