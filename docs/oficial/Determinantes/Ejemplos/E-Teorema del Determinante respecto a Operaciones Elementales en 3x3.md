
Definamos nuestra matriz base $A$ y calculemos su determinante y sus cofactores de la fila 3:

$$A = \begin{pmatrix} 1 & 2 & 1 \\ 0 & 1 & 3 \\ 2 & 1 & 1 \end{pmatrix}$$

Luego  
- $C_{31} = +\det \begin{pmatrix} 2 & 1 \\ 1 & 3 \end{pmatrix} = 6 - 1 = 5$
    
- $C_{32} = -\det \begin{pmatrix} 1 & 1 \\ 0 & 3 \end{pmatrix} = -(3 - 0) = -3$
    
- $C_{33} = +\det \begin{pmatrix} 1 & 2 \\ 0 & 1 \end{pmatrix} = 1 - 0 = 1$
    

$$\det(A) = a_{31}C_{31} + a_{32}C_{32} + a_{33}C_{33} = 2(5) + 1(-3) + 1(1) = 10 - 3 + 1 = \mathbf{8}$$

### **Caso 1. Escalar una fila ($A \xrightarrow{cF_r} B$)**

**Operación:** Multiplicamos la Fila 3 por un escalar $c = 10$.

$$B = \begin{pmatrix} 1 & 2 & 1 \\ 0 & 1 & 3 \\ \mathbf{20} & \mathbf{10} & \mathbf{10} \end{pmatrix}$$

Desarrollamos el determinante por la misma fila que alteramos (la fila 3). Como las demás filas (1 y 2) están intactas, los cofactores $C_{3j}$ de la matriz $B$ **son exactamente los mismos** que los de la matriz $A$.

$$\det(B) = b_{31}C_{31} + b_{32}C_{32} + b_{33}C_{33}$$

$$\det(B) = \mathbf{20}(5) + \mathbf{10}(-3) + \mathbf{10}(1)$$

Sacamos el $10$ como factor común, $\det B = c \sum_j a_{rj} C_{rj}$ en la demostración general

$$\det(B) = 10 \cdot [2(5) + 1(-3) + 1(1)]$$

$$\det(B) = 10 \cdot [\det(A)] = 10 \cdot 8 = \mathbf{80}$$

Vemos cómo el escalar "sale" limpiamente de la sumatoria.

### **Caso 3. Permutar dos filas ($A \xrightarrow{F_r \leftrightarrow F_s} B$)**

**Operación:** Intercambiamos la Fila 1 y la Fila 2.

$$B = \begin{pmatrix} \mathbf{0} & \mathbf{1} & \mathbf{3} \\ \mathbf{1} & \mathbf{2} & \mathbf{1} \\ 2 & 1 & 1 \end{pmatrix}$$

La clave de la demostración es desarrollar por la fila $k$ que **no se movió** (en este caso, la fila 3). Las entradas son $b_{3j} = a_{3j}$, es decir, los números $(2, 1, 1)$.

¿Pero qué le pasó a los cofactores de la fila 3? Vamos a calcularlos en la nueva matriz $B$:

- $C_{31}^B = +\det \begin{pmatrix} 1 & 3 \\ 2 & 1 \end{pmatrix} = 1 - 6 = \mathbf{-5}$ (Nota: es el negativo del $C_{31}^A = 5$)
    
- $C_{32}^B = -\det \begin{pmatrix} 0 & 3 \\ 1 & 1 \end{pmatrix} = -(0 - 3) = \mathbf{3}$ (Nota: es el negativo del $C_{32}^A = -3$)
    
- $C_{33}^B = +\det \begin{pmatrix} 0 & 1 \\ 1 & 2 \end{pmatrix} = 0 - 1 = \mathbf{-1}$ (Nota: es el negativo del $C_{33}^A = 1$)
    

Al permutar las filas de arriba, invertimos el determinante de todas las submatrices $2 \times 2$. Por lo tanto, $M_{kj}^B = -M_{kj}^A$.

$$\det(B) = 2(-5) + 1(3) + 1(-1) = -10 + 3 - 1 = \mathbf{-8}$$

Exactamente $-\det(A)$.

### **Caso 2. Sumar un múltiplo de otra fila ($A \xrightarrow{F_r + cF_s} B$)**

**Operación:** A la Fila 3 le sumamos la Fila 1 multiplicada por $100$ ($F_3 \to F_3 + 100 F_1$).

Las nuevas entradas de la fila 3 serán: $2 + 100(1) = 102$, $1 + 100(2) = 201$, $1 + 100(1) = 101$.

$$B = \begin{pmatrix} 1 & 2 & 1 \\ 0 & 1 & 3 \\ \mathbf{102} & \mathbf{201} & \mathbf{101} \end{pmatrix}$$

Desarrollamos por la alterada fila 3. Como las filas 1 y 2 están intactas, los cofactores son idénticos a los de $A$ ($5, -3, 1$).

$$\det(B) = 102(5) + 201(-3) + 101(1)$$

Ahora separamos los números en la suma original $(a_{rj} + ca_{sj})$:

$$\det(B) = (2 + 100 \cdot 1)(5) + (1 + 100 \cdot 2)(-3) + (1 + 100 \cdot 1)(1)$$

Por propiedad distributiva, reagrupamos todo en dos grandes bloques:

$$\det(B) = \underbrace{[2(5) + 1(-3) + 1(1)]}_{\text{Mismos componentes que } A} + \underbrace{100 \cdot [1(5) + 2(-3) + 1(1)]}_{\text{El "extra" } D}$$

 Vemos

$D = 100 \cdot [5 - 6 + 1] = 100 \cdot [\mathbf{0}] = 0$

El resultado es cero porque los números que se están multiplicando con los cofactores de la fila 3 son $(1, 2, 1)$, que son los elementos de la Fila 1

Geométricamente, ese segundo bloque está calculando el determinante de la matriz $A'$ donde hemos reemplazado la fila 3 con una copia de la fila 1:

$$A' = \begin{pmatrix} 1 & 2 & 1 \\ 0 & 1 & 3 \\ \mathbf{1} & \mathbf{2} & \mathbf{1} \end{pmatrix}$$

Como tiene dos filas repetidas, su determinante colapsa a cero.

$$\det(B) = \det(A) + 100 \cdot (0) = \mathbf{8}$$