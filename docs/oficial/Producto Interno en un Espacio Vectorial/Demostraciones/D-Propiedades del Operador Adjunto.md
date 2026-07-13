**Proposición.** Sean $T, S: V \to V$ transformaciones lineales en un espacio vectorial $V$ sobre $\mathbb{R}$ provisto de un producto interno. Entonces, se cumplen las siguientes propiedades:

1. $(Id)^* = Id$  _(El adjunto de la identidad es la identidad)._
    
2. $(T+S)^* = T^* + S^*$
    
3. $(cT)^* = cT^*$ para todo escalar $c \in \mathbb{R}$.
    
4. $(TS)^* = S^* T^*$ _(El adjunto de una composición invierte el orden)._
    
5. $(T^*)^* = T$ _(El adjunto del adjunto es el operador original)._
****
**Demostración.**
Veamos **1**).
Evaluamos el adjunto de la identidad por definición:

$$\langle v, (Id)^*(w) \rangle = \langle Id(v), w \rangle$$

Como la función identidad no le hace nada al vector ($Id(v) = v$):

$$= \langle v, w \rangle$$

Y podemos reescribir a $w$ como $Id(w)$:

$$= \langle v, Id(w) \rangle$$

Como $\langle v, (Id)^*(w) \rangle = \langle v, Id(w) \rangle$ para cualquier par de vectores, concluimos que $(Id)^* = Id$. 

Ahora veamos **2**)
Planteamos la definición para la suma:

$$\langle v, (T+S)^*(w) \rangle = \langle (T+S)(v), w \rangle$$

Por definición de suma de transformaciones lineales:

$$= \langle T(v) + S(v), w \rangle$$

Por la propiedad de linealidad (distributiva) del producto interno:

$$= \langle T(v), w \rangle + \langle S(v), w \rangle$$

Aplicamos la definición de adjunto individualmente a $T$ y a $S$:

$$= \langle v, T^*(w) \rangle + \langle v, S^*(w) \rangle$$

Volvemos a usar la linealidad del producto interno (esta vez "hacia atrás"):

$$= \langle v, T^*(w) + S^*(w) \rangle$$

$$= \langle v, (T^*+S^*)(w) \rangle$$

Concluimos que $(T+S)^* = T^* + S^*$. 

Veamos **3**).
_(Nota: Lo siguiente funciona directo porque estamos en $\mathbb{R}$. Si estuviéramos en los complejos $\mathbb{C}$, el escalar saldría conjugado)._

Planteamos:

$$\langle v, (cT)^*(w) \rangle = \langle (cT)(v), w \rangle$$

$$= \langle c \cdot T(v), w \rangle$$

Sacamos el escalar $c$ del producto interno (por linealidad en la primera componente):

$$= c \langle T(v), w \rangle$$

Aplicamos la definición de adjunto para $T$:

$$= c \langle v, T^*(w) \rangle$$

Volvemos a meter el escalar dentro del producto interno, en la segunda componente (como estamos en $\mathbb{R}$, entra tal cual):

$$= \langle v, c \cdot T^*(w) \rangle$$

$$= \langle v, (cT^*)(w) \rangle$$

Concluimos que $(cT)^* = cT^*$.

Veamos **4**).
Recordemos que $TS$ significa la composición $T(S(v))$.

$$\langle v, (TS)^*(w) \rangle = \langle (TS)(v), w \rangle$$

$$= \langle T(S(v)), w \rangle$$

Primero aplicamos la definición del adjunto para "despegar" $T$ y pasarla al otro lado:

$$= \langle S(v), T^*(w) \rangle$$

Ahora aplicamos la definición del adjunto para "despegar" $S$ y pasarla al otro lado:

$$= \langle v, S^*(T^*(w)) \rangle$$

$$= \langle v, (S^*T^*)(w) \rangle$$

Concluimos que $(TS)^* = S^* T^*$.

Veamos **5**).
Planteamos la definición para el "adjunto del adjunto":

$$\langle v, (T^*)^*(w) \rangle = \langle T^*(v), w \rangle$$

Como estamos en $\mathbb{R}$, el producto interno es **simétrico** ($\langle x, y \rangle = \langle y, x \rangle$). Usamos esto para dar vuelta los vectores:

$$= \langle w, T^*(v) \rangle$$

Ahora, por definición del adjunto de $T$, pasamos la $T$ hacia el primer vector:

$$= \langle T(w), v \rangle$$

Volvemos a aplicar la simetría del producto interno para acomodarlos en el orden original:

$$= \langle v, T(w) \rangle$$

Al haber llegado a que $\langle v, (T^*)^*(w) \rangle = \langle v, T(w) \rangle$, queda demostrado que $(T^*)^* = T$.