**Corolario**. Sea $W$ un subespacio de un espacio vectorial $V$ con dimensión finita $n$ y $S_0$ un subconjunto LI de $W$. Entonces, $S_0$ se puede completar a una base de $W$.
****
**Demostración.** Sea $S_0 \subseteq W$ L.I. Como $S_0$ es un conjunto L.I. en $V$, y $\dim V = n$, se tiene $|S_0| \le n$.
Se extiende $S_0$ a una base de $W$ como sigue:

* Si $S_0$ genera $W$, tenemos que es una base de $W$ (pues $S$ es L.I. y genera $W$).
* Si $S_0$ no genera $W$, existe $y \in W$ tal que $y \notin \langle S_0 \rangle$ entonces el conjunto $S_1 = S_0 \cup \{y\}$ es L.I. (lema anterior ([[D-Añadir un vector externo al generador de un conjunto L.I. preserva su independencia lineal]])).

Si $S_1$ genera $W$, ya está; sino, $\exists w_2 \in W$ tal que $S_1 \cup \{w_2\}$ es L.I.
Continuando de este modo, en una cantidad finita de pasos obtendremos que $S_m = S_0 \cup \{w_1, \dots, w_m\}$ es L.I. y genera $W$.