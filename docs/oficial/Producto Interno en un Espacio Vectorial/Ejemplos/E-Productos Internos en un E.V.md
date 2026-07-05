**Ejemplo 1. El producto interno canónico en $\mathbb{R}^n$.**

En $\mathbb{R}^n$ existe un producto interno estándar que se llama **producto interno canónico** (también conocido comúnmente como producto escalar). Para los vectores $u = (x_1, \dots, x_n)$ y $v = (y_1, \dots, y_n)$ en $\mathbb{R}^n$, está definido como la suma de los productos de sus componentes correspondientes:

$$ \langle u, v \rangle = \sum_{i=1}^n x_i y_i = x_1 y_1 + x_2 y_2 + \dots + x_n y_n $$
****
**Ejemplo 2. Un producto interno alternativo en $\mathbb{R}^2$.**

Para los vectores $u = (x_1, x_2)$ y $v = (y_1, y_2)$ en $\mathbb{R}^2$, se define la siguiente operación:

$$ \langle u, v \rangle = x_1 y_1 - x_2 y_1 - x_1 y_2 + 4x_2 y_2 $$

Para verificar si cumple la condición de ser **definida positiva** (Axioma 3), evaluamos el producto del vector $u$ consigo mismo:

$$ \langle u, u \rangle = x_1^2 - 2x_1 x_2 + 4x_2^2 $$

Completando cuadrados, la expresión se puede reescribir como:

$$ \langle u, u \rangle = (x_1 - x_2)^2 + 3x_2^2 $$

Como toda suma de números reales al cuadrado es mayor o igual a cero, se tiene que $\langle u, u \rangle > 0$ siempre que $u \neq 0$ (y $\langle u, u \rangle = 0$ si y solo si $u = 0$). Los axiomas 1 y 2 (Linealidad y Simetría) también se pueden verificar fácilmente, por lo que esta fórmula define un producto interno válido en $\mathbb{R}^2$ distinto al canónico.