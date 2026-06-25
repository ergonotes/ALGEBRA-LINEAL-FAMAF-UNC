Sea $V = \mathbb{R}^3$.
- **Base de partida (Canónica):** $\mathcal{B} = \{e_1, e_2, e_3\}$, donde $e_1 = (1, 0, 0)$, $e_2 = (0, 1, 0)$ y $e_3 = (0, 0, 1)$.
    
- **Base de llegada:** $\mathcal{B}' = \{w_1, w_2, w_3\}$, donde $w_1 = (1, 1, 1)$, $w_2 = (1, 1, 0)$ y $w_3 = (1, 0, 0)$.
    
Hallar la matriz de cambio de base $[\text{Id}_V]_{\mathcal{B}\mathcal{B}'}$ de $\mathcal{B}$ a $\mathcal{B}'$.

Para ello, debemos encontrar las coordenadas de cada $e_n$ expresado como combinación lineal de $\mathcal{B}'$.

Buscamos escalares tales que $e_1 = c_{11}w_1 + c_{21}w_2 + c_{31}w_3$.

$$(1, 0, 0) = c_{11}(1, 1, 1) + c_{21}(1, 1, 0) + c_{31}(1, 0, 0)$$

$$(1, 0, 0) = (c_{11} + c_{21} + c_{31}, c_{11} + c_{21}, c_{11})$$

- Componente $z$: $c_{11} = 0$
    
- Componente $y$: $c_{11} + c_{21} = 0 \implies 0 + c_{21} = 0 \implies c_{21} = 0$
    
- Componente $x$: $c_{11} + c_{21} + c_{31} = 1 \implies 0 + 0 + c_{31} = 1 \implies c_{31} = 1$
    
    $$[e_1]_{\mathcal{B}'} = \begin{pmatrix} 0 \\ 0 \\ 1 \end{pmatrix}$$
    

Para el siguiente vector:
$$(0, 1, 0) = c_{12}(1, 1, 1) + c_{22}(1, 1, 0) + c_{32}(1, 0, 0)$$

$$(0, 1, 0) = (c_{12} + c_{22} + c_{32}, c_{12} + c_{22}, c_{12})$$

Igualando:

- Componente $z$: $c_{12} = 0$
    
- Componente $y$: $c_{12} + c_{22} = 1 \implies 0 + c_{22} = 1 \implies c_{22} = 1$
    
- Componente $x$: $c_{12} + c_{22} + c_{32} = 0 \implies 0 + 1 + c_{32} = 0 \implies c_{32} = -1$
    
    $$[e_2]_{\mathcal{B}'} = \begin{pmatrix} 0 \\ 1 \\ -1 \end{pmatrix}$$
    

**Para el tercer vector ($e_3$):**

$$(0, 0, 1) = c_{13}(1, 1, 1) + c_{23}(1, 1, 0) + c_{33}(1, 0, 0)$$

$$(0, 0, 1) = (c_{13} + c_{23} + c_{33}, c_{13} + c_{23}, c_{13})$$

Igualando:

- Componente $z$: $c_{13} = 1$
    
- Componente $y$: $c_{13} + c_{23} = 0 \implies 1 + c_{23} = 0 \implies c_{23} = -1$
    
- Componente $x$: $c_{13} + c_{23} + c_{33} = 0 \implies 1 - 1 + c_{33} = 0 \implies c_{33} = 0$
    
    $$[e_3]_{\mathcal{B}'} = \begin{pmatrix} 1 \\ -1 \\ 0 \end{pmatrix}$$
    

Apilamos los tres vectores columna que acabamos de descubrir:

$$[\text{Id}_V]_{\mathcal{B}\mathcal{B}'} = \begin{pmatrix} 0 & 0 & 1 \\ 0 & 1 & -1 \\ 1 & -1 & 0 \end{pmatrix}$$


Como partimos de la base canónica $\mathcal{B}$, el vector de coordenadas de cualquier vector geométrico $(x, y, z)$ es trivialmente él mismo:

$$[v]_{\mathcal{B}} = \begin{pmatrix} x \\ y \\ z \end{pmatrix}$$

Aplicamos la [[D-Composición de Transformaciones Lineales]] multiplicando la matriz por este vector genérico para hallar la fórmula:

$$[v]_{\mathcal{B}'} = [\text{Id}_V]_{\mathcal{B}\mathcal{B}'} \cdot [v]_{\mathcal{B}}$$

$$[v]_{\mathcal{B}'} = \begin{pmatrix} 0 & 0 & 1 \\ 0 & 1 & -1 \\ 1 & -1 & 0 \end{pmatrix} \begin{pmatrix} x \\ y \\ z \end{pmatrix}$$

Multiplicamos fila por columna algebraicamente, y tenemos:

$$[v]_{\mathcal{B}'} = \begin{pmatrix} z \\ y - z \\ x - y \end{pmatrix}$$

****
Para comprobar que nuestra fórmula general es infalible, reconstruimos el vector original usando las nuevas coordenadas algebraicas como los escalares que multiplican a los vectores de $\mathcal{B}'$:

$$v = \alpha_1 w_1 + \alpha_2 w_2 + \alpha_3 w_3$$

Sustituimos las coordenadas obtenidas:

$$v = z(1, 1, 1) + (y - z)(1, 1, 0) + (x - y)(1, 0, 0)$$

Distribuimos escalarmente:

$$v = (z, z, z) + (y - z, y - z, 0) + (x - y, 0, 0)$$
$$v = (x, y, z) \quad \blacksquare$$

Vemos que la igualdad se cumple.