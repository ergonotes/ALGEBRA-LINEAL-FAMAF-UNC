**Definición 1.2.0** Se dice que la matriz $A$ es inversible si existe una matriz $B$ (necesariamente del mismo orden que $A$) llamada inversa de $A$, tal que $$BA = AB = I$$Caso contrario se dice que $A$ es no inversible.
El ejemplo trivial de matriz invertible es la matriz identidad. Otro ejemplo se vé en el apartado [[E-Matriz inversible]]. 
****
#### **Lema**. **Si $A$ tiene una inversa a la izquierda, $B$, y una inversa a la derecha, $C$, entonces $B = C$.**
**Demostración**. Supóngase que $BA = I$ y que $AC = I$. Entonces
$$B = BI = B(AC) = (BA)C = IC = C. \quad \blacksquare$$
****
Así, si $A$ es inversa a la izquierda e inversa a la derecha, $A$ es invertible y tiene una inversa bilátera que se representará por $A^{-1}$ y se llamará simplemente la inversa de $A$.
****
#### **Teorema 10.** **Sean $A$ y $B$ dos matrices $n \times n$ sobre $F$.**
1. Si $A$ es invertible, también lo es $A^{-1}$ y $(A^{-1})^{-1} = A$.
2. Si $A$ y $B$ son invertibles, también lo es $AB$ y $(AB)^{-1} = B^{-1}A^{-1}$.
**Demostración**. La primera afirmación es evidente por la simetría de la definición. La segunda se desprende de las relaciones$$(B^{-1}A^{-1})(AB)= B^{-1}(A^{-1}A)B = B^{-1}(I)B= (B^{-1}B) = I. \quad \blacksquare$$Haciendo lo mismo para $(AB)(B^{-1}A^{-1})$.
****
#### **Corolario**. **Un producto de matrices inversibles es inversible**.
****
#### **Teorema 11. Una matriz elemental es invertible.**
**Demostración**. Sea $E$ una matriz fundamental correspondiente a la operación elemental de fila $e$. Si $e_1$ es la operación inversa de $e$ y $E_1 = e_1(I)$, entonces
$$EE_1 = e(E_1) = e(e_1(I)) = I$$
y
$$E_1E = e_1(E) = e_1(e(I)) = I$$
con lo que $E$ es invertible y $E_1 = E^{-1}$. $\blacksquare$
([[E-Inversas de Matrices Elementales]])
****
#### **Teorema 12. Si $A$ es una matriz $n \times n$, los siguientes enunciados son equivalentes.**
1. $A$ es invertible.
2. $A$ es equivalente por filas a la matriz identidad $n \times n$.
3. $A$ es un producto de matrices elementales.
(**[[D-Una matriz inversible es equivalente a Id, es producto de matrices elementales y viceversa]]**)
****
#### **Observación**. Sea $R$ una matriz $n \times n$ escalón reducida por fila tal que no tiene filas nulas. 
Entonces $R = I_n$.
****
#### **Corolario**. Sean $A$ y $B$ matrices $m \times n$. Entonces, $B$ es equivalente por filas a $A$ si y sólo si existe matriz invertible $P$ de orden $m \times m$ tal que $B = PA$.
**Demostración.** $(\Rightarrow)$ $B$ es equivalente por filas a $A$, luego existe $P$ matriz producto de matrices elementales tal que $B = PA$. Como cada matriz elemental es invertible, y el producto de matrices invertibles es invertible, se deduce que $P$ es invertible.

$(\Leftarrow)$ Sea $P$ matriz invertible tal que $B = PA$. Como $P$ es invertible, por el teorema anterior, $P$ es producto de matrices elementales, luego $B = PA$ es equivalente por filas a $A$. $\square$
****
#### **Corolario**. Sea $A$ matriz $n \times n$. Sean $e_1, \ldots, e_k$ las operaciones elementales...
por filas que reducen a $A$ a una **MERF** y esta **MERF** es la identidad, es decir $e_1(e_2(\ldots (e_k(A))\ldots)) = I_n$. Entonces, $A$ invertible y las mismas operaciones elementales aplicadas a $I_n$ nos llevan a $A^{-1}$, es decir $e_1(e_2(\ldots (e_k(I_n))\ldots)) = A^{-1}$.

**Demostración**. Por el teorema anterior, al ser $A$ equivalente por filas a la identidad, $A$ es invertible. Sean las matrices elementales $E_i = e_i(I_n)$ para $i=1, \ldots, k$, entonces (ver corolario 1.4.2) $E_1 E_2 \ldots E_k A = I_n$, por lo tanto, multiplicando por $A^{-1}$ a derecha en ambos miembros,
$$E_1 E_2 \ldots E_k AA^{-1} = I_n A^{-1} \iff$$
$$E_1 E_2 \ldots E_k I_n = A^{-1} \iff$$
$$e_1(e_2(\ldots (e_k(I_n))\ldots)) = A^{-1}.$$
****
#### **Teorema**. **Sea $A$ matriz $n \times n$ con coeficientes en $K$. Entonces, las siguientes afirmaciones son equivalentes.**
$i)$ $A$ es invertible.
$ii)$ El sistema $AX = Y$ tiene una única solución para toda matriz $Y$ de orden $n \times 1$.
$iii)$ El sistema homogéneo $AX = 0$ tiene una única solución trivial.
**[[D-El sistema de ecuaciones asociado a una matriz inversible tiene una y solo una solución]]**
****
#### **Corolario.** **[[D-Una matriz cuadrada que tiene una inversa a la izquierda o a la derecha es inversible]].**
