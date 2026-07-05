**Teorema.** Sea $T: V \to V$ operador lineal **diagonalizable** ($V$ espacio vectorial, con $\dim V < \infty$).

Si $\lambda_1, \dots, \lambda_k$o son autovalores distintos de $T \implies$ el polinomio característico de $T$ es de la forma:

$$

P_T(x) = (x - \lambda_1)^{d_1} \cdot \dots \cdot (x - \lambda_k)^{d_k} \quad \ \ \text{con } d_i = \dim(V_{\lambda_i})

$$
****
**Demostración.** (Leer con detenimiento)
Sabemos que [[E-Una matriz se puede diagonalizar si y solo si logras juntar suficientes autovectores independientes como para armar una base completa del espacio]], y como $T$ es diagonalizable, existe una base $\beta$ del espacio vectorial $V$ tal que la matriz asociada $[T]_\beta$ es diagonal.

Vamos a **reordenar esta base**. Agrupando todos los autovectores que corresponden al autovalor $\lambda_1$, luego los de $\lambda_2$, y así sucesivamente hasta $\lambda_k$.

$$\beta = \{v_{1,1}, \dots, v_{1,d_1}, v_{2,1}, \dots, v_{2,d_2}, \dots, v_{k,1}, \dots, v_{k,d_k}\}$$

Aquí, $d_i$ es simplemente la cantidad de autovectores asociados a $\lambda_i$ que hay en la base. Además, se cumple que $T(v_{i,j}) = \lambda_i v_{i,j}$.

Luego si tomamos cualquier vector $v$ en el espacio $V$, lo podemos escribir como una combinación lineal de todos los elementos de la base $\beta$.

$$v = w_1 + w_2 + \dots + w_k$$

Donde cada $w_i$ representa la suma de los componentes asociados al autovalor $\lambda_i$ (es decir, $w_i = \sum c_{ij} v_{ij}$).

Como cada $v_{ij}$ en ese bloque es autovector de $\lambda_i$, al aplicar la transformación $T$ por linealidad, ocurre algo muy conveniente:

$$T(v) = \lambda_1 w_1 + \lambda_2 w_2 + \dots + \lambda_k w_k$$


Ahora, el objetivo es probar que el autoespacio $V_{\lambda_j}$ está generado **exclusivamente** por los vectores $\{v_{j,1}, \dots, v_{j,d_j}\}$.

Para probar esto, se toma un vector $v$ que pertenece al autoespacio $V_{\lambda_j}$. Por definición, eso significa que $T(v) = \lambda_j v$.

Y calculamos $T(v)$ de dos maneras distintas para forzar una igualdad:

- **Forma 1 (por linealidad):** $T(v) = \lambda_1 w_1 + \dots + \lambda_k w_k$
    
- **Forma 2 (por ser autovector):** $T(v) = \lambda_j v = \lambda_j (w_1 + \dots + w_k) = \lambda_j w_1 + \dots + \lambda_j w_k$
    
Al restar ambas expresiones, el resultado debe ser cero:

$$0 = (\lambda_1 - \lambda_j)w_1 + \dots + (\lambda_j - \lambda_j)w_j + \dots + (\lambda_k - \lambda_j)w_k$$

En la ecuación anterior, el término con $w_j$ se anula porque $(\lambda_j - \lambda_j) = 0$.

Nos quedan sumas de vectores $w_i$ multiplicados por escalares $(\lambda_i - \lambda_j)$ que son distintos de cero (porque los autovalores son distintos).

Para que la ecuación se cumpla, todos los $w_i$ (salvo $w_j$) deben ser obligatoriamente cero.

Por lo tanto, $v = w_j$. Esto prueba que cualquier vector $v$ en el autoespacio $V_{\lambda_j}$ es simplemente una combinación lineal de $\{v_{j,1}, \dots, v_{j,d_j}\}$.

Como estos $d_j$ vectores son independientes (porque forman parte de la base original $\beta$), la dimensión del autoespacio es exactamente:

$$\dim(V_{\lambda_j}) = d_j$$


Luego la matriz $[T]_\beta$ se dibuja en la imagen como una matriz diagonal por bloques. Cada bloque es de tamaño $d_i \times d_i$ y tiene la forma $\lambda_i I_{d_i}$ (donde $I$ es la matriz identidad).

Finalmente, al calcular el polinomio característico con el determinante $\det(xI - T)$, y sabiendo que [[D-El determinante de una matriz triangular es el producto de sus elementos diagonales]], llegamos a la fórmula final:

$$P_T(x) = (x - \lambda_1)^{d_1} \cdot \dots \cdot (x - \lambda_k)^{d_k}$$