**Proposición.** Sea $V$ un espacio vectorial de dimensión finita. Sea $S = \{v_1, \dots, v_m\}$ un conjunto de generadores de $V$. Entonces existe un subconjunto $\mathcal{B} \subseteq S$ que es una base de $V$.
****
**Demostración.** Vamos a definir inductivamente subconjuntos $G_j \subseteq S$, $j = 1, \dots, m$, que sean L.I.
$j = 1: G_1 = \{v_1\}$ si $v_1 \neq 0$ (luego $G_1$ es L.I.); o $G_1 = \emptyset$ si $v_1 = 0$.
$j = 2$:
$$
G_2 = \begin{cases} G_1 \cup \{v_2\} & \text{si } v_2 \notin \langle G_1 \rangle, \\ G_1 & \text{si } v_2 \in \langle G_1 \rangle. \end{cases}
$$

Observemos que $G_2$ es L.I.: si $v_2 \notin \langle G_1 \rangle$, entonces $G_1 \cup \{v_2\}$ es L.I. (prop. ant.); si $v_2 \in \langle G_1 \rangle$, entonces $G_2 = G_1$ que es L.I. Además $\langle G_2 \rangle = \langle v_1, v_2 \rangle$ en ambos casos.
$j = 3$: Hacemos lo mismo, $G_3 = G_2$ o $G_2 \cup \{v_3\}$ (en ambos casos es L.I.).
En general, ya tenemos definido $G_j \subseteq S$ L.I. y tal que $\langle G_j \rangle = \langle \{v_1, \dots, v_j\} \rangle$. Definimos:

$$
G_{j+1} = \begin{cases} G_j \cup \{v_{j+1}\} & \text{si } v_{j+1} \notin \langle G_j \rangle, \\ G_j & \text{si } v_{j+1} \in \langle G_j \rangle. \end{cases}
$$

En ambos casos $G_{j+1}$ es L.I. y $\langle G_{j+1} \rangle = \langle G_j \cup \{v_{j+1}\} \rangle = \langle \{v_1, \dots, v_{j+1}\} \rangle$.
Y así sigo. En el último paso, definimos $G_m$, que es L.I. y tal que

$$
\langle G_m \rangle = \langle \{v_1, \dots, v_m\} \rangle = V \quad (\text{pues } S = \{v_1, \dots, v_m\} \text{ genera } V).
$$

Por lo tanto $G_m$ así construído es L.I. y genera $V$, luego es base de $V$. $\square$