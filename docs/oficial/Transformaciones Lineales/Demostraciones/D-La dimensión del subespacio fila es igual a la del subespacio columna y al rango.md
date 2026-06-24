**Teorema**. Si $A$ es una matriz $m \times n$ con coeficientes en $\mathbb{K}$, entonces
$$
\text{rango fila } (A) = \text{rango columna } (A).
$$

****

**Demostración**. Sea $T$ la transformación lineal
$$
\begin{aligned}
T: \mathbb{K}^{n \times 1} &\to \mathbb{K}^{m \times 1} \\
X &\mapsto AX.
\end{aligned}
$$
Observar que
$$
\text{Nu}(T) = \{X \in \mathbb{K}^{n \times 1} : AX = 0\}.
$$
Es decir $\text{Nu}(T)$ es el subespacio de soluciones del sistema homogéneo $AX = 0$. Ahora bien, si $k = \text{rango fila } (A)$, sabemos (al escalonar la matriz $A$ con Gauss, obtenemos $k$ filas "*sobrevivientes*" con pivotes) que la dimensión del subespacio de soluciones del sistema homogéneo $AX = 0$ es $n - k$ (al tener $n$ columnas o incógnitas y $k$ de esas columnas tienen pivote). Luego, definiendo:
$$k \ = \ \text{rango fila}(A)$$
$$n \ =  \ \dim V$$
 Como la transformación va desde el espacio $\mathbb{K}^{n \times 1}$ (llamado $V$), la dimensión total de ese espacio de partida es exactamente $n$. 
$$\text{Dimensión del subespacio de soluciones} \ = \ \text{nulidad}(T) \ = \ n-k$$
El subespacio de soluciones al sistema $AX = 0$ es exactamente el Núcleo (o _Kernel_) de la transformación. La dimensión de ese núcleo es la **nulidad** como vimos. 

Luego, aplicando el diccionario nuevo:  
$$\text{nulidad}(T) = \dim V - \text{rango fila}(A)$$

Pasamos sumando el $\text{rango fila}(A)$ hacia la izquierda, y pasa restando la $\text{nulidad}(T)$ hacia la derecha:

$$\text{rango fila}(A) = \dim V - \text{nulidad}(T)$$
Por otro lado
$$
\text{Im}(T) = \{AX : X \in \mathbb{K}^{n \times 1}\}.
$$
Ahora bien,
$$
AX = \begin{bmatrix} a_{11}x_1 + \cdots a_{1n}x_n \\ \vdots \\ a_{m1}x_1 + \cdots + a_{mn}x_n \end{bmatrix} = x_1 \begin{bmatrix} a_{11} \\ \vdots \\ a_{m1} \end{bmatrix} + \cdots + x_n \begin{bmatrix} a_{1n} \\ \vdots \\ a_{mn} \end{bmatrix}
$$
Es decir, que la imagen de $T$ es el espacio generado por las columnas de $A$. Por tanto,
$$
\text{rango}(T) = \text{rango columna } (A).
$$
Por el teorema anterior ([[D-La dimensión del dominio de una transformación lineal es igual a la suma de su nulidad y rango]])
$$
\text{rango}(T) = \dim V - \text{nulidad}(T),
$$
y por lo tanto

$$
\text{rango columna } (A) = \dim V - \text{nulidad}(T).
$$
Obviamente, las igualdades anteriores implican
$$
\text{rango fila } (A) = \text{rango columna } (A).
$$