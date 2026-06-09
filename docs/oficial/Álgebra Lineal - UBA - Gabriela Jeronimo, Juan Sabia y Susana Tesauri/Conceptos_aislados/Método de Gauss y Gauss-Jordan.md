### Método de Gauss (o *eliminación de Gauss*)
- Se usa para transformar la matriz en **forma triangular superior**.  
- Es decir, se hacen ceros **debajo** de los pivotes, pero no se toca lo que queda arriba.  
Ejemplo de resultado típico (matriz triangular superior):
$$\begin{bmatrix}
* & * & * \\
0 & * & * \\
0 & 0 & *
\end{bmatrix}$$
---
### Método de Gauss–Jordan (o *eliminación completa*)
- Se continúa eliminando hasta dejar la matriz en **forma reducida por filas** (*forma escalonada reducida*).  
- Esto significa que no solo hay ceros debajo de cada pivote, sino también **arriba**.  
- Cada pivote es \($1$\) y es el único número distinto de cero en su columna.  
- Se puede leer la solución del sistema **directamente**.  
Ejemplo de resultado típico (matriz reducida por filas):$$
\begin{bmatrix}
1 & 0 & 0 \\
0 & 1 & 0 \\
0 & 0 & 1
\end{bmatrix}
$$Este método en particular es el mencionado en el apartado de **[[2.4.1 Matrices reducidas por filas]]** del libro.

---
### **🔹 ¿Para qué se usa cada uno?**
- **Gauss**  
  - Más rápido y eficiente.  
  - Ideal para resolver sistemas grandes en cálculo numérico.  
  - Se usa mucho en programación y aplicaciones prácticas.  
- **Gauss–Jordan**  
  - Útil en teoría y para sistemas pequeños.  
  - Permite obtener la solución general directamente.  
  - Método natural para calcular la inversa de una matriz:
$$    
    [A \,|\, I] \;\;\xrightarrow{\text{Gauss–Jordan}}\;\; [I \,|\, A^{-1}]
    $$
