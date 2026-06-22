**Teorema**. Sean $V, W$ espacios vectoriales sobre un cuerpo $\mathbb{K}$ y sea $T : V \to W$ una transformación lineal. Supóngase que $V$ es de dimensión finita. Entonces
$$
\text{rango}(T) + \text{nulidad}(T) = \dim V.
$$
****
**Demostración.** Sean
$$
\begin{aligned}
n &= \dim V \\
k &= \dim(\text{Nu } T) = \text{nulidad}(T).
\end{aligned}
$$
Entonces debemos probar que
$$
n - k = \dim(\text{Im } T) = \text{rango}(T).
$$
Sea $\{v_1, \dots, v_k\}$ una base de $\text{Nu } T$. Existen vectores $\{v_{k+1}, \dots, v_n\}$ en $V$ tales que $\{v_1, \dots, v_n\}$ es una base de $V$. Para probar el teorema, demostraremos que $\{Tv_{k+1}, \dots, Tv_n\}$ es una base para la imagen de $T$.

(1) $\{Tv_{k+1}, \dots, Tv_n\}$ genera la imagen de $T$.
Si $w \in \text{Im}(T)$, entonces existe $v \in V$ tal que $T(v) = w$, como $\{v_1, \dots, v_n\}$ es base de $V$, existen $\lambda_1, \dots, \lambda_n \in \mathbb{K}$, tal que $v = \lambda_1 v_1 + \cdots + \lambda_n v_n$, por lo tanto
$$
\begin{aligned}
w &= T(v) \\
&= \lambda_1 T(v_1) + \cdots + \lambda_k T(v_k) + \lambda_{k+1} T(v_{k+1}) + \cdots + \lambda_n T(v_n) \\
&= 0 + \cdots + 0 + \lambda_{k+1} T(v_{k+1}) + \cdots + \lambda_n T(v_n) \\
&= \lambda_{k+1} T(v_{k+1}) + \cdots + \lambda_n T(v_n).
\end{aligned}
$$
Por lo tanto, $\{Tv_{k+1}, \dots, Tv_n\}$ genera la imagen de $T$.

(2) $\{Tv_{k+1}, \dots, Tv_n\}$ es un conjunto linealmente independiente.
Para ver que $\{Tv_{k+1}, \dots, Tv_n\}$ es linealmente independiente, supóngase que se tienen escalares $\mu_i$ tales que
$$
\sum_{i=k+1}^n \mu_i Tv_i = 0,
$$
luego
$$
0 = \sum_{i=k+1}^n \mu_i Tv_i = T\left( \sum_{i=k+1}^n \mu_i v_i \right).
$$
Por lo tanto $v = \sum_{i=k+1}^n \mu_i v_i \in \text{Nu}(T)$. Como $\{v_1, \dots, v_k\}$ es una base de $\text{Nu } T$, existen escalares $\lambda_i$ tales que 
$$
v = \sum_{i=1}^k \lambda_i v_i,
$$
es decir
$$
\sum_{j=k+1}^n \mu_j v_j = \sum_{i=1}^k \lambda_i v_i.
$$
Luego
$$
\begin{aligned}
0 &= \sum_{i=1}^k \lambda_i v_i - \left( \sum_{j=k+1}^n \mu_j v_j \right) \\
&= \lambda_1 v_1 + \cdots + \lambda_k v_k - \mu_{k+1} v_{k+1} - \cdots - \mu_n v_n.
\end{aligned}
$$
Como $\{v_1, \dots, v_n\}$ es una base, y por lo tanto un conjunto LI, tenemos que $0 = \lambda_1 = \cdots = \lambda_k = \mu_{k+1} = \cdots = \mu_n$, y en particular $0 = \mu_{k+1} = \cdots = \mu_n$. Por lo tanto $\{Tv_{k+1}, \dots, Tv_n\}$ es un conjunto linealmente independiente. $\square$
