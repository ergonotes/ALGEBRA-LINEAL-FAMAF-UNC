**Proposición**. Sean $S$ y $T$ subespacios de un espacio vectorial $V$. Entonces se cumple que...
1. $S+T$ es un subespacio vectorial de $V$.

2. $S+T=⟨S∪T⟩$ _(Es decir, la suma es exactamente igual al subespacio generado por la unión de $S$ y $T$, lo que lo convierte por definición en el menor subespacio que contiene a ambos)._

3. Si $S=⟨X⟩$ y $T=⟨W⟩$, entonces $S+T=⟨X∪W⟩$.
****
**Demostración**. 
($1$). **El vector nulo está en $S+T$.**
Como $S$ y $T$ son subespacios, ambos contienen obligatoriamente al vector nulo $0$.
Si sumamos el cero de $S$ con el cero de $T$, obtenemos $0 + 0 = 0$.
Como $0$ se puede escribir como una suma de un elemento de $S$ y uno de $T$, entonces **$0 \in S+T$**.
**Cerradura bajo la suma.** 
Tomemos dos vectores cualquiera que pertenezcan a $S+T$, digamos $u$ y $v$. Por definición, existen $s_1, s_2 \in S$ y $t_1, t_2 \in T$ tales que: $$u = s_1 + t_1$$ $$v = s_2 + t_2$$Si los sumamos: $$u + v = (s_1 + t_1) + (s_2 + t_2)$$Como la suma es conmutativa, reordenamos: $$u + v = (s_1 + s_2) + (t_1 + t_2)$$Como $S$ es subespacio, $(s_1 + s_2) \in S$. Como $T$ es subespacio, $(t_1 + t_2) \in T$. Por lo tanto, la suma total pertenece a $S+T$ (volver a ver definición de suma de subespacios por si hay dudas).
**Cerradura bajo producto por escalar.**
Tomemos un vector $u = s + t \in S+T$ y un escalar $\alpha$ del cuerpo $K$.
$$\alpha u = \alpha (s + t) = \alpha s + \alpha t$$Como $S$ y $T$ son subespacios, $\alpha s \in S$ y $\alpha t \in T$. Por lo tanto, la combinación sigue perteneciendo a $S+T$. 
$S+T$ cumple las tres reglas, por lo tanto, es un subespacio vectorial de $V$.
****
($2$). Para demostrar que dos conjuntos son iguales, hay que demostrar que uno está contenido en el otro, y viceversa ($\subseteq$ y $\supseteq$).

Veamos $S+T \subseteq \langle S \cup T \rangle$:
Toma cualquier vector $v \in S+T$. Sabemos que $v = s + t$. Como $s$ pertenece a $S$, lógicamente pertenece a la unión $S \cup T$. Lo mismo pasa con $t$.
Por lo tanto, $v = s + t$ es una combinación lineal de elementos que están en $S \cup T$. Por definición de generador, esto significa que $v \in \langle S \cup T \rangle$.

Veamos $\langle S \cup T \rangle \subseteq S+T$:
Por definición, $\langle S \cup T \rangle$ es _el subespacio más pequeño_ que contiene tanto a $S$ como a $T$.
¿Contiene $S+T$ a $S$? Sí, porque cualquier vector $s \in S$ se puede escribir como $s + 0$ (donde $0 \in T$).
¿Contiene $S+T$ a $T$? Sí, por la misma razón ($0 + t$).
Como ya demostramos en ($1$) que $S+T$ es un subespacio, y acabamos de ver que contiene a $S \cup T$, entonces obligatoriamente debe contener al subespacio generado $\langle S \cup T \rangle$.

Al contenerse mutuamente, son exactamente el mismo conjunto.
****
($3$). Esta demostración usa la misma lógica de "doble contención" de la parte anterior.
Veamos $S+T \subseteq \langle X \cup W \rangle$:
Toma un vector $v \in S+T$, donde $v = s + t$.   
Como $s$ es generado por $X$, podemos escribirlo como una combinación lineal: $$s = a_1x_1 + \dots + a_nx_n$$ 
Como $t$ es generado por $W$, podemos escribirlo como: $t = b_1w_1 + \dots + b_mw_m$.
Si sumamos ambos:
$$v = (a_1x_1 + \dots + a_nx_n) + (b_1w_1 + \dots + b_mw_m)$$
Esta ecuación nos grita en la cara que $v$ está formado por una gran combinación lineal usando únicamente elementos de $X$ y elementos de $W$. Por lo tanto, $v \in \langle X \cup W \rangle$.

Demostrar que $\langle X \cup W \rangle \subseteq S+T$:
Toma cualquier vector $v$ generado por $X \cup W$.
Por definición, $v$ es una combinación lineal de varios vectores, algunos provenientes de $X$ y otros provenientes de $W$.
Si agrupamos todos los términos que usan vectores de $X$ por un lado, y todos los que usan vectores de $W$ por otro, nos queda: $$v = (\text{combinación de elementos de } X) + (\text{combinación de elementos de } W)$$
El primer paréntesis es, por definición, un elemento de $S$. El segundo paréntesis es un elemento de $T$. Por lo tanto, $v = s + t$, lo que significa que $v \in S+T$.

Nuevamente, al contenerse mutuamente, la igualdad queda demostrada.