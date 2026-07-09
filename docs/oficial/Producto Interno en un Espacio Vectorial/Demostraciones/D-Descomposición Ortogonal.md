**Teorema.** Sea $V$ un espacio vectorial sobre $\mathbb{R}$ provisto de un producto interno (y de dimensión finita). Si $W \subseteq V$ es un subespacio vectorial de $V$, entonces el espacio total $V$ se puede expresar como la suma directa de $W$ y su complemento ortogonal $W^\perp$. Es decir:

$$V = W \oplus W^\perp$$
****
**Demostración.** Para demostrar que $V = W \oplus W^\perp$, debemos probar dos cosas (según la definición de [[3.Suma Directa de Subespacios]]):

1. Que $V = W + W^\perp$ (Cualquier vector de $V$ se puede armar sumando un elemento de $W$ y uno de $W^\perp$).
    
2. Que $W \cap W^\perp = \{0\}$ (No hay solapamiento entre los subespacios).

Sabemos por la [[D-Existencia de una Base Ortogonal en Subespacios]], (y la [[D-Ortogonalización de Gram-Schmidt]]) que $W$ tiene una base ortonormal, digamos $\{w_1, \dots, w_r\}$.

También sabemos, que [[D-Todo conjunto linealmente independiente se puede extender hasta formar una base]], y aplicando nuevamente el corolario, y teorema citados, llegamos a formar una base ortonormal para todo el espacio $V$. Sea esta base completa $\{w_1, \dots, w_r, w_{r+1}, \dots, w_n\}$.

Ahora tomemos un vector cualquiera $v \in V$. Como tenemos una base para todo el espacio, podemos escribir:

$$v = c_1 w_1 + \dots + c_r w_r + c_{r+1} w_{r+1} + \dots + c_n w_n$$

Agrupamos los términos de nuestra combinación lineal en dos grandes bloques. Llamaremos $z$ a la primera parte (los vectores de la base de $W$) y $u$ a la segunda parte (los vectores que agregamos para completar la base de $V$):

$$z = c_1 w_1 + \dots + c_r w_r$$

$$u = c_{r+1} w_{r+1} + \dots + c_n w_n$$

De esta manera, hemos escrito a nuestro vector original como la suma $v = z + u$.

- **Para $z$:** Como $z$ es una combinación lineal exclusiva de $\{w_1, \dots, w_r\}$, que es exactamente la base de $W$, resulta evidente que $z \in W$.
    
- **Para $u$:** Necesitamos probar que $u \in W^\perp$. Para ello, $u$ debe ser ortogonal a cualquier vector $w \in W$.

Como nuestra base total es ortonormal, los vectores $\{w_{r+1}, \dots, w_n\}$ son todos perpendiculares a los vectores de la base de $W$. 
Por lo tanto, el producto interno de cualquier $w_j$ (con $j = r+1, \dots, n$) contra cualquier $w \in W$ da cero: $\langle w_j, w \rangle = 0$.

Como $u$ está formado solo por esos vectores $w_j$, concluimos que $u$ es completamente ortogonal a $W$, por lo que $u \in W^\perp$.

Como cualquier vector $v \in V$ se puede escribir como $v = z + u$, con $z \in W$ y $u \in W^\perp$:

$$V = W + W^\perp$$

Además, por la proposición anterior (inciso _c_), ya habíamos demostrado que la intersección de un subespacio con su ortogonal contiene únicamente al vector nulo:

$$W \cap W^\perp = \{0\}$$

Como se cumplen las dos condiciones de la suma directa, concluimos finalmente que:

$$V = W \oplus W^\perp$$

