**Ejemplo.** Decidir si existe transformación lineal $T$ de $\mathbb{R}^2$ a $\mathbb{R}^3$ tal que $T(1,1)=(0,-1,1)$ y $T(1,0)=(3,2,1)$
****
**Solución.** Tomamos un vector cualquiera $(x,y)$ y buscamos los escalares $\alpha$ y $\beta$ para fabricarlo con tus ingredientes, lo hacemos de esta forma sabiendo que $(1,0)$ y $(1,1)$ forman una base de $\mathbb{R}^2$
$$(x,y) = \alpha(1,1) + \beta(1,0)$$$$(x,y) = (\alpha + \beta, \alpha)$$De aquí deducimos rápidamente el sistema de ecuaciones:
- $\alpha = y$

- $\alpha + \beta = x \Rightarrow \beta = x - y$

Sabiendo que $(x,y) = y(1,1) + (x-y)(1,0)$, aplicamos $T$ a ambos lados. Como es una transformación lineal, respeta sumas y saca escalares:
$$T(x,y) = y \cdot T(1,1) + (x-y) \cdot T(1,0)$$Sustituimos $T(1,1)$ por $(0,-1,1)$ y $T(1,0)$ por $(3,2,1)$:
$$T(x,y) = y(0,-1,1) + (x-y)(3,2,1)$$
$$T(x,y) = (0, -y, y) + (3x-3y, 2x-2y, x-y)$$
Sumamos coordenada a coordenada:
$$T(x,y) = (3x-3y, 2x-3y, x)$$
****
Ejemplo 2. Los vectores
$$
\begin{aligned}
\alpha_1 &= (1, 2) \\
\alpha_2 &= (3, 4)
\end{aligned}
$$
son linealmente independientes y, por tanto, forman una base de $\mathbb{R}^2$. De acuerdo con el Teorema 1, existe una única transformación lineal de $\mathbb{R}^2$ en $\mathbb{R}^2$ tal que
$$
\begin{aligned}
T\alpha_1 &= (3, 2, 1) \\
T\alpha_2 &= (6, 5, 4)
\end{aligned}
$$
De ser así, se debe poder encontrar $T(\epsilon_1)$. Encontrados los escalares $c_1, c_2$ tales que $\epsilon_1 = c_1\alpha_1 + c_2\alpha_2$, se sabe entonces que $T\epsilon_1 = c_1T\alpha_1 + c_2T\alpha_2$. Si $(1, 0) = c_1(1, 2) + c_2(3, 4)$, entonces $c_1 = -2$ y $c_2 = 1$. Con lo que
$$
\begin{aligned}
T(1, 0) &= -2(3, 2, 1) + (6, 5, 4) \\
&= (0, 1, 2).
\end{aligned}
$$