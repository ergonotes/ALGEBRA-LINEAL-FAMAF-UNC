**Proposición.** Sea $T: V \to W$ una transformación lineal. Entonces se cumple que:

1. Si $U$ es un subespacio vectorial de $V$, entonces su **imagen directa**, definida como $T(U) = \{T(u) \mid u \in U\}$, es un subespacio vectorial de $W$.

2. Si $Z$ es un subespacio vectorial de $W$, entonces su **preimagen** (o imagen inversa), definida como $T^{-1}(Z) = \{v \in V \mid T(v) \in Z\}$, es un subespacio vectorial de $V$.
****
**Demostración.**
**Hipótesis:** $U$ es un subespacio de $V$.
**Objetivo:** Probar que $T(U) = \{ T(u) \mid u \in U \}$ es subespacio de $W$.
Como $U$ es un subespacio, sabemos que el vector nulo $0_V$ pertenece a $U$.
Por propiedad de toda transformación lineal, sabemos que $T(0_V) = 0_W$.
Como pudimos fabricar el $0_W$ usando un elemento de $U$, entonces obligatoriamente **$0_W \in T(U)$**.
**Cerradura bajo la suma:**
Tomemos dos vectores cualquiera que ya estén en la imagen, digamos $w_1, w_2 \in T(U)$.
Por definición de imagen, existen dos vectores "origen" $u_1, u_2 \in U$ tales que $T(u_1) = w_1$ y $T(u_2) = w_2$.
Si sumamos los vectores destino:
 $$w_1 + w_2 = T(u_1) + T(u_2)$$Usando el poder de la transformación lineal, agrupamos:
$$w_1 + w_2 = T(u_1 + u_2)$$
Como $U$ es subespacio, la suma $(u_1 + u_2)$ pertenece a $U$. Por lo tanto, acabamos de demostrar que $w_1 + w_2$ es la imagen de un vector válido de $U$. Entonces, **$(w_1 + w_2) \in T(U)$**.
**Cerradura bajo producto por escalar:**
Tomemos un vector $w \in T(U)$ y un escalar $\alpha$. Sabemos que existe un $u \in U$ tal que $T(u) = w$.
Multiplicamos:
$$\alpha w = \alpha T(u)$$
Usando el poder de la transformación lineal, metemos el escalar:
$$\alpha w = T(\alpha u)$$
Como $U$ es subespacio, el vector $(\alpha u)$ pertenece a $U$. Por ende, $\alpha w$ es imagen de un vector de $U$. Entonces, **$\alpha w \in T(U)$**.

$\blacksquare$ **Conclusión 1:** $T(U)$ cumple las tres reglas, es un subespacio vectorial de $W$.

### Parte 2: Demostrar que la preimagen $T^{-1}(Z)$ es un subespacio de $V$

**Hipótesis:** $Z$ es un subespacio de $W$.

**Objetivo:** Probar que $T^{-1}(Z) = \{ v \in V \mid T(v) \in Z \}$ es subespacio de $V$.

_(Recuerda la regla mental aquí: para probar que un vector $v$ pertenece a $T^{-1}(Z)$, tienes que pasarlo por la máquina $T$ y verificar que el resultado aterrice dentro de $Z$)._

1. **El vector nulo está en $T^{-1}(Z)$:**
    
    Pasamos el vector nulo $0_V$ por la máquina: $T(0_V) = 0_W$.
    
    Como $Z$ es un subespacio, sabemos que $0_W \in Z$.
    
    Como el $0_V$ logró aterrizar dentro de $Z$, se gana el derecho a pertenecer a la preimagen. Por lo tanto, **$0_V \in T^{-1}(Z)$**.
    
2. **Cerradura bajo la suma:**
    
    Tomemos dos vectores $v_1, v_2 \in T^{-1}(Z)$. Esto significa que sus destinos cumplen: $T(v_1) \in Z$ y $T(v_2) \in Z$.
    
    Ahora debemos probar si el vector $(v_1 + v_2)$ se gana el derecho a entrar. Lo pasamos por la máquina:
    
    $$T(v_1 + v_2) = T(v_1) + T(v_2)$$
    
    Sabemos que $T(v_1)$ y $T(v_2)$ son vectores que viven en $Z$. Y como $Z$ es un subespacio (cerrado para la suma), la suma de ambos forzosamente vive en $Z$.
    
    Como el destino final de $(v_1 + v_2)$ está en $Z$, entonces el origen **$(v_1 + v_2) \in T^{-1}(Z)$**.
    
3. **Cerradura bajo producto por escalar:**
    
    Tomemos un vector $v \in T^{-1}(Z)$ (lo que significa que $T(v) \in Z$) y un escalar $\alpha$.
    
    Probamos la suerte del vector $(\alpha v)$ pasándolo por la máquina:
    
    $$T(\alpha v) = \alpha T(v)$$
    
    Sabemos que $T(v)$ vive en $Z$. Como $Z$ es un subespacio (cerrado para el producto por escalar), multiplicar ese vector por $\alpha$ nos da un resultado que sigue viviendo en $Z$.
    
    Como el destino de $(\alpha v)$ aterrizó en $Z$, su origen es válido. Por lo tanto, **$\alpha v \in T^{-1}(Z)$**.
    

$\blacksquare$ **Conclusión 2:** $T^{-1}(Z)$ cumple las tres reglas, es un subespacio vectorial de $V$.

¡Y listo! Las dos rutas (ida y vuelta) quedan matemáticamente selladas y demostradas.