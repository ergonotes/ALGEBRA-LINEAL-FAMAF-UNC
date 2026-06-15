**Proposición.** Sea $V$ espacio vectorial de dimensión finita y sean $V_1, V_2$ dos subespacios de $V$ tal que $V = V_1 \oplus V_2$. Sea $\mathcal{B}_1$ base de $V_1$ y $\mathcal{B}_2$ base de $V_2$, entonces $\mathcal{B} = \mathcal{B}_1 \cup \mathcal{B}_2$ es base de $V$.
****
**Demostración**. Sea $\mathcal{B}_1 = \{u_1, \dots, u_r\}$ y $\mathcal{B}_2 = \{u_{r+1}, \dots, u_{r+s}\}$, debemos ver entonces que el conjunto $\mathcal{B} = \{u_1, \dots, u_{r+s}\}$ genera todo el espacio y es LI.

Sea $v \in V$, como $V_1 + V_2 = V$, existen $v_1 \in V_1$ y $v_2 \in V_2$ tales que $v = v_1 + v_2$. Como $\mathcal{B}_1$ es base de $V_1$, tenemos que $v_1 = a_1u_1 + \cdots + a_ru_r$, análogamente $v_2 = a_{r+1}u_{r+1} + \cdots + a_{r+s}u_{r+s}$ y por lo tanto $v = a_1u_1 + \cdots + a_{r+s}u_{r+s}$. Es decir $\mathcal{B}$ genera $V$.

Si $a_1u_1 + \cdots + a_ru_r + a_{r+1}u_{r+1} + \cdots + a_{r+s}u_{r+s} = 0$, entonces 
$$
a_1u_1 + \cdots + a_ru_r = -a_{r+1}u_{r+1} - \cdots - a_{r+s}u_{r+s}.
$$
Ahora bien, el término de la izquierda en la última igualdad pertenece a $V_1$, mientras que el de a derecha pertenece a $V_2$. Como $V_1 \cap V_2 = 0$, tenemos que  
$$
a_1u_1 + \cdots + a_ru_r = 0 = -a_{r+1}u_{r+1} - \cdots - a_{r+s}u_{r+s}.
$$
Como $\mathcal{B}_1$ es base de $V_1$, $a_1 = \cdots = a_r = 0$ y como $\mathcal{B}_2$ es base de $V_2$, $a_{r+1} = \cdots = a_{r+s} = 0$. Es decir $\mathcal{B}$ es LI. $\square$
