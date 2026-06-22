Repsecto a la definición de **espacio vectorial** otorgada en el apartado [[1.1.2 Espacios vectoriales]], lo que hace la misma es **construir una estructura paso a paso**, primero aclaremos que los elementos de $V$ se llaman _vectores_ y los elementos de $K$ se llaman _escalares_. La acción $\cdot$ se llama _producto por escalares_.
1. **¿Por qué se exige que $V$ sea un conjunto no vacío?**
- Un **espacio vectorial** requiere que haya **elementos (vectores)** para operar.
- Si $V = \varnothing$, no tendría sentido hablar de suma de vectores ni de multiplicación escalar.
- Además, todos los espacios vectoriales **deben tener al menos el vector cero**, así que $V$ no puede estar vacío.
1. **¿Por qué se especifica que $+$ es una operación en $V$?**
Esto significa que: $$ + : V \times V \rightarrow V $$Es decir, **la suma de dos vectores es otro vector**. Esto, entre otras condiciones más adelante, convierte a $V$ en un **grupo abeliano** bajo la suma.

2. **¿Por qué se dice que $\cdot$ es una acción de $K$ en $V$? ¿Por qué no se dice simplemente que es una operación en $V$?**
$\cdot$ no es una operación **interna** en $V$
Una operación interna es algo como $\circ : V \times V \to V$.  
Pero en este caso, la multiplicación escalar es: $$ \cdot : K \times V \rightarrow V $$Es decir, **uno de los elementos proviene del cuerpo $K$** (los escalares), **y el otro del espacio vectorial $V$** (los vectores).