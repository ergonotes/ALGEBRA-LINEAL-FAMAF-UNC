**Teorema**. Sea $V$ espacio vectorial y sea $T : V \to V$ una aplicación lineal. Sean $v_1, \dots, v_m$ autovectores de $T$, con autovalores $\lambda_1, \dots, \lambda_m$ respectivamente. Suponga que estos autovalores son distintos entre sí, esto es, $\lambda_i \neq \lambda_j$ si $i \neq j$. Entonces $v_1, \dots, v_m$ son linealmente independientes.
****
**Demostración**. Hagamos la demostración por inducción sobre $m$.
Caso base. Si $m = 1$, no hay nada que demostrar puesto que un vector no nulo es LI.

Paso inductivo. Supongamos que el enunciado es verdadero para el caso $m - 1$ con $m > 1$, (hipótesis inductiva o HI), y probemos entonces que esto implica que es cierto para $m$. Debemos ver que si

$$
(*) \ \ \ \quad c_1v_1 + c_2v_2 + \cdots + c_mv_m = 0
$$
entonces $c_1 = \dots = c_m = 0$. Multipliquemos ($*$) por $\lambda_1$, obtenemos:

$$
(**) \ \ \ \quad c_1\lambda_1v_1 + c_2\lambda_1v_2 + \cdots + c_m\lambda_1v_m = 0.
$$
También apliquemos $T$ a ($*$) y obtenemos

$$
(***) \ \ \ \quad c_1\lambda_1v_1 + c_2\lambda_2v_2 + \cdots + c_m\lambda_mv_m = 0.
$$
Ahora a ($**$) le restamos ($***$) y obtenemos:

$$
c_2(\lambda_1 - \lambda_2)v_2 + \cdots + c_m(\lambda_1 - \lambda_m)v_m = 0.
$$
Como, por hipótesis inductiva, $v_2, \dots, v_m$ son LI, tenemos que $c_i(\lambda_1 - \lambda_i) = 0$ para $i \ge 2$. Como $\lambda_1 - \lambda_i \neq 0$ para $i \ge 2$, obtenemos que $c_i = 0$ para $i \ge 2$. Por (*) eso implica que $c_1 = 0$ y por lo tanto $c_i = 0$ para todo $i$. $\square$