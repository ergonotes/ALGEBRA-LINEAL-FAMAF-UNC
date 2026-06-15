**Teorema**. Si $W_1$ y $W_2$ son subespacios de dimensión finita de un espacio vectorial, entonces $W_1 + W_2$ es de dimensión finita y
$$
\dim W_1 + \dim W_2 = \dim(W_1 \cap W_2) + \dim(W_1 + W_2).
$$
****
**Demostración.** El conjunto $W_1 \cap W_2$ es un subespacio de $W_1$ y $W_2$ y por lo tanto un espacio vectorial de dimensión finita. Sea $u_1, \dots, u_k$ una base de $W_1 \cap W_2$, y ya que **[[D-Todo conjunto linealmente independiente se puede extender hasta formar una base]]**, existen $v_1, \dots, v_n$ vectores en $W_1$ y $w_1, \dots, w_m$ vectores en $W_2$ tal que
$$
\{u_1, \dots, u_k, v_1, \dots, v_n\} \quad \text{es una base de } W_1,
$$
 y
$$
\{u_1, \dots, u_k, w_1, \dots, w_m\} \quad \text{es una base de } W_2.
$$
 (los vectores base $u$ de la intersección son justamente una **base**, mientras que los demás $w$ y $v$ son simplemente vectores exclusivos de $W_2$ y $W_1$ respectivamente)
Es claro que, el subespacio $W_1 + W_2$ es generado por los vectores
$$
u_1, \dots, u_k, v_1, \dots, v_n, w_1, \dots, w_m.
$$
Veamos que estos vectores forman un conjunto independiente. En efecto, supóngase que
$$
\sum \lambda_i u_i + \sum \gamma_i v_i + \sum \mu_i w_i = 0,
$$
luego
$$
\sum \mu_i w_i = -\sum \lambda_i u_i - \sum \gamma_i v_i.
$$
vemos que el lado izquierdo tiene solo vectores $w$, esto significa que el resultado es un vector que vive en $W_2$, mientras que el lado derecho tiene vectores $u$ y $v$, esto quiere decir que el resultado es un vector que vive en $W_1$.
Si un vector vive en $W_2$​ y al mismo tiempo es igual a un vector que vive en $W_1$​, **significa que ese vector vive en la intersección ($W_1​∩W_2$​).** 
Ahora recordemos que al principio dijimos que la intersección _solo_ se fabrica usando vectores base $u$, que son **L.I**, por lo tanto, la única forma de que el lado izquierdo (hecho de $w$) sea parte de la intersección, es que esa suma de vectores $w$ en realidad valga cero. Esto demuestra que **todos los coeficientes $μ$ valen $0$**.
Como descubrimos que todos los μ=0, la parte de las w desaparece por completo de nuestra ecuación original
$$
\sum \lambda_i u_i + \sum \gamma_i v_i  = 0,
$$
y ahora vemos que los $u$ y los $v$ son exactamente la base que definimos de $W_1$, y como también es **L.I**, los coeficientes $λ$ y $γ$ valen $0$.
Ya que demostramos que el conjunto gigante es una base **L.I** para la suma, veamos cuál es la dimensión de $W_1+W_2$ :
Supongamos hay $k$ vectores (de la intersección), $n$ vectores (exclusivos de $W_1$​) y luego $m$ vectores (exclusivos de $W_2$​)  $$\implies \ \ \ \text{Dimensión Total }=k+n+m$$ y si revisamos la fórmula original del teorema: 
$$
\dim W_1 + \dim W_2 = (k + n) + (k + m) = 2k + n + m
$$
$$
\dim(W_1 \cap W_2) + \dim(W_1 + W_2) = k + (k + n + m) = 2k + n + m
$$
