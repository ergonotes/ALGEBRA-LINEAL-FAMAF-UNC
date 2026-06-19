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
**Ejemplo 2.** 