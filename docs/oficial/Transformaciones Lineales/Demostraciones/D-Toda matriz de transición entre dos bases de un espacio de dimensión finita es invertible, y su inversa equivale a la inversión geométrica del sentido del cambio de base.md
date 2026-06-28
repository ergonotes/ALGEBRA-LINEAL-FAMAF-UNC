**Corolario.** $V$ espacio vectorial sobre $\mathbb{K}$. Sea $\beta, \beta'$ dos bases de $V$. 

Entonces la matriz de cambio de base de $\beta$ a $\beta'$ $P = [\text{Id}]_{\beta}^{\beta'}$ es una matriz invertible y su inversa es $P^{-1} = [\text{Id}]_{\beta'}^{\beta} = \text{matriz de cambio de base de } \beta' \text{ a } \beta$.
****
**Demostración.** $Q = [\text{Id}]_{\beta'}^{\beta}$, $P = [\text{Id}]_{\beta}^{\beta'}$, 

Al multiplicar ambas matrices, la base intermedia $\beta'$ actúa como el puente que se fusiona con las coordenadas de la otra base, y la expresión termina quedando en términos de la base $\beta$, es lo que se hace en particular para la demostración de la [[D-Representación Matricial de la Composición]], entonces
 $$[\text{Id}]_{\beta'}^{\beta} [\text{Id}]_{\beta}^{\beta'} = [\text{Id} \circ \text{Id}]_{\beta}^{\beta} $$
 Luego, por las [[D-Propiedades de Operadores en una misma base]] (2) y sabiendo que la base de entrada y salida son la misma,
 $$= [\text{Id}]_{\beta}^{\beta} = \text{Id} = \text{matriz identidad}$$

$$\Rightarrow Q \cdot P = \text{Id}$$