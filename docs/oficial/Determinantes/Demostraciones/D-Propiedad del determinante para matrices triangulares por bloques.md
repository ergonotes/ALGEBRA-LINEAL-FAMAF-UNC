Lema: Sean $A \in M_{r \times r}(\mathbb{K})$, $B \in M_{r \times s}(\mathbb{K})$ y $C \in M_{s \times s}(\mathbb{K})$ matrices de bloques. $\Rightarrow \det \begin{pmatrix} A & B \\ 0 & C \end{pmatrix} = \det(A)\det(C)$
****
**Demostración**. Sea $R$ la Matriz Escalonada Reducida por Filas (MERF) de $C$. Entonces existen matrices elementales $E_1, E_2, \dots, E_k$ de tamaño $s \times s$ tales que $C = E_1 E_2 \dots E_k R$. 

Podemos factorizar la matriz de bloques original de la siguiente manera, debido a la definición de producto de matrices: $$\begin{pmatrix} A & B \\ 0 & C \end{pmatrix} = \begin{pmatrix} \text{Id}_r & 0 \\ 0 & E_1 \end{pmatrix} \dots \begin{pmatrix} \text{Id}_r & 0 \\ 0 & E_k \end{pmatrix} \begin{pmatrix} A & B \\ 0 & R \end{pmatrix}$$

Por la propiedad multiplicativa del determinante, (**El determinante del producto es el producto de los determinantes**) se extrae el determinante de cada factor:
$$\det \begin{pmatrix} A & B \\ 0 & C \end{pmatrix} = \det(E_1) \dots \det(E_k) \cdot \det \begin{pmatrix} A & B \\ 0 & R \end{pmatrix}$$
  
Dividimos el análisis en dos casos posibles:

Caso 1: Si $C$ no es invertible $\Rightarrow R$ posee al menos una fila nula.$\Rightarrow$ La matriz por bloques completa $\begin{pmatrix} A & B \\ 0 & R \end{pmatrix}$ tiene al menos una fila completamente nula en la parte inferior $\Rightarrow \det \begin{pmatrix} A & B \\ 0 & R \end{pmatrix} = 0$.$\Rightarrow \det \begin{pmatrix} A & B \\ 0 & C \end{pmatrix} = \det(E_1) \dots \det(E_k) \cdot 0 = 0$. Como $C$ no es invertible, sabemos que $\det(C) = 0$, por lo que se verifica trivialmente la igualdad $0 = \det(A) \cdot 0$.

  

Caso 2: Si $C$ es invertible $\Rightarrow R = \text{Id}_s$. Agrupando los determinantes de las matrices elementales, sabemos que $\det(C) = \det(E_1) \dots \det(E_k) \det(\text{Id}_s) = \det(E_1) \dots \det(E_k)$. Sustituimos en nuestra ecuación principal: $\det \begin{pmatrix} A & B \\ 0 & C \end{pmatrix} = \det(C) \cdot \det \begin{pmatrix} A & B \\ 0 & \text{Id}_s \end{pmatrix}$

  

Aplicando operaciones elementales por fila del tipo $F_i \leftarrow F_i + cF_j$, podemos usar las filas del bloque $\text{Id}_s$ inferior para anular todos los coeficientes del bloque rectangular $B$ superior. Dado que estas operaciones específicas no alteran el valor del determinante: $\det \begin{pmatrix} A & B \\ 0 & \text{Id}_s \end{pmatrix} = \det \begin{pmatrix} A & 0 \\ 0 & \text{Id}_s \end{pmatrix} = \det(A) \cdot \det(\text{Id}_s) = \det(A)$

  

Sustituyendo este último resultado, llegamos a la demostración de la propiedad: $\Rightarrow \det \begin{pmatrix} A & B \\ 0 & C \end{pmatrix} = \det(C) \cdot \det(A) = \det(A)\det(C)$ $\blacksquare$