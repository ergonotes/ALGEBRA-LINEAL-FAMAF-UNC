**Proposición**. Sea $A \in M_n(\mathbb{K})$ matriz triangular superior cuyos elementos en la diagonal son $d_1, \dots, d_n$. Entonces $\det A = d_1 \cdot d_2 \cdot \dots \cdot d_n$.
****
**Demostración.** Podemos demostrar el resultado por inducción sobre $n$: es claro que si $n=1$, es decir si $A=[d_1]$, el determinante vale $d_1$. Por otro lado, si $n > 1$, observemos que $A(1|1)$ es también triangular superior con valores $d_2, \dots, d_n$ en la diagonal principal. Entonces, usamos la definición de la fórmula del determinante visto en el inciso de [[1.Determinante]], y observamos que el desarrollo por la primera columna solo tiene un término, pues esta columna solo tiene un coeficiente no nulo, el $d_1$ en la primera posición. Por lo tanto,
$$
\det(A) = d_1 \det(A(1|1)) \stackrel{(\text{HI})}{=} d_1 \cdot (d_2 \cdot \dots \cdot d_n). \ \square
$$
****
A la hora de comprobar la proposición, podemos usar el desarrollo por primera columna, o el desarrollo de Laplace.