**Ejemplo 1**. Sea $T: \mathbb{R}^3 \to \mathbb{R}$, definida
$$
T(x, y, z) = x + 2y + 3z.
$$

Encontrar una base del núcleo y de la imagen.
****
**Solución**. Es claro que como $T$ no es $0$, la imagen es todo $\mathbb{R}$ (y por lo tanto cualquier $r \in \mathbb{R}, r \neq 0$ es base de la imagen).

Con respecto al núcleo, debemos encontrar una base del subespacio
$$
\text{Nu}(T) = \{(x, y, z) : x + 2y + 3z = 0\}.
$$
Como $x + 2y + 3z = 0 \iff x = -2y - 3z$, luego,

$$(1) \ \ \ \quad 
\text{Nu}(T) = \{(-2s - 3t, s, t) : s, t \in \mathbb{R}\}.
$$
Ahora bien, $(-2s - 3t, s, t) = s(-2, 1, 0) + t(-3, 0, 1)$, por lo tanto
$$
\text{Nu}(T) = \langle (-2, 1, 0), (-3, 0, 1) \rangle,
$$
y como $(-2, 1, 0), (-3, 0, 1)$ son **LI**, tenemos que forman una base del núcleo. $\square$
****
La expresión $(1)$, que depende de dos parámetros ($s$ y $t$) que son independientes entre ellos, es llamada la *descripción paramétrica* del núcleo.
****
**Ejemplo 2.** Sea $T: \mathbb{R}^3 \to \mathbb{R}^4$, definida
$$
T(x, y, z) = (x + y, x + 2y + z, 3y + 3z, 2x + 4y + 2z).
$$
(1) Describir $\text{Nu}(T)$ en forma paramétrica y dar una base.
(2) Describir $\text{Im}(T)$ en forma paramétrica y dar una base.
****
**Solución**. Observemos que
$$
\text{Nu}(T) = \{(x, y, z) \in \mathbb{R}^3 : (x + y, x + 2y + z, 3y + 3z, 2x + 4y + 2z) = (0, 0, 0, 0)\}.
$$
Por lo tanto, describir el núcleo de $T$ se reduce a encontrar las soluciones de una sistema de ecuaciones lineales homogéneo, y la matriz asociada a este sistema es.
$$
A = \begin{bmatrix}
1 & 1 & 0 \\
1 & 2 & 1 \\
0 & 3 & 3 \\
2 & 4 & 2
\end{bmatrix}
$$

Por otro lado,
$$
\text{Im}(T) = \{(y_1, y_2, y_3, y_4) \in \mathbb{R}^4 : (x + y, x + 2y + z, 3y + 3z, 2x + 4y + 2z) = (y_1, y_2, y_3, y_4)\}
$$
$$
= \left\{ (y_1, y_2, y_3, y_4) \in \mathbb{R}^4 : A \begin{bmatrix} x \\ y \\ z \end{bmatrix} = \begin{bmatrix} y_1 \\ y_2 \\ y_3 \\ y_4 \end{bmatrix} \right\}.
$$

Por lo tanto, y haciendo abuso de notificación,
$$
\text{Nu}(T) = \{v = (x, y, z) : A \cdot v = 0\}
$$
$$
\text{Im}(T) = \{y = (y_1, y_2, y_3, y_4) : \text{tal que } \exists v \in \mathbb{R}^3, A \cdot v = y\}
$$

En ambos casos, la solución depende de resolver el sistema de ecuaciones cuya matriz asociada es $A$:
$$
\left[ \begin{array}{ccc|c} 1 & 1 & 0 & y_1 \\ 1 & 2 & 1 & y_2 \\ 0 & 3 & 3 & y_3 \\ 2 & 4 & 2 & y_4 \end{array} \right] \xrightarrow[\xrightarrow{F_4-2F_1}]{F_2-F_1} \left[ \begin{array}{ccc|c} 1 & 1 & 0 & y_1 \\ 0 & 1 & 1 & -y_1+y_2 \\ 0 & 3 & 3 & y_3 \\ 0 & 2 & 2 & -2y_1+y_4 \end{array} \right] \xrightarrow[\xrightarrow{F_4-2F_2}]{\xrightarrow{F_1-F_2, F_3-3F_2}} \left[ \begin{array}{ccc|c} 1 & 0 & -1 & 2y_1-y_2 \\ 0 & 1 & 1 & -y_1+y_2 \\ 0 & 0 & 0 & 3y_1-3y_2+y_3 \\ 0 & 0 & 0 & -2y_2+y_4 \end{array} \right],
$$
es decir
$$
T(x, y, z) = (y_1, y_2, y_3, y_4) \iff \begin{cases} x-z = 2y_1-y_2 \\ y+z = -y_1+y_2 \\ 0 = 3y_1-3y_2+y_3 \\ 0 = -2y_2+y_4 \end{cases}
$$
Si hacemos $y_1=y_2=y_3=y_4=0$, entonces las soluciones del sistema describen el núcleo de $T$, es decir
$$
\text{Nu}(T) = \{(x, y, z) : x-z=0, y+z=0\} = \{(s, -s, s) : s \in \mathbb{R}\},
$$
que es la forma paramétrica. Una base del núcleo de $T$ es $(1, -1, 1)$.
Con respecto a la imagen de $T$ tenemos
$$
(y_1, y_2, y_3, y_4) \in \text{Im}(T) \iff \exists x, y, z \in \mathbb{R} \text{ tal que } 2y_1-y_2 = x-z, \ -y_1+y_2 = y+z; \text{ y } 0 = 3y_1-3y_2+y_3 \text{ y } 0 = -2y_2+y_4.
$$
Como variando los valores de $x, y, z$ es posible obtener, para cualesquiera valores de $y_1, y_2, y_3, y_4$, $2y_1-y_2 = x-z$, $-y_1+y_2 = y+z$, tenemos

$$
(y_1, y_2, y_3, y_4) \in \text{Im}(T) \iff 0 = 3y_1-3y_2+y_3 \text{ y } 0 = -2y_2+y_4.
$$
Luego,
$$
\text{Im}(T) = \{(y_1, y_2, y_3, y_4) : \text{tal que } 0 = 3y_1-3y_2+y_3 \text{ y } 0 = -2y_2+y_4\}.
$$
Ahora bien,
$$
0 = -2y_2+y_4 \iff 2y_2 = y_4 \iff y_2 = \frac{1}{2}y_4.
$$
Por otro lado
$$
0 = 3y_1-3y_2+y_3 \iff 3y_1 = 3y_2-y_3 \iff y_1 = y_2 - \frac{1}{3}y_3 \iff y_1 = \frac{1}{2}y_4 - \frac{1}{3}y_3.
$$
Es decir, cambiando $y_3$ por $s$ e $y_4$ por $t$:
$$
\text{Im}(T) = \{(-\frac{1}{3}s + \frac{1}{2}t, \frac{1}{2}t, s, t) : s, t \in \mathbb{R}\}.
$$
Como $(-\frac{1}{3}s + \frac{1}{2}t, \frac{1}{2}t, s, t) = s(-\frac{1}{3}, 0, 1, 0) + t(\frac{1}{2}, \frac{1}{2}, 0, 1)$ el conjunto $\{(-\frac{1}{3}, 0, 1, 0), (\frac{1}{2}, \frac{1}{2}, 0, 1)\}$ es una base de $\text{Im}(T)$. $\square$