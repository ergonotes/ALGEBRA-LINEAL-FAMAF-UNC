**Teorema**. Sean $V, W$ espacios vectoriales de dimensión finita sobre $\mathbb{K}$ tal que $\dim V = \dim W$. Sea $T: V \to W$ transformación lineal. Entonces, son equivalentes:

(a) $T$ es un isomorfismo.
(b) $T$ es monomorfismo.
(c) $T$ es epimorfismo.
(d) Si $\{v_1, \dots, v_n\}$ es una base de $V$, entonces $\{T(v_1), \dots, T(v_n)\}$ es una base de $W$.
****
**Demostración**. Sea $n = \dim V = \dim W$.
(a) $\Rightarrow$ (b). Como $T$ es isomorfismo, es biyectiva y por lo tanto inyectiva.

(b) $\Rightarrow$ (c). $T$ monomorfismo, entonces $\text{nulidad}(T) = 0$ ([[D-Una transformación lineal es un monomorfismo si y solo si su núcleo es el subespacio trivial]]). 
Luego, como $\text{rango}(T) + \text{nulidad}(T) = \dim V$, tenemos que $\text{rango}(T) = \dim V$. Como $\dim V = \dim W$, tenemos que $\dim \text{Im}(T) = \dim W$ y por lo tanto $\text{Im}(T) = W$. En consecuencia, $T$ es suryectiva.

(c) $\Rightarrow$ (a). $T$ es suryectiva, entonces $\text{rango}(T) = n$, luego $\text{nulidad}(T) = 0$, por lo tanto $\text{Nu}(T) = 0$ y en consecuencia $T$ es inyectiva. Como $T$ es suryectiva e inyectiva es un isomorfismo.

Hasta aquí probamos que (a), (b) y (c) son equivalentes, luego si probamos que (a), (b) o (c) $\Rightarrow$ (d) y que (d) $\Rightarrow$ (a), (b) o (c), estaría probado el teorema.

(a) $\Rightarrow$ (d). Sea $\{v_1, \dots, v_n\}$ una base de $V$, entonces $\{v_1, \dots, v_n\}$ es LI y genera $V$. Por proposición anterior ([[D-Monomorfismo conserva LI, Epimorfismo conserva generadores]]), tenemos que $\{T(v_1), \dots, T(v_n)\}$ es LI y genera $W$, por lo tanto $\{T(v_1), \dots, T(v_n)\}$ es una base de $W$.

(d) $\Rightarrow$ (a). Como $T$ de una base es una base, entonces $T$ de un conjunto LI es un conjunto LI y $T$ de un conjunto de generadores de $V$ es un conjunto de generadores de $W$. Por lo tanto, por proposición anterior ([[D-Monomorfismo conserva LI, Epimorfismo conserva generadores]]), $T$ es monomorfismo y epimorfismo, luego $T$ es un isomorfismo. $\square$