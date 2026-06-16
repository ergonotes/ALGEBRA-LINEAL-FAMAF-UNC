**Ejemplo 1.** Sea $V = \mathbb{P}_2$ el espacio vectorial de los polinomios de grado $\le 2$. Definimos el operador derivada $D: \mathbb{P}_2 \to \mathbb{P}_2$ tal que a cada polinomio $p(x)$ le asigna su derivada $p'(x)$:

$$D(ax^2 + bx + c) = 2ax + b$$

Para demostrar que $D$ es una transformación lineal, verificamos que cumple las dos propiedades fundamentales:

**Preserva la suma (Aditividad).**
Sean $p(x)$ y $q(x)$ dos polinomios cualesquiera en $\mathbb{P}_2$.

$$D(p(x) + q(x)) = \frac{d}{dx}[p(x) + q(x)] = p'(x) + q'(x) = D(p(x)) + D(q(x))$$

**Preserva el producto por escalar.**
Sea $p(x) \in \mathbb{P}_2$ y $\alpha$ un escalar. 

$$D(\alpha p(x)) = \frac{d}{dx}[\alpha p(x)] = \alpha p'(x) = \alpha D(p(x))$$

Como el operador $D$ preserva tanto la suma vectorial como el producto por escalares, se demuestra formalmente que la derivación es una transformación lineal.
****
**Ejemplo 2.** Sea $P$ una matriz $m \times m$ dada, con elementos en el cuerpo $F$, y sea $Q$ otra matriz $n \times n$ dada, sobre $F$. Se define una función $T$ del espacio $F^{m \times n}$ en sí mismo por $T(A) = PAQ$. Entonces $T$ es una transformación lineal de $F^{m \times n}$ en $F^{m \times n}$, porque

$$
\begin{aligned}
T(cA + B) &= P(cA + B)Q \\
&= (cPA + PB)Q \\
&= cPAQ + PBQ \\
&= cT(A) + T(B).
\end{aligned}
$$
Es importante aclarar que cuando se dice "*T es una función del espacio $F^{m×n}$ en sí mismo*", es equivalente a decir, _"Esta trasnformación solo acepta matrices de tamaño $m×n$ como monedas de entrada_"
****
Ejemplo 3. Si $V$ es cualquier espacio vectorial, la **transformación identidad** $I$, definida por $I\alpha = \alpha$, es una transformación lineal de $V$ en $V$. La **transformación cero** $0$, definida por $0\alpha = 0$, es una transformación lineal de $V$ en $V$.