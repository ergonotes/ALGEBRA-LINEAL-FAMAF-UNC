- Supongamos que $S$ es un subespacio ([[1.1.3 Subespacios]]) de $\mathbb{R}^2$ y que contiene algún elemento $v$ no nulo. Entonces, para todo $\lambda \in \mathbb{R}$, $\lambda \cdot v \in S$. Si éstos son todos los elementos de $S$, entonces $S$ es un subespacio (que, gráficamente, resulta ser una recta que pasa por el origen).
Este último ejemplo descarta el caso del subespacio trivial ${ (0, 0) }$, que fue mencionado antes. En cambio, se toma un vector cualquiera $v \in \mathbb{R}^2$, con $v \ne 0$, dentro del subespacio $S$. Y como $S$ es un subespacio, al tomar cualquier escalar $\lambda \in \mathbb{R}$, se garantiza que $\lambda v$ también pertenece a $S$. Tomemos el ejemplo para explicar el ejemplo:
Supongamos que el subespacio $S$ contiene un vector no nulo:  
$$v = (2, 3) \in \mathbb{R}^2$$
Como $S$ es un subespacio, debe ser cerrado bajo multiplicación escalar. Eso significa que, **si tomas cualquier número real** $\lambda$, entonces el vector:  
$$\lambda v = \lambda (2, 3) = (2\lambda, 3\lambda)$$
también pertenece a $S$.
Esto geométricamente significa que el conjunto de todos los vectores $(2\lambda, 3\lambda)$, **cuando $\lambda$ recorre todos los reales**, **describe una recta en el plano**.
De hecho, ese conjunto es:  $${ (x, y) \in \mathbb{R}^2 \mid \exists \lambda \in \mathbb{R},\ x = 2\lambda,\ y = 3\lambda }$$Y se debe a que cuando multiplicas un vector fijo por escalares reales:
- Si $\lambda > 0$, obtienes vectores en la misma dirección.
- Si $\lambda < 0$, obtienes vectores en la dirección opuesta.
- Si $\lambda = 0$, obtienes el vector nulo.
El conjunto de todos esos vectores está alineado, formando una **recta que pasa por el origen**.
****
 - Ahora supongamos con la notación del punto anterior, si $S$ contiene algún elemento que no es de la forma $\lambda \cdot v$, digamos $v'$, contiene también a todos los múltiplos de $v'$. Luego, $S$ contiene a las dos rectas $L$ y $L'$ que pasan por el origen y cuyas direcciones son $v$ y $v'$ respectivamente. Es claro (usando la regla del paralelogramo) que cualquier punto en $\mathbb{R}^2$ es suma de un elemento de $L$ más uno de $L'$, luego pertenece a $S$.  En consecuencia, $S = \mathbb{R}^2$. 
 Supón que el subespacio $S \subseteq \mathbb{R}^2$ contiene:
1. Un vector no nulo $v$, entonces ya sabemos que contiene **la recta** generada por $v$: todos los vectores $\lambda v$.
2. Ahora, si además contiene otro vector $v'$ que **no** es múltiplo de $v$, entonces:
    - $S$ debe contener también todos los múltiplos de $v'$, es decir, otra recta distinta pasando por el origen.
    - Como $v$ y $v'$ **no son colineales**, las direcciones de $v$ y $v'$ **generan un plano completo**.
La frase “**usando la regla del paralelogramo**” es una forma gráfica de decir que **sumar vectores en distintas direcciones genera todo el plano**.
###### **¿Qué significa que generen el plano completo?**
El conjunto de todas las combinaciones lineales de $v$ y $v'$:
$${λv+μv′∣λ,μ∈R}$$
es todo $\mathbb{R}^2$. Esto se debe a que $v$ y $v'$ son **linealmente independientes**, y por tanto **forman una base de** $\mathbb{R}^2$.