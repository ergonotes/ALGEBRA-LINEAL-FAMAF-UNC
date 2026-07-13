**Proposición.** Sea $T: V \to V$ una transformación lineal en un espacio con producto interno. Las siguientes dos afirmaciones son equivalentes:

1. $T$ es una transformación autoadjunta.
    
2. La matriz asociada $A = [T]_\beta$ es una matriz **simétrica** (es decir, $A = A^t$) para cualquier base **ortonormal** (**BON**) $\beta$ de $V$.
****
**Demostración.**
Veamos ($1 \implies 2$).

Sea $\beta$ una base ortonormal cualquiera de $V$. Llamemos $A = [T]_\beta$ a la matriz de la transformación en dicha base.

Por la [[D-Representación Matricial del Operador Adjunto]], sabemos que la matriz del adjunto $T^*$ en una base ortonormal es exactamente la traspuesta de la matriz original. Es decir:

$$[T^*]_\beta = A^t$$

Supongamos que la afirmación 1 es cierta, es decir, que $T$ es autoadjunta.

Por definición, esto significa que:

$$T = T^*$$

Si dos transformaciones lineales son exactamente la misma, sus matrices asociadas en una misma base deben ser idénticas:

$$[T]_\beta = [T^*]_\beta$$

Reemplazando cada lado por sus respectivas matrices ($A$ y $A^t$):

$$A = A^t$$

Esto significa, por definición, que la matriz $A$ es simétrica. Queda probada la primera implicación.

**Veamos ($2 \implies 1$).**

Supongamos que la afirmación 2 es cierta, es decir, que la matriz $A = [T]_\beta$ es simétrica ($A = A^t$).

Por el teorema de la matriz del adjunto, sabemos que $A^t = [T^*]_\beta$. Sustituyendo esto en la igualdad de simetría obtenemos:

$$[T]_\beta = [T^*]_\beta$$

Sabemos que la asignación de matrices a transformaciones lineales (fijada una base) es un isomorfismo (es decir, es una relación biyectiva). Si las matrices de dos transformaciones son iguales, las transformaciones mismas deben ser iguales:

$$T = T^*$$

Esto, por definición, significa que $T$ es un operador autoadjunto. Queda probada la segunda implicación.