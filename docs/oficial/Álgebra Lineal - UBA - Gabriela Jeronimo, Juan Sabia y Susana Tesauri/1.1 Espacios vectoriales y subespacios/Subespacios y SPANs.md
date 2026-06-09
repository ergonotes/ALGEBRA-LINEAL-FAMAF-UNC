## **Teorema**. Sea $V$ un $K$-espacio vectorial y sean $v_1, \ldots, v_n \in V$. 
Entonces el conjunto de combinaciones lineales de $v_1, \ldots, v_n$,
$$ W = \{\lambda_1 v_1 + \ldots + \lambda_n v_n : \lambda_1, \ldots, \lambda_n \in K\} $$
es un subespacio vectorial de $V$.

**Demostración**. Sean $v, w \in W$. Entonces
$$v = \lambda_1 v_1 + \ldots + \lambda_n v_n, \quad w = \mu_1 v_1 + \ldots + \mu_n v_n.$$
Si $c \in K$, entonces
$$cv + w = (c\lambda_1 + \mu_1)v_1 + \ldots + (c\lambda_n + \mu_n)v_n.$$
Por lo tanto,
$$cv + w \in W. \quad \square$$
****
Si un ejercicio pide: _"Demuestra que el conjunto $W$ es un subespacio"_, y logramos reescribir la fórmula de $W$ para que se vea como una suma de vectores multiplicados por parámetros $λ$, podríamos decir: **"Por el Teorema de las Combinaciones Lineales, esto es un subespacio".** Ahorrándonos tener que probar la suma, la multiplicación y el vector nulo a mano.
****
#### **Definición**. Sea $S$ un conjunto de vectores de un espacio vectorial $V$. 
El **espacio** **generado**, o **SPAN**, por $S$ es el conjunto de todas las combinaciones lineales de elementos de $S$, y se denota por$$ \langle S \rangle = \left\{ \sum_{i=1}^{n} a_i v_i : v_i \in S, a_i \in K, n \in \mathbb{N} \right\}. $$Si $S = \{v_1, \ldots, v_n\}$,
entonces
$$ \langle S \rangle = \{a_1 v_1 + \ldots + a_n v_n : a_i \in K\}. $$
[[E-SPANs]]
****
### **Teorema**. Sea $V$ un espacio vectorial sobre $K$ y $S = \{v_1, \ldots, v_n\} \subset V$. 
Entonces la intersección de todos los subespacios que contienen a $S$ es igual al espacio generado por $S$:
$$ \langle v_1, \ldots, v_n \rangle = \langle S \rangle = \bigcap_{\substack{S \subseteq W \\ W \text{ subespacio}}} W. $$
[[D-La intersección de todos los subespacios que contienen a S es igual al espacio generado por S]]
****
### **Proposición**. Sea $V$ un espacio vectorial sobre un cuerpo $K$, y sea $S$ un subconjunto no vacío de $V$. 
$\langle S \rangle$ es subespacio vectorial de $V$.
**[[D-El SPAN de un subconjunto no vacío en V es subespacio vectorial de V]]**
****
#### **Definición**. Decimos que $S$ es un conjunto de generadores de $V$ si $\langle S \rangle = V$.

#### **Observación**. El conjunto de generadores de un espacio vectorial no es único: puede ocurrir que $S_1 \neq S_2$ y sin embargo $\langle S_1 \rangle = \langle S_2 \rangle$.
Por ejemplo, en $\mathbb{R}^3$, sea $S = \{(1, 0, 0), (0, 1, 0), (-1, 2, 0)\}$. Entonces
$$ \langle S \rangle = \{(a_1 - a_3, a_2 + 2a_3, 0) : a_1, a_2, a_3 \in K\} = \{(x, y, z) \in \mathbb{R}^3 : z = 0\}. $$
También puede ser generado por $S' = \{(1, 0, 0), (0, 1, 0)\}$
o por $S_2 = \{(1, 1, 0), (1, -1, 0)\}$.
****
#### **Definición**. Si $S_1, S_2, \ldots, S_k$ son subconjuntos de un espacio vectorial $V$, el conjunto de todas las sumas $\alpha_1 + \alpha_2 + \ldots + \alpha_k$ de vectores $\alpha_i$ de $S_i$ se llama suma de los subconjuntos $S_1, S_2, \ldots, S_k$ y se representa por
$$ S_1 + S_2 + \ldots + S_k $$
Si $W_1, W_2, \ldots, W_k$ son subespacios de $V$, entonces la suma
$$ W = W_1 + W_2 + \ldots + W_k $$
como es fácil ver, es un subespacio de $V$ que contiene cada uno de los subespacios $W_i$.
****
#### **Proposición**. Sea $V$ un espacio vectorial sobre $K$ y sean $v_1, \ldots, v_r$ elementos de de $V$. Entonces
$$ \langle v_1, \ldots, v_r \rangle = \langle v_1 \rangle + \ldots + \langle v_r \rangle. $$
**Demostración**. Probemos el resultado viendo que los dos conjuntos se incluyen mutuamente.
($\subseteq$) Sea $w \in \langle v_1, \ldots, v_r \rangle$, luego $w = \lambda_1 v_1 + \ldots + \lambda_r v_r$. Como $\lambda_i v_i \in \langle v_i \rangle$, $1 \leq i \leq r$, tenemos que $w \in \langle v_1 \rangle + \ldots + \langle v_r \rangle$. En consecuencia, $\langle v_1, \ldots, v_r \rangle \subseteq \langle v_1 \rangle + \ldots + \langle v_r \rangle$.
($\supseteq$) Si $w \in \langle v_1 \rangle + \ldots + \langle v_r \rangle$, entonces $w = w_1 + \ldots + w_r$ con $w_i \in \langle v_i \rangle$ para todo $i$. Por lo tanto, $w_i = \lambda_i v_i$ para algún $\lambda_i \in K$ y $w = \lambda_1 v_1 + \ldots + \lambda_r v_r \in \langle v_1, \ldots, v_r \rangle$. En consecuencia, $\langle v_1 \rangle + \ldots + \langle v_r \rangle \subseteq \langle v_1, \ldots, v_r \rangle$. $\square$

