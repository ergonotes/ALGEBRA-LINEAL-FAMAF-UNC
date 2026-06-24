**Proposición**. Sea $T: V \to W$ transformación lineal. Entonces,
(1) $T$ es monomorfismo si y sólo si $T$ de un conjunto LI es LI.
(2) $T$ es epimorfismo si y sólo si $T$ de un conjunto de generadores de $V$ es un conjunto de generadores de $W$.
****
**Demostración**.
(1) ($\Rightarrow$) Sea $\{v_1, \dots, v_n\}$ un conjunto LI en $V$ y sean $\lambda_1, \dots, \lambda_n \in \mathbb{K}$ tales que
$$
\lambda_1 T(v_1) + \cdots + \lambda_n T(v_n) = 0,
$$
entonces
$$
0 = T(\lambda_1 v_1 + \cdots + \lambda_n v_n).
$$
Como $T$ es inyectiva, y, como vimos en el inciso, **[[D-Una transformación lineal es un monomorfismo si y solo si su núcleo es el subespacio trivial]]**:
$$
\lambda_1 v_1 + \cdots + \lambda_n v_n = 0,
$$
lo cual implica que $\lambda_1, \dots, \lambda_n$ son todos nulos. Por lo tanto, $T(v_1), \dots, T(v_n)$ son LI.

(1) ($\Leftarrow$) Sea $v \in V$ tal que $T(v) = 0$. Veremos que eso implica que $v = 0$. Ahora bien, sea $\{v_1, \dots, v_n\}$ una base de $V$, entonces existen $\lambda_1, \dots, \lambda_n \in \mathbb{K}$ tales que
$$
v = \lambda_1 v_1 + \cdots + \lambda_n v_n,
$$
por lo tanto
$$
0 = T(v) = T(\lambda_1 v_1 + \cdots + \lambda_n v_n) = \lambda_1 T(v_1) + \cdots + \lambda_n T(v_n).
$$
Como $\{v_1, \dots, v_n\}$ es LI, por hipótesis, $\{T(v_1), \dots, T(v_n)\}$ es LI y, por lo tanto, $\lambda_1, \dots, \lambda_n$ son todos nulos. Luego $v = 0$. Es decir probamos que el núcleo de $T$ es 0, luego por proposición anterior ([[D-Una transformación lineal es un monomorfismo si y solo si su núcleo es el subespacio trivial]]), $T$ es monomorfismo.

(1) ($\Leftarrow$/alternativa) Sea $v \in V$ tal que $T(v) = 0$. Si $v \neq 0$, entonces $\{v\}$ es un conjunto LI en $V$. Luego, $\{T(v)\}$ es un conjunto LI en $W$ y por lo tanto $T(v) \neq 0$. Así, si $T(v) = 0$ entonces $v = 0$ y por tanto $T$ es un monomorfismo.

(2) ($\Rightarrow$) Sea $\{v_1, \dots, v_n\}$ un conjunto de generadores de $V$ y sea $w \in W$. Como $T$ es epimorfismo, existe $v \in V$ tal que $T(v) = w$. Ahora bien,
$$
v = \lambda_1 v_1 + \cdots + \lambda_n v_n, \quad \text{para algún } \lambda_1, \dots, \lambda_n \in \mathbb{K},
$$
por lo tanto,
$$
w = T(v) = T(\lambda_1 v_1 + \cdots + \lambda_n v_n) = \lambda_1 T(v_1) + \cdots + \lambda_n T(v_n).
$$
Es decir, cualquier $w \in W$ se puede escribir como combinación lineal de los $T(v_1), \dots, T(v_n)$ y, por lo tanto, generan $W$.
(2) ($\Leftarrow$) Sea $\{v_1, \dots, v_n\}$ una base de $V$, por hipótesis $T(v_1), \dots, T(v_n)$ generan $W$, es decir dado cualquier $w \in W$, existen $\lambda_1, \dots, \lambda_n \in \mathbb{K}$ tales que
$$
w = \lambda_1 T(v_1) + \cdots + \lambda_n T(v_n),
$$
y por lo tanto $w = T(v)$, con
$$
v = \lambda_1 v_1 + \cdots + \lambda_n v_n.
$$
$\square$