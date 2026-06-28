Veamos cuales son las matrices elementales $2 \times 2$.$\text{(1) Si } c \ne 0, \text{ multiplicar por } c \text{ la primera fila y multiplicar por } c \text{ la segunda fila son}$$$\begin{bmatrix}
c & 0 \\
0 & 1
\end{bmatrix},
\begin{bmatrix}
1 & 0 \\
0 & c
\end{bmatrix}$$$\text{(2) Si } c \in \mathbb{K}, \text{ sumar a la fila 2 la fila 1 multiplicada por } c$ $\text{ o sumar a la fila 1 la fila 2 }\text{multiplicada por } c \text{ son respectivamente.}$   $$\begin{bmatrix}
    1 & 0 \\
    c & 1
    \end{bmatrix},
    \begin{bmatrix}
    1 & c \\
    0 & 1
    \end{bmatrix}$$$\text{(3) Finalmente, intercambiando la fila 1 por la fila 2 obtenemos la matriz}$
$$\begin{bmatrix}
0 & 1 \\
1 & 0
\end{bmatrix}
$$
****
$\text{En el caso de matrices } m \times m \text{ tampoco es difícil encontrar las matrices elementales:}$$\text{(1) Si } c \ne 0, \text{ multiplicar por } c \text{ la fila } k$ $\text{ de la matriz identidad, resulta en la matriz elemental}$ $\text{que tiene todos 1's en la diagonal, excepto en la posición } k,$ 
$k \text{ donde vale } c, \text{ es decir si} \\e(I_m) = [a_{ij}], \text{ entonces}$
$$a_{ij} = \begin{cases}
1 & \text{si } i = j \text{ e } i \ne k, \\
c & \text{si } i = j = k, \\
0 & \text{si } i \ne j.
\end{cases}$$$\text{Gráficamente,}$ $$
\begin{array}{c}
\overset{k}{\downarrow} \\
\begin{bmatrix}
1 & 0 & \cdots & 0 \\
\vdots & \vdots &  & \vdots \\
0 & \cdots & c & \cdots & 0 \\
\vdots &  & \vdots & & \vdots \\
0 &  & \cdots & & 1 \end{bmatrix}
 \end{array} \\ $$
$\text{(2) si } c \in \mathbb{K}, \text{ sumar a la fila } r \text{ la fila } s$ 
$\text{ multiplicada por } c, \text{ resulta en la matriz elemental que}$$\text{tiene todos 1's en la diagonal, y todos los demás coeficientes son 0, excepto en la fila } r$$\text{y columna } s \text{ donde vale } c, \text{ es decir si } e(I_m) = [a_{ij}], \text{ entonces}$ 
$$a_{ij} = \begin{cases}
1 & \text{si } i = j \\    
c & \text{si } i = r, j = s, \\
0 & \text{otro caso}.  
\end{cases}
$$
$\text{Gráficamente,}$ $$\begin{array}{c} \overset{r}{\downarrow} \ \ \ \ 
    \overset{s}{\downarrow} \\
    \begin{bmatrix}
    1 & 0 & \cdots & 0 \\
    \vdots & \vdots &  & \vdots \\
    0 & \cdots & 1 & c & \cdots & 0 \\
    \vdots &  & \vdots & & \vdots \\
    0 &  & \cdots & & & 1
    \end{bmatrix}
    \end{array}$$ $\text{(3) Finalmente, intercambiar la fila } r \text{ por la fila } s$ $\text{ resulta ser}$ 
  $$\qquad a_{ij} = \begin{cases}
    1 & \text{si } (i = j, i \ne r, i \ne s) \text{ o } (i = r, j = s) \text{ o } (i = s, j = r) \\
    0 & \text{otro caso}.
    \end{cases}$$ 
$\text{Gráficamente,}$ 
$$\begin{array}{c}\ \ \ \ \ \ \ \ \overset{r}{\downarrow} \qquad \ \overset{s}{\downarrow} \\
    \begin{bmatrix}
    1 &  &  &  & & 0 \\
    & \ddots &  &  &  &  \\
    &  & 0 & \cdots & 1 &  \\
    &  & \vdots & \ddots & \vdots &  \\
    &  & 1 & \cdots & 0 &  \\
    0 &  &  &  &  & 1
    \end{bmatrix}
    \end{array}$$
