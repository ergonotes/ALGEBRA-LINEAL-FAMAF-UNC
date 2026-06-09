Geométricamente, decir que un conjunto de vectores es **linealmente dependiente** significa que **al menos uno de esos vectores no aporta una dirección nueva**; está atrapado en la "sombra" (el subespacio) que ya trazaron los demás.
****
#### **DEFINICIÓN**. Sea $V$ un espacio vectorial sobre $\mathbb{K}$. Un subconjunto $S$ de $V$ se dice *linealmente dependiente* (o simplemente, *dependiente*)... 
 si existen vectores distintos $v_1, \dots, v_n \in S$ y escalares $\lambda_1, \dots, \lambda_n$ de $\mathbb{K}$, no todos nulos, tales que
$$
\lambda_1 v_1 + \dots + \lambda_n v_n = 0.
$$
Un conjunto que no es linealmente dependiente se dice **linealmente independiente**.

Si el conjunto $S$ tiene solo un número finito de vectores $v_1, \dots, v_n$ se dice, a veces, que los $v_1, \dots, v_n$ son dependientes (o independientes), en vez de decir que $S$ es dependiente (o independiente).
[[E-LI y LD]]
****
#### **Observaciones a partir de la definición**
1. **Todo conjunto que contiene un conjunto linealmente dependiente es linealmente dependiente.**
	1. *Si ya existen vectores tales que $0$ es combinación lineal no trivial de los vectores en un conjunto, no importa cuantos vectores más haya en el conjunto, ya puedo expresar al $0$ como combinación lineal no trivial de los vectores mencionados*
2. **Todo subconjunto de un conjunto linealmente independiente es linealmente independiente.**
3. **Todo** **conjunto** **que contiene el vector $0$ es linealmente dependiente; en efecto, $1 \cdot 0 = 0$.**
	1. *Con el vector nulo ya puedo expresar al $0$ como combinación lineal*
****
### **Definición.** Sea $V$ un espacio vectorial. Una **base** de $V$ es... 
un conjunto de vectores linealmente independiente de $V$ que genera el espacio $V$. 

El espacio $V$ es de **dimensión finita** si tiene una base finita.
##### **Base Canónica**
Sea el espacio vectorial $\mathbb{K}^n$ y sean
$$
\begin{aligned}
e_1 &= (1, 0, 0, \dots, 0) \\
e_2 &= (0, 1, 0, \dots, 0) \\
&\quad \dots \dots \\
e_n &= (0, 0, 0, \dots, 1)
\end{aligned}
$$Entonces veamos que $e_1, \dots, e_n$ es una base de $\mathbb{K}^n$.
Vemos primero si $e_1, \dots, e_n$ genera $\mathbb{K}^n$...
Si $(x_1, \dots, x_n) \in \mathbb{K}^n$, entonces
$$
(x_1, \dots, x_n) = x_1 e_1 + \dots + x_n e_n.
$$
Por lo tanto, $e_1, \dots, e_n$ genera a $\mathbb{K}^n$.
Veamos ahora si $e_1, \dots, e_n$ es L.I, para verificar la definición, Si
$$
x_1 e_1 + \dots + x_n e_n = 0,
$$
entonces
$$
\begin{aligned}
(0, \dots, 0) &= x_1(1, 0, \dots, 0) + x_2(0, 1, \dots, 0) + \dots + x_n(0, 0, \dots, 1) \\
&= (x_1, 0, \dots, 0) + (0, x_2, \dots, 0) + \dots + (0, 0, \dots, x_n) \\
&= (x_1, x_2, \dots, x_n).
\end{aligned}
$$
Luego, $x_1 = x_2 = \dots = x_n = 0$ y por lo tanto $e_1, \dots, e_n$ es LI.

Para $1 \le i \le n$, al vector $e_i$ se lo denomina el $i$-ésimo **vector** **canónico** y a la base $\mathcal{B}_n = \{e_1, \dots, e_n\}$ se la denomina la **base** **canónica** de $\mathbb{K}^n$.
****
### **Teorema.** Sea $V$ un espacio vectorial generado por un conjunto finito de vectores $\beta_1, \beta_2, \dots, \beta_m$. 
Entonces todo conjunto independiente de vectores de $V$ es finito y no contiene más de $m$ elementos.

En términos sencillos, ***"Si nos basta con $m$ vectores para generar todo el espacio, entonces es imposible encontrar dentro de ese espacio más de $m$ vectores que sean independientes entre sí."***
**[[D-Un espacio construido con x vectores no puede contener más de x direcciones independientes]]**
****
### **Corolario.** Si $V$ es un espacio vectorial de dimensión finita, entonces dos bases cualesquiera de $V$ tienen el mismo número (finito) de elementos.
***Demostración**.* Como $V$ es de dimensión finita, tiene una base finita $\{\beta_1, \beta_2, \dots, \beta_m\}$.
Por el Teorema anterior, toda base de $V$ es finita y contiene no más de $m$ elementos. Así, si $\{\alpha_1, \alpha_2, \dots, \alpha_n\}$ es una base, $n \le m$. 
Por el mismo razonamiento, pensemos $\{\alpha_1, \alpha_2, \dots, \alpha_n\}$ como la base que ya existe previamente en $V$, y veamos que se tiene que cumplir $m \le n$ con $\{\beta_1, \beta_2, \dots, \beta_m\}$. Luego $m = n$ y ambas tienen el mismo número de elementos. $\blacksquare$