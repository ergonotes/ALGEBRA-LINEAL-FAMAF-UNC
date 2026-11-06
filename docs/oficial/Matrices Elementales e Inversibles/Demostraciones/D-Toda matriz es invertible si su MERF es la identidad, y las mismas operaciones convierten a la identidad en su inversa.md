**Corolario**. Sea $A$ matriz $n \times n$. Sean $e_1, \ldots, e_k$ las operaciones elementales por filas que reducen a $A$ a una **MERF** y esta **MERF** es la identidad, es decir $e_1(e_2(\ldots (e_k(A))\ldots)) = I_n$. Entonces, $A$ invertible y las mismas operaciones elementales aplicadas a $I_n$ nos llevan a $A^{-1}$, es decir $e_1(e_2(\ldots (e_k(I_n))\ldots)) = A^{-1}$.
****
**Demostración**. Por el teorema anterior, al ser $A$ equivalente por filas a la identidad, $A$ es invertible. Sean las matrices elementales $E_i = e_i(I_n)$ para $i=1, \ldots, k$, entonces (ver corolario 1.4.2) $E_1 E_2 \ldots E_k A = I_n$, por lo tanto, multiplicando por $A^{-1}$ a derecha en ambos miembros,
$$E_1 E_2 \ldots E_k AA^{-1} = I_n A^{-1} \iff$$
$$E_1 E_2 \ldots E_k I_n = A^{-1} \iff$$
$$e_1(e_2(\ldots (e_k(I_n))\ldots)) = A^{-1}.$$