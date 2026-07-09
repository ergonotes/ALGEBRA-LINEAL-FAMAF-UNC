**Corolario.** Sea $V$ un espacio vectorial (de dimensión finita) provisto de un producto interno. Si $W$ es un subespacio vectorial de $V$, entonces existe una base ortogonal para $W$.
****
**Demostración.**
Como $W$ es un subespacio vectorial, sabemos que tiene alguna base. Sea $\{v_1, \dots, v_k\}$ dicha base de $W$.

Ya que [[D-Todo conjunto linealmente independiente se puede extender hasta formar una base]], podemos tomar estos vectores y agregarles más vectores linealmente independientes hasta formar una base completa para todo el espacio $V$.

Llamemos a esta base extendida: $\{v_1, \dots, v_k, v_{k+1}, \dots, v_n\}$.

Aplicamos la [[D-Ortogonalización de Gram-Schmidt]] a nuestra nueva base extendida de $V$.

Como resultado, obtenemos un nuevo conjunto de vectores $\{w_1, \dots, w_n\}$ que forma una **base ortogonal** para todo el espacio $V$. Y además,  por el mismo teorema, tomando exactamente los primeros $k$ vectores se cumple que:

$$\text{esp.gen}(w_1, \dots, w_k) = \text{esp.gen}(v_1, \dots, v_k)$$

Por definición de nuestro primer paso, el espacio generado por los vectores originales $\{v_1, \dots, v_k\}$ es exactamente nuestro subespacio $W$. Sustituyendo esto tenemos:

$$\text{esp.gen}(w_1, \dots, w_k) = W$$

Esto significa que los vectores $\{w_1, \dots, w_k\}$ generan a $W$. Como además son mutuamente ortogonales (y no nulos, por ende, linealmente independientes), concluimos que el conjunto $\{w_1, \dots, w_k\}$ es una base ortogonal para el subespacio $W$. 

