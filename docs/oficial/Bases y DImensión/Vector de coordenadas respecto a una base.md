En el lenguaje formal del álgebra lineal, la notación **$[v]_B$** significa **el vector de coordenadas** del vector $v$ respecto a la base ordenada $B$.

Si tenemos un espacio vectorial $V$ y una base ordenada $B = \{u_1, u_2, \dots, u_n\}$, sabemos, por teorema, que cualquier vector $v$ se puede escribir de forma única como una combinación lineal:

$$v = \alpha_1 u_1 + \alpha_2 u_2 + \dots + \alpha_n u_n$$

La notación $[v]_B$ lo que hace es ignorar a los vectores de la base y "extraer" únicamente los escalares (tus antiguos $\alpha$ y $\beta$), apilándolos en un vector columna (o fila, dependiendo del autor, pero usualmente columna):

$$[v]_B = \begin{pmatrix} \alpha_1 \\ \alpha_2 \\ \vdots \\ \alpha_n \end{pmatrix}$$

> "El vector $v$ es el plato final; $[v]_B$ es la lista exacta de cantidades que necesitamos para cocinarlo usando la receta $B$."

****
#### **Linealidad del vector de coordenadas**
**Observación.** Sea $V$ un espacio vectorial de dimensión finita $n$ sobre un cuerpo $K$, y sea $B$ una base ordenada de $V$. La función de coordenadas que asigna a cada vector $v \in V$ su vector columna $[v]_B \in K^n$ es una **transformación lineal** (específicamente, un isomorfismo). 
Por lo tanto, para cualesquiera vectores $v, w \in V$ y cualquier escalar $c \in K$, se satisface que: 
$$[v + w]_B = [v]_B + [w]_B$$ y también
$$[cv]_B = c[v]_B$$


