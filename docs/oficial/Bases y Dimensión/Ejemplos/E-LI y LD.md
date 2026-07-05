La regla algebraica fundamental dice que un conjunto de vectores es **Dependiente** si puedes escribir al menos uno de ellos como una fórmula matemática usando los demás (es decir, una combinación lineal). Si es imposible hacer esto, son **Independientes**.
****
### Ejemplo 1. $v_1 = (1, 0)$ y $v_2 = (0, 1)$
Vemos
$$(1, 0) = k \cdot (0, 1)$$
$$(1, 0) = (0, k)$$
Esto genera un absurdo matemático, porque $1$ nunca será igual a $0$. Es imposible escribir uno en función del otro. Por lo tanto, son **Independientes**.
### Ejemplo 2. $u_1 = (2, 4)$ y $u_2 = (4, 8)$
Es claro
$$u_2 = 2 \cdot u_1$$

$$(4, 8) = 2 \cdot (2, 4)$$

$$(4, 8) = (4, 8)$$
Fabricamos un vector a partir del otro, y por tanto son **dependientes**
### Ejemplo 3. $w_1 = (1, 0)$, $w_2 = (0, 1)$ y $w_3 = (3, 5)$

Podemos mostrar que podemos fabricar a $w_3$ combinando los otros dos. La ecuación algebraica a resolver es:
$$w_3 = a \cdot w_1 + b \cdot w_2$$

Sustituyendo:

$$(3, 5) = a(1, 0) + b(0, 1)$$

$$(3, 5) = (a, 0) + (0, b)$$

$$(3, 5) = (a, b)$$

Vemos claramente que si elegimos $a = 3$ y $b = 5$. Se demuestra que hay redundancia y son **Dependientes**.