#### **Observación 2.5.2** Un caso especial de multiplicación es la multiplicación por matrices diagonales. 
Sea $n \in \mathbb{N}$ y$$\operatorname{diag}(d_1, d_2, \ldots, d_n) := \begin{pmatrix} d_1 & 0 & \cdots & 0 \\ 0 & d_2 & \cdots & 0 \\ \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & \cdots & d_n \end{pmatrix}$$matriz $n \times n$ diagonal con valor $d_i$ en la posición $ii$, entonces si $A$ es matriz $n \times p$, con multiplicación a izquierda de la matriz diagonal por $A$ obtenemos:
$\begin{pmatrix} d_1 & 0 & \cdots & 0 \\ 0 & d_2 & \cdots & 0 \\ \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & \cdots & d_n \end{pmatrix} \begin{pmatrix} a_{11} & a_{12} & \cdots & a_{1p} \\ a_{21} & a_{22} & \cdots & a_{2p} \\ \vdots & \vdots & \ddots & \vdots \\ a_{n1} & a_{n2} & \cdots & a_{np} \end{pmatrix} = \begin{pmatrix} d_1 a_{11} & d_1 a_{12} & \cdots & d_1 a_{1p} \\ d_2 a_{21} & d_2 a_{22} & \cdots & d_2 a_{2p} \\ \vdots & \vdots & \ddots & \vdots \\ d_n a_{n1} & d_n a_{n2} & \cdots & d_n a_{np} \end{pmatrix}$.
Esto es claro, pues si denotamos $D = \operatorname{diag}(d_1, d_2, \dots, d_n)$, el coeficiente $ij$ de $DA$ es la fila $i$ de $D$ por la columna $j$ de $A$, es decir$$[DA]_{ij} = 0 \cdot a_{ij} + \cdots + 0 \cdot a_{i-1,j} + d_i a_{ij} + 0 \cdot a_{i+1,j} + \cdots + 0 \cdot a_{nj} = d_i a_{ij}$$Observar que en el caso de que $D$ sea matriz escalar (es decir $d_1 = d_2 = \cdots = d_n$), $DA$ es multiplicar por el mismo número todos los coeficientes de $A$. En particular, en este caso, si $A$ es $n \times n$, $DA = AD$.

Finalmente, de lo visto más arriba respecto a la multiplicación por una
matriz diagonal obtenemos:![[Pasted image 20250914164501.png]]
****
#### **Más observaciones**
- **Multiplicar cualquier matriz por la matriz nula resulta la matriz nula,**

- **Existen divisores de cero**: en general, $AB=0$ no implica que $A=0$ o $B=0$ o, lo que es lo mismo, el producto de matrices no nulas puede resultar en una matriz nula. Por ejemplo
![[Pasted image 20250914165307.png]]

- En general **no se cumple la propiedad cancelativa**: si $A\neq0$ y $AB=AC$ no necesariamente se cumple que $B=C$. Por ejemplo,
![[Pasted image 20250914165407.png]]

No se cumple la fórmula del binomio: sean $A, B$ matrices $n × n$, entonces
$$(A + B)^2 = (A + B)(A + B)$$$$
= A(A + B) + B(A + B)$$$$= AA + AB + BA + BB$$
$$= A^2 + AB + BA + B^2,$$
y esta última expresión puede no ser igual a $A2 + 2AB + B2$ ya que el
producto de matrices no es conmutativo (en general).