**Definición 1.2.0** Se dice que la matriz $A$ es inversible si existe una matriz $B$ (necesariamente del mismo orden que $A$) llamada inversa de $A$, tal que $$BA = AB = I$$Caso contrario se dice que $A$ es no inversible.
El ejemplo trivial de matriz invertible es la matriz identidad. Otro ejemplo se vé en el apartado [[E-Matriz inversible]]. 
****
#### **La inversa de una Matriz es ÚNICA**
**Lema**. **Si $A$ tiene una inversa a la izquierda, $B$, y una inversa a la derecha, $C$, entonces $B = C$.**
**Demostración**. Supóngase que $BA = I$ y que $AC = I$. Entonces
$$B = BI = B(AC) = (BA)C = IC = C. \quad \blacksquare$$
****
Así, si $A$ es inversa a la izquierda e inversa a la derecha, $A$ es invertible y tiene una inversa bilátera que se representará por $A^{-1}$ y se llamará simplemente la inversa de $A$.
****
#### **Inversa de la Inversa, y Producto de matrices Invertibles**
**Teorema 10.** **Sean $A$ y $B$ dos matrices $n \times n$ sobre $F$.**
1. Si $A$ es invertible, también lo es $A^{-1}$ y $(A^{-1})^{-1} = A$.
2. Si $A$ y $B$ son invertibles, también lo es $AB$ y $(AB)^{-1} = B^{-1}A^{-1}$.
**Demostración**. La primera afirmación es evidente por la simetría de la definición. La segunda se desprende de las relaciones$$(B^{-1}A^{-1})(AB)= B^{-1}(A^{-1}A)B = B^{-1}(I)B= (B^{-1}B) = I. \quad \blacksquare$$Haciendo lo mismo para $(AB)(B^{-1}A^{-1})$.
****
#### **Corolario**. **Un producto de matrices inversibles es inversible**.
Como vimos en el teorema anterior.
****
#### **Teorema 11. Una matriz elemental es invertible.**
**Demostración**. Sea $E$ una matriz fundamental correspondiente a la operación elemental de fila $e$. Si $e_1$ es la operación inversa de $e$ y $E_1 = e_1(I)$, entonces
$$EE_1 = e(E_1) = e(e_1(I)) = I$$
y
$$E_1E = e_1(E) = e_1(e(I)) = I$$
con lo que $E$ es invertible y $E_1 = E^{-1}$. $\blacksquare$
([[E-Inversas de Matrices Elementales]])
****
#### **No toda Matriz Cuadrada es Invertible**
Sea la matriz cuadrada $A$ de tamaño $2 \times 2$:
$$
A = \begin{pmatrix} 1 & 2 \\ 2 & 4 \end{pmatrix}
$$
si comenzamos a reducir por filas, encontraremos una fila nula, por lo que $A$ no es equivalente a $I$.
****
#### **La suma de dos Matrices Invertibles puede no ser Invertible**
Sabemos $I$ tiene inversa $I^{-1}=I$, y $-I$ tiene inversa $-I^{-1}=-I$, luego: 
$$
I + (-I) = \begin{pmatrix} 1 & 0 \\ 0 & 1 \end{pmatrix} + \begin{pmatrix} -1 & 0 \\ 0 & -1 \end{pmatrix} = \begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix}
$$
y la matriz nula no es invertible.
****
#### **Caracterización de Matrices Invertibles** 
**Teorema 12. Si $A$ es una matriz $n \times n$, los siguientes enunciados son equivalentes.**
1. $A$ es invertible.
2. $A$ es equivalente por filas a la matriz identidad $n \times n$.
3. $A$ es un producto de matrices elementales.
(**[[D-Una matriz inversible es equivalente a Id, es producto de matrices elementales y viceversa]]**)
****
#### Toda matriz cuadrada en forma MERF es la identidad si no tiene filas nulas
**Observación**. Sea $R$ una matriz $n \times n$ escalón reducida por fila tal que no tiene filas nulas. Entonces $R = I_n$.
****
#### [[D-Dos matrices son equivalentes por filas si y sólo si una resulta de multiplicar la otra por una matriz invertible]]
**Corolario**. Sean $A$ y $B$ matrices $m \times n$. Entonces, $B$ es equivalente por filas a $A$ si y sólo si existe matriz invertible $P$ de orden $m \times m$ tal que $B = PA$.
****
#### [[D-Toda matriz es invertible si su MERF es la identidad, y las mismas operaciones convierten a la identidad en su inversa]]
**Corolario**. Sea $A$ matriz $n \times n$. Sean $e_1, \ldots, e_k$ las operaciones elementales por filas que reducen a $A$ a una **MERF** y esta **MERF** es la identidad, es decir $e_1(e_2(\ldots (e_k(A))\ldots)) = I_n$. Entonces, $A$ invertible y las mismas operaciones elementales aplicadas a $I_n$ nos llevan a $A^{-1}$, es decir $e_1(e_2(\ldots (e_k(I_n))\ldots)) = A^{-1}$.
****
### **[[D-El sistema de ecuaciones asociado a una matriz inversible tiene una y solo una solución]]**
**Teorema**. Sea $A$ matriz $n \times n$ con coeficientes en $K$. Entonces, las siguientes afirmaciones son equivalentes.

$i)$ $A$ es invertible.

$ii)$ El sistema $AX = Y$ tiene una única solución para toda matriz $Y$ de orden $n \times 1$.

$iii)$ El sistema homogéneo $AX = 0$ tiene una única solución trivial.

**Corolario (consecuencia).** Un sistema lineal homogéneo $Bx=0$ tiene solución no trivial sí y sólo si $B$ es no inversible.
****
#### **Corolario.** **[[D-Una matriz cuadrada que tiene una inversa a la izquierda o a la derecha es inversible]].**
****
#### **Cálculo de la Inversa mediante reducción por filas**
Si tenemos que
$$
A \xrightarrow{e_1} \xrightarrow{e_2} \xrightarrow{e_3} I.
$$
Las mismas operaciones sobre la identidad producen
$$
I \xrightarrow{e_1} \xrightarrow{e_2} \xrightarrow{e_3} A^{-1}.
$$
Por eso:
$$
[A \mid I] \longrightarrow [I \mid A^{-1}].
$$
****
[[Criterio de Inversibilidad para Diagonal de Matrices]]
****
[[Inversa de una matriz 2x2]]
