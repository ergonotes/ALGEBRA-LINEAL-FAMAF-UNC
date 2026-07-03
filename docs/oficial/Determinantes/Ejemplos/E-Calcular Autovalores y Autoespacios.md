**Ejemplo 1.** Tenemos una transformación lineal $T: \mathbb{R}^2 \to \mathbb{R}^2$ definida por la siguiente regla:

$$T(x,y) = (2x+3y, 2x+y)$$

Extraemos los coeficientes de $x$ e $y$ para armar la matriz asociada a la transformación (en la base canónica), a la cual llamaremos $A$:

$$A = \begin{pmatrix} 2 & 3 \\ 2 & 1 \end{pmatrix}$$

Para hallar los autovalores, debemos resolver la ecuación $\det(A - \lambda I) = 0$. Primero planteamos la matriz restando $\lambda$ a la diagonal principal:

$$\det \begin{pmatrix} 2 - \lambda & 3 \\ 2 & 1 - \lambda \end{pmatrix} = 0$$

Resolvemos el determinante de $2 \times 2$ :

$$(2 - \lambda)(1 - \lambda) - (3 \cdot 2) = 0$$

$$2 - 2\lambda - \lambda + \lambda^2 - 6 = 0$$

$$\lambda^2 - 3\lambda - 4 = 0$$

Resolvemos la cuadrática:

$$(\lambda - 4)(\lambda + 1) = 0$$

De aquí concluimos que los autovalores de la transformación son:

- **$\lambda_1 = -1$**
    
- **$\lambda_2 = 4$**
    
Un autoespacio es el conjunto de todos los vectores que están asociados a un autovalor específico (más el vector nulo). Se calcula resolviendo el sistema homogéneo $(A - \lambda I)v = 0$ para cada autovalor. Es decir, buscamos el núcleo de la transformación.

**Autoespacio para $\lambda = -1$ (Llamado $E_{-1}$):**

1. Reemplazamos $\lambda = -1$ en la matriz con la variable en la diagonal:
    
    $$\begin{pmatrix} 2 - (-1) & 3 \\ 2 & 1 - (-1) \end{pmatrix} = \begin{pmatrix} 3 & 3 \\ 2 & 2 \end{pmatrix}$$
    
2. Planteamos el sistema de ecuaciones para un vector $(x,y)$:
    
    $$\begin{pmatrix} 3 & 3 \\ 2 & 2 \end{pmatrix} \begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix}$$
    
3. Ambas filas nos dan información equivalente o redundante (por ejemplo, la primera fila nos dice que $3x + 3y = 0$). Si dividimos todo por 3, llegamos a la condición:
    
    $$x = -y$$
    
4. Esto significa que cualquier vector de este autoespacio tiene su primera coordenada como el negativo de la segunda. El espacio está generado por el vector base $(-1, 1)$:
    
    $$E_{-1} = \text{gen} \left\{ \begin{pmatrix} -1 \\ 1 \end{pmatrix} \right\}$$
    

**Autoespacio para $\lambda = 4$ (Llamado $E_4$):**

1. Reemplazamos $\lambda = 4$ en la matriz:
    
    $$\begin{pmatrix} 2 - 4 & 3 \\ 2 & 1 - 4 \end{pmatrix} = \begin{pmatrix} -2 & 3 \\ 2 & -3 \end{pmatrix}$$
    
2. Planteamos el sistema de ecuaciones:
    
    $$\begin{pmatrix} -2 & 3 \\ 2 & -3 \end{pmatrix} \begin{pmatrix} x \\ y \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix}$$
    
3. Tomamos la primera ecuación y despejamos $x$:
    
    $$-2x + 3y = 0 \implies 2x = 3y \implies x = \frac{3}{2}y$$
    
4. Para evitar fracciones al elegir un vector representativo, podemos darle a $y$ el valor de $2$, lo que automáticamente hace que $x$ valga $3$. El espacio está generado por el vector $(3, 2)$:
    
    $$E_{4} = \text{gen} \left\{ \begin{pmatrix} 3 \\ 2 \end{pmatrix} \right\}$$