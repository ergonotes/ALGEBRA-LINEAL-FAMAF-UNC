**Ejemplo.** Decidir si existe transformacion lineal $T$ de $\mathbb{R}^2$ a $\mathbb{R}^3$ tal que $T(1,1)=(0,-1,1)$ y $T(1,0)=(3,2,1)$
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