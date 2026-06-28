#### **Teorema**. **Sea $A$ matriz $n \times n$ con coeficientes en $K$. Entonces, las siguientes afirmaciones son equivalentes.**
$i)$ $A$ es invertible.
$ii)$ El sistema $AX = Y$ tiene una única solución para toda matriz $Y$ de orden $n \times 1$.
$iii)$ El sistema homogéneo $AX = 0$ tiene una única solución trivial.
****
**Demostración**.
$i) \Rightarrow ii)$ Sea $X_0$ solución del sistema $AX = Y$, luego
$$ AX_0 = Y \Rightarrow A^{-1}AX_0 = A^{-1}Y \Rightarrow X_0 = A^{-1}Y. $$
Es decir, $X_0$ es único (siempre igual a $A^{-1}Y$).

$ii) \Rightarrow i)$ Es trivial, tomando $Y=0$.
$iii) \Rightarrow i)$ Sea $R$ la matriz escalón reducida por filas equivalente a $A$, es decir $R = PA$ con $P$ invertible y $R$ es MERF. Si $R$ tiene una fila nula, entonces por teorema 1.2.5, el sistema $AX = 0$ tiene más de una solución, lo cual es absurdo. Por lo tanto, $R$ no tiene filas nulas. Como es una matriz cuadrada y es MERF, tenemos que $R = I_n$. Luego $A$ es equivalente por filas a $I_n$ y por teorema anterior ([[D-Una matriz inversible es equivalente a Id, es producto de matrices elementales y viceversa]]) se deduce que $A$ es invertible. $\square$
