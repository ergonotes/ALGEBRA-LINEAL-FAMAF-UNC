**Proposición.** Si $P$ es una matriz invertible $n \times n$ (con coeficientes en $K$), entonces las columnas de $P$ forman una base de $K^n$.
****
**Demostración.** Denotamos $C_1, \dots, C_n$ las columnas de $P$, es decir, $$C_j = \begin{pmatrix} P_{1j} \\ \vdots \\ P_{nj} \end{pmatrix}, \quad j = 1, \dots, n$$
Observemos que
$$
Px = \begin{pmatrix} P_{11}x_1 + \cdots + P_{1n}x_n \\ P_{21}x_1 + \cdots + P_{2n}x_n \\ \vdots \\ P_{n1}x_1 + \cdots + P_{nn}x_n \end{pmatrix} = x_1 \begin{pmatrix} P_{11} \\ \vdots \\ P_{n1} \end{pmatrix} + \cdots + x_n \begin{pmatrix} P_{1n} \\ \vdots \\ P_{nn} \end{pmatrix} = x_1C_1 + \cdots + x_nC_n.
$$

Si $P$ es invertible $\Rightarrow PX = 0$ tiene solo la solución trivial $\Rightarrow \{C_1, \dots, C_n\}$ son L.I.
Para ver que $\{C_1, \dots, C_n\}$ generan $K^n$: sea $Y \in K^n$. Como $P$ es invertible, $\exists X$ tal que $PX = Y$ (diciendo que $P$ es invertible, decimos que siempre podemos encontrar $P^{-1}$ tal que $X = P^{-1}Y$), $\Rightarrow Y$ se puede escribir como combinación lineal de $C_1, \dots, C_n$.
Por lo tanto son base. $\square$