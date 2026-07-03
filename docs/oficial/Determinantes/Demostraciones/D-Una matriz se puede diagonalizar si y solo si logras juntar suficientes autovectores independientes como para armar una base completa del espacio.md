**Teorema.** Sea $T: V \to V$ una transformación lineal.

**$T$ es diagonalizable $\iff$ existe una base $\beta$ de $V$ formada por autovectores de $T$.**

**Es decir,** Existe una base $\beta = \{v_1, \dots, v_n\}$ de $V$ tal que $T(v_j) = \lambda_j v_j$ para algún escalar $\lambda_j \in K$.
****
**Demostración.**
($\impliedby$).
_Asumimos que existe la base de autovectores y demostramos que es diagonalizable._

- **Hipótesis:** Si $\beta = \{v_1, \dots, v_n\}$ es una base de $V$ y está conformada por autovectores, por definición se cumple que $T(v_j) = \lambda_j v_j$.
    
- **Desarrollo:** Al construir la matriz de la transformación en esta base, llamada $[T]_\beta$, las columnas corresponden a las coordenadas de estos transformados. Como $T(v_1)$ es $\lambda_1 v_1$ (y cero en el resto), $T(v_2)$ es $\lambda_2 v_2$, y así sucesivamente, la matriz resulta tener valores solo en su diagonal principal:
    
    $$[T]_\beta = \begin{pmatrix} \lambda_1 & 0 & \dots & 0 \\ 0 & \lambda_2 & \dots & 0 \\ \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & \dots & \lambda_n \end{pmatrix}$$
    
- **Conclusión:** Como $[T]_\beta$ es una matriz diagonal, queda demostrado que $T$ es diagonalizable.
    

($\implies$).
_Asumimos que es diagonalizable y demostramos que la base está formada por autovectores._

- **Hipótesis:** Si $T$ es diagonalizable, existe una base $\beta = \{v_1, \dots, v_n\}$ tal que la matriz asociada $[T]_\beta$ es una matriz diagonal:
    
    $$[T]_\beta = \begin{pmatrix} d_1 & \dots & 0 & \dots & 0 \\ 0 & \dots & \vdots & \dots & 0 \\ \vdots & \dots & d_j & \dots & \vdots \\ 0 & \dots & 0 & \dots & d_n \end{pmatrix}$$
    
- **Desarrollo:** Si observamos una columna cualquiera de esta matriz (la **$j$-ésima columna**), vemos que todos sus elementos son $0$ excepto el elemento en la posición de la diagonal, que es $d_j$. Esta columna representa las coordenadas del transformado $T(v_j)$ en la base $\beta$.
    
- Al reescribir estas coordenadas como una combinación lineal de los vectores de la base $\beta$, obtenemos:
    
    $$T(v_j) = 0 \cdot v_1 + \dots + d_j v_j + \dots + 0 \cdot v_n$$
    
    Lo cual se simplifica directamente a:
    
    $$T(v_j) = d_j v_j$$
    
Sabemos que los vectores de una base nunca pueden ser el vector nulo ($v_j \neq 0$). Por lo tanto, la ecuación $T(v_j) = d_j v_j$ nos dice expresamente que $d_j$ es un **autovalor** y que $v_j$ es su correspondiente **autovector**. Queda demostrado que la base $\beta$ está íntegramente formada por autovectores.