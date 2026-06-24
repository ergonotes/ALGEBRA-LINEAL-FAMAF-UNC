**Proposición**. Sea $V$ y $W$ espacios vectoriales de dimensión $n$ y $m$ respectivamente y sea $T: V \to W$ una transformación lineal. Sea $\mathcal{B} = \{v_1, \dots, v_n\}$ una base ordenada de $V$, y $\mathcal{B}' = \{w_1, \dots, w_m\}$ una base ordenada de $W$. Entonces

$$
[T]_{\mathcal{B}\mathcal{B}'}[v]_{\mathcal{B}} = [T(v)]_{\mathcal{B}'}, \quad \forall v \in V.
$$
****
**Demostración**. Si
$$
Tv_j = \sum_{i=1}^m a_{ij}w_i
$$
entonces $[T]_{ij} = a_{ij}$. Sea $v \in V$, entonces $v = x_1v_1 + \cdots + x_nv_n$ con $x_i \in \mathbb{K}$, por lo tanto
$$
[v]_{\mathcal{B}} = \begin{bmatrix} x_1 \\ \vdots \\ x_n \end{bmatrix}.
$$
Ahora bien,
$$
T(v) = T\left(\sum_{j=1}^n x_jv_j\right) = \sum_{j=1}^n x_jT(v_j) =  \sum_{j=1}^n x_j \sum_{i=1}^m a_{ij} w_i = \sum_{j=1}^n \sum_{i=1}^m x_j, a_{ij}, w_i
$$
**El intercambio de sumatorias**: Como son sumas finitas, se pueden reordenar libremente:

$$\sum_{j=1}^n \sum_{i=1}^m x_j, a_{ij}, w_i = \sum_{i=1}^m \sum_{j=1}^n x_j, a_{ij}, w_i = \sum_{i=1}^m \left(\sum_{j=1}^n a_{ij}, x_j\right) w_i$$
$$= \underbrace{\left(\sum_{j=1}^n a_{1j},x_j\right)}_{i=1} w_1 + \underbrace{\left(\sum_{j=1}^n a_{2j},x_j\right)}_{i=2} w_2 + \cdots + \underbrace{\left(\sum_{j=1}^n a_{mj},x_j\right)}_{i=m} w_m$$

Esto es una combinación lineal de la base $\mathcal{B}'$ y, por lo tanto,

$$[T(v)]_{\mathcal{B}'} = \begin{bmatrix} \sum_{j=1}^n a_{1j}x_j \\ \sum_{j=1}^n a_{2j}x_j \\ \vdots \\ \sum_{j=1}^n a_{mj}x_j \end{bmatrix}$$
Por otro lado,

$$
[T]_{\mathcal{B}\mathcal{B}'}[v]_{\mathcal{B}} = \begin{bmatrix} a_{11} & a_{12} & \cdots & a_{1n} \\ a_{21} & a_{22} & \cdots & a_{2n} \\ \vdots & \vdots & & \vdots \\ a_{m1} & a_{m2} & \cdots & a_{mn} \end{bmatrix} \begin{bmatrix} x_1 \\ x_2 \\ \vdots \\ x_n \end{bmatrix} = \begin{bmatrix} \sum_{j=1}^n a_{1j}x_j \\ \sum_{j=1}^n a_{2j}x_j \\ \vdots \\ \sum_{j=1}^n a_{mj}x_j \end{bmatrix}.
$$
De estas ecuaciones se deduce la formula del enunciado. $\square$







