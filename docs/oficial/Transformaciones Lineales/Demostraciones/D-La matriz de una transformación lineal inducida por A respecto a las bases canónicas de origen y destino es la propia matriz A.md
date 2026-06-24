**Observación.** Sea $A \in \mathbb{K}^{m \times n}$. Podemos definir la transformación lineal inducida $T_A : \mathbb{K}^n \to \mathbb{K}^m$ dada por la regla de correspondencia $T_A(X) = AX$.

Si $E_n = \{e_1, \dots, e_n\}$ es la base canónica de $\mathbb{K}^n$, y $E_m = \{e'_1, \dots, e'_m\}$ es la base canónica de $\mathbb{K}^m$, entonces la matriz asociada a la transformación respecto a estas bases es exactamente la matriz $A$:

$$[T_A]_{E_n, E_m} = A$$
****
**Demostración.**
Por definición, la matriz asociada a una transformación lineal $T_A$ respecto a las bases $E_n$ y $E_m$ es una matriz $M$ de tamaño $m \times n$, cuya $j$-ésima columna está dada por el vector de coordenadas de la imagen del $j$-ésimo vector de la base del dominio, expresado en la base del codominio. Formalmente:

$$\text{Columna}_j(M) = [T_A(e_j)]_{E_m} \quad \text{para todo } j = 1, 2, \dots, n$$

Aplicamos la definición de nuestra transformación $T_A$ al $j$-ésimo vector de la base canónica $E_n$:

$$T_A(e_j) = A e_j$$

Sabiendo que el vector canónico $e_j$ tiene un $1$ en la posición $j$ y ceros en el resto, el producto matricial $A e_j$ aísla exactamente la $j$-ésima columna de la matriz $A$.

Es decir, si denotamos las entradas de $A$ como $a_{ij}$, el resultado es:

$$T_A(e_j) = \begin{pmatrix} a_{11} & \dots & a_{1j} & \dots & a_{1n} \\ a_{21} & \dots & a_{2j} & \dots & a_{2n} \\ \vdots & \ddots & \vdots & \ddots & \vdots \\ a_{m1} & \dots & a_{mj} & \dots & a_{mn} \end{pmatrix} \begin{pmatrix} 0 \\ \vdots \\ 1 \\ \vdots \\ 0 \end{pmatrix} = \begin{pmatrix} a_{1j} \\ a_{2j} \\ \vdots \\ a_{mj} \end{pmatrix}$$

El vector resultante $\begin{pmatrix} a_{1j} & a_{2j} & \dots & a_{mj} \end{pmatrix}^T$ pertenece a $\mathbb{K}^m$. Debemos expresarlo como combinación lineal de la base canónica $E_m = \{e'_1, e'_2, \dots, e'_m\}$:

$$T_A(e_j) = a_{1j}e'_1 + a_{2j}e'_2 + \dots + a_{mj}e'_m = \sum_{i=1}^{m} a_{ij} e'_i$$

Por definición de vector de coordenadas, extraemos los escalares de esta combinación lineal para formar una columna:

$$[T_A(e_j)]_{E_m} = \begin{pmatrix} a_{1j} \\ a_{2j} \\ \vdots \\ a_{mj} \end{pmatrix}$$


Hemos demostrado que para todo $j \in \{1, 2, \dots, n\}$, la $j$-ésima columna de la matriz asociada $[T_A]_{E_n, E_m}$ es exactamente igual a la $j$-ésima columna de la matriz original $A$.

Dado que dos matrices son iguales si y solo si todas sus columnas correspondientes son idénticas, concluimos que:

$$[T_A]_{E_n, E_m} = A \quad \blacksquare$$

