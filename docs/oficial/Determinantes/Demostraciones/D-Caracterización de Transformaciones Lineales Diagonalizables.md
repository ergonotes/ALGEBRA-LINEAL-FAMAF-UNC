**Teorema**. 
**Premisas:**

- Sea $V$ un espacio vectorial de dimensión finita sobre un cuerpo $\mathbb{K}$.
    
- Sea $T: V \to V$ una transformación lineal.
    
- Sean $\lambda_1, \dots, \lambda_k$ los autovalores distintos de $T$.
    
- Sea $V_{\lambda_j}$ el autoespacio de $T$ correspondiente al autovalor $\lambda_j$.

**Equivalencias:**

Las siguientes tres afirmaciones son equivalentes:

1. $T$ es diagonalizable.
    
2. El polinomio característico de $T$ es $P_T(x) = (x - \lambda_1)^{d_1} \cdot \dots \cdot (x - \lambda_k)^{d_k}$, donde $d_j = \dim(V_{\lambda_j})$.
    
3. $\dim(V_{\lambda_1}) + \dots + \dim(V_{\lambda_k}) = \dim(V)$.
****
**Demostración.**
**$(1) \implies (2)$**

- Supongamos como hipótesis verdadera que $T$ es diagonalizable.
    
- Por el teorema de "[[D-Igualdad de Multiplicidades en Matrices Diagonalizables]]", sabemos que si un operador $T$ es diagonalizable y $\lambda_1, \dots, \lambda_k$ son sus autovalores distintos, su polinomio característico toma necesariamente la forma $P_T(x) = (x - \lambda_1)^{d_1} \cdot \dots \cdot (x - \lambda_k)^{d_k}$.
    
- Ese mismo teorema nos asegura que cada exponente corresponde a la dimensión del autoespacio asociado: $d_i = \dim(V_{\lambda_i})$.

**$(2) \implies (3)$**

- Supongamos ahora que el polinomio característico es $P_T(x) = (x - \lambda_1)^{d_1} \dots (x - \lambda_k)^{d_k}$ y que $d_j = \dim(V_{\lambda_j})$.
    
- Por definición de las notas, estamos trabajando con un espacio vectorial $V$ de dimensión finita $n$, y el polinomio característico surge del determinante de una matriz de tamaño $n \times n$.
    
- El grado total de ese polinomio característico debe ser obligatoriamente $n$. Al estar expresado de forma factorizada, la suma de todos sus exponentes nos da el grado total, por lo tanto: $d_1 + d_2 + \dots + d_k = n$.
    
- Sustituyendo nuestras equivalencias ($n = \dim(V)$ y $d_j = \dim V_{\lambda_j}$), obtenemos la ecuación $\dim(V_{\lambda_1}) + \dots + \dim(V_{\lambda_k}) = \dim(V)$. Hemos demostrado la afirmación 3.

**$(3) \implies (1)$**

- Supongamos finalmente que la suma de las dimensiones de todos los autoespacios nos da la dimensión del espacio total: $\dim(V_{\lambda_1}) + \dots + \dim(V_{\lambda_k}) = \dim(V)$.
    
- Cada autoespacio $V_{\lambda_j}$ aporta una cantidad $d_j$ de autovectores que son linealmente independientes entre sí para formar su propia base.
    
- Si tomamos todas esas pequeñas bases y las unimos, tendremos un total de vectores exactamente igual a $\dim(V)$.
    
- Sabemos que [[D-Autovalores distintos producen autovectores linealmente independientes]], ($\lambda_i \neq \lambda_j$), entonces los autovectores asociados a ellos son obligatoriamente linealmente independientes.
    
- Como tenemos $\dim(V)$ autovectores que además son linealmente independientes en su totalidad, estos forman una base completa del espacio $V$.
    
- Llegamos entonces a la definición crucial: $T$ es diagonalizable $\iff$ existe una base $\beta$ de $V$ formada por autovectores de $T$. Al haber logrado armar esa base, comprobamos que $T$ es diagonalizable, lo que equivale a la afirmación 1 y cierra nuestro ciclo lógico. 