**Definición.** Sea $V$ espacio vectorial sobre $K$ y $v_1, \ldots, v_n$ vectores en $V$. Dado $v \in V$, diremos que $v$ es combinación lineal de los $v_1, \ldots, v_n$ si existen escalares $\lambda_1, \ldots, \lambda_n$ en $K$, tal que
$$v = \lambda_1 v_1 + \ldots + \lambda_n v_n.$$
****
#### **Observación**. **La pregunta de si un vector $v = (b_1, \ldots, b_m) \in \mathbb{K}^m$ es combinación lineal de vectores $v_1, \ldots, v_n \in \mathbb{K}^m$ se resuelve con un sistema de ecuaciones lineales** 
Si $v_i = (a_{1i}, \ldots, a_{mi})$, para $1 \leq i \leq n$, entonces $v = \lambda_1 v_1 + \ldots + \lambda_n v_n$ se traduce, en coordenadas, a
$$ (b_1, \ldots, b_m) = \lambda_1(a_{11}, \ldots, a_{m1}) + \ldots + \lambda_n(a_{1n}, \ldots, a_{mn}) $$
$$ = (\lambda_1 a_{11} + \ldots + \lambda_n a_{1n}, \ldots, \lambda_1 a_{m1} + \ldots + \lambda_n a_{mn}). $$
Luego, $v$ es combinación lineal de los vectores $v_1, \ldots, v_n \in \mathbb{K}^n$ si y sólo si se tiene solución el siguiente sistema de ecuaciones con incógnitas $\lambda_1, \ldots, \lambda_n$:
$$ a_{11}\lambda_1 + a_{12}\lambda_2 + \ldots + a_{1n}\lambda_n = b_1 $$
$$ \vdots $$
$$ a_{m1}\lambda_1 + a_{m2}\lambda_2 + \ldots + a_{mn}\lambda_n = b_m $$