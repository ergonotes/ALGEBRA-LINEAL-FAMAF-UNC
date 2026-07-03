**Proposición.** Sea $V$ un espacio vectorial de dimensión finita sobre un cuerpo $K$, y sea $T: V \to V$ una transformación lineal. Sea $I: V \to V$ la transformación identidad. Para cualquier escalar $\lambda \in K$, las siguientes afirmaciones son equivalentes:

1. $\lambda$ es un autovalor de $T$.
    
2. $\det(\lambda I - T) = 0$.

****
**Demostración.** Veremos que se cumple el **sí sólo sí**:
Por definición, decimos que $\lambda \in K$ es un autovalor de $T$ si y solo si existe un vector $v \in V$ no nulo ($v \neq 0$) tal que la transformación de ese vector es un múltiplo escalar de sí mismo:

$$T(v) = \lambda v$$

Sabemos que aplicar un escalar a un vector es lo mismo que aplicarle la transformación identidad $I$ multiplicada por ese escalar ($\lambda v = \lambda I(v)$):

$$T(v) = \lambda I(v)$$

 Luego 

$$\lambda I(v) - T(v) = 0$$

Por la linealidad, podemos agrupar las transformaciones que se están aplicando al mismo vector $v$:

$$(\lambda I - T)(v) = 0$$

Llegamos a que la transformación lineal $(\lambda I - T)$ aplicada a un vector $v$ (que sabemos que es **distinto de cero**) da como resultado el vector nulo.

Por definición, el conjunto de vectores que se transforman en cero forma el **núcleo** (o kernel) de la transformación. Como $v \neq 0$, esto significa que el núcleo de $(\lambda I - T)$ contiene más elementos que solo el vector nulo. Es decir, el núcleo no es trivial:

$$\ker(\lambda I - T) \neq \{0\}$$

 Sabemos [[D-Una transformación lineal es un monomorfismo si y solo si su núcleo es el subespacio trivial]] y, en consecuencia, **no es invertible** (es una matriz singular, y no cumple las condiciones vistas en el inciso [[3.Isomorfismos de espacios vectoriales]]).
 
 En otras palabras, la transformación $\lambda I - T$ manda a un vector $v\neq0$ al $0$, es decir, aplasta el espacio, por lo que el determinante de esta transformación es cero. 

$$\det(\lambda I - T) = 0$$

