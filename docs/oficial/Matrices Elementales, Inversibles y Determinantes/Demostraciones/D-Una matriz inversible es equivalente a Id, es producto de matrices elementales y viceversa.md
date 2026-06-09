Si $A$ es una matriz $n \times n$, los siguientes enunciados son equivalentes.
(i) $A$ es invertible.
(ii) $A$ es equivalente por filas a la matriz identidad $n \times n$.
(iii) $A$ es un producto de matrices elementales.
****
**Demostración.** 
$i) \Rightarrow ii)$ Sea $R$ la matriz escalón reducida por fila equivalente por filas a $A$. Entonces, existen $E_1, \ldots, E_k$ matrices elementales tal que $E_1 \ldots E_k A = R$. Como las matrices elementales son invertibles, el producto de matrices elementales es invertible, luego $E_1, \ldots, E_k$ es invertible y por lo tanto $R = E_1 \ldots E_k A$ es invertible.
Recordemos que las matrices escalón reducidas por fila si tienen filas nulas, ellas se encuentran al final. Ahora bien, si la última fila de $R$ es nula entonces, $RB$ tiene la última fila nula también y por lo tanto no puede ser igual a la identidad, es decir, en ese caso $R$ no es invertible, lo cual produce un absurdo. Concluyendo: la última fila ($f$ila $n$) de $R$ no es nula y como **MERF**, $R$ no tiene filas nulas. Por lo tanto $R=I_n$, y entonces, $A$ es equivalente por filas a $I_n$.

$ii) \Rightarrow iii)$ Como $A$ es equivalente por filas a $I_n$, al ser la equivalencia por filas una relación de equivalencia, tenemos que $I_n$ es equivalente por filas a $A$, es decir existen $E_1, \ldots, E_k$ matrices elementales, tales que $E_1 E_2 \ldots E_k I_n = A$. Por lo tanto, $A = E_1 E_2, \ldots, E_k$ producto de matrices elementales.

$iii) \Rightarrow i)$ Sea $A = E_1 E_2, \ldots, E_k$ donde $E_i$ es una matriz elemental ($i = 1, \ldots, k$). Como cada $E_i$ es invertible, el producto de ellos es invertible, por lo tanto $A$ es invertible. $\square$

