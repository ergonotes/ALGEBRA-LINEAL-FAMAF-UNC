Sea $T: K^n \to K^m$ una transformación lineal. Entonces existen escalares únicos $a_{ij} \in K$ (con $1 \le i \le m$ y $1 \le j \le n$) tales que, para cualquier vector $x = (x_1, x_2, \dots, x_n) \in K^n$, la transformación está dada explícitamente por la fórmula:

$$T(x_1, \dots, x_n) = (a_{11}x_1 + \dots + a_{1n}x_n, \dots, a_{m1}x_1 + \dots + a_{mn}x_n)$$
****
**Demostración.** 
Tomamos un vector cualquiera en el dominio, $$x = (x_1, x_2, \dots, x_n) \in K^n$$
Sabemos que la forma más estándar de fabricar este vector es usando la **base canónica** $E = \{e_1, e_2, \dots, e_n\}$, donde $e_1 = (1,0,\dots,0)$, etc.

Escribimos nuestro vector como una combinación lineal de esta base:

$$x = x_1 e_1 + x_2 e_2 + \dots + x_n e_n$$

Apliquemos la transformación $T$:

$$T(x) = T(x_1 e_1 + x_2 e_2 + \dots + x_n e_n)$$
 luego

$$T(x) = x_1 T(e_1) + x_2 T(e_2) + \dots + x_n T(e_n)$$

Ahora nos fijamos en los términos $T(e_j)$. Estos son los destinos de los vectores canónicos, y sabemos que aterrizan en el espacio de llegada $K^m$.

Vamos a bautizar a esas coordenadas usando la letra $a$, donde el primer subíndice indicará la fila y el segundo indicará de qué vector canónico provienen:

- $T(e_1) = (a_{11}, a_{21}, \dots, a_{m1})$
    
- $T(e_2) = (a_{12}, a_{22}, \dots, a_{m2})$
    
- $\dots$
    
- $T(e_n) = (a_{1n}, a_{2n}, \dots, a_{mn})$
    

$$T(x) = x_1 (a_{11}, a_{21}, \dots, a_{m1}) + x_2 (a_{12}, a_{22}, \dots, a_{m2}) + \dots + x_n (a_{1n}, a_{2n}, \dots, a_{mn})$$

$$T(x) = (a_{11}x_1, a_{21}x_1, \dots, a_{m1}x_1) + (a_{12}x_2, a_{22}x_2, \dots, a_{m2}x_2) + \dots + (a_{1n}x_n, a_{2n}x_n, \dots, a_{mn}x_n)$$

Finalmente, sumamos todas estas tuplas coordenada a coordenada. Juntamos todas las primeras posiciones, luego todas las segundas, y así sucesivamente hasta la posición $m$:

$$T(x) = (a_{11}x_1 + a_{12}x_2 + \dots + a_{1n}x_n, \dots, a_{m1}x_1 + a_{m2}x_2 + \dots + a_{mn}x_n)$$

Y esa es exactamente la fórmula de la proposición

