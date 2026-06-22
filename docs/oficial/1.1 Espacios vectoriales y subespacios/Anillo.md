La siguiente definición que daremos se refiere a conjuntos en los cuales hay dos operaciones relacionadas entre sí.
##### **Definición 1.4.** Sea $A$ un conjunto y sean $+$ y $·$ operaciones de $A$. Se dice que $(A, +, ·)$ es un anillo si...
1) $(A, +)$ es un grupo conmutativo
2) · es asociativa y tiene elemento neutro
3) Valen las propiedades distributivas: Para $(a, b, c) ∈ (A)$,
	- $a · (b + c) = a · b + a · c$
	- $(b + c) · a = b · a + c · a$
Además, si $·$ es conmutativa, se dice que $(A, +, ·)$ es un anillo conmutativo.
**Notación.** Cuando quede claro cuáles son las operaciones $+$ y $·$, para referirnos al anillo $(A, +, ·)$, escribiremos simplemente $A$. 

**Ejemplos.**
$\bullet$ $(\mathbb{Z}, +, \cdot)$, $(\mathbb{Q}, +, \cdot)$, $(\mathbb{R}, +, \cdot)$ y $(\mathbb{C}, +, \cdot)$ son anillos conmutativos.  
$\bullet$ $(\mathbb{Z}_n, +, \cdot)$ es un anillo conmutativo. 
La notación $\mathbb{Z}_n$​ (o $(Z_n,+,⋅)$ se refiere al **anillo de los enteros módulo $n$**, donde $n$ es un entero positivo ($n \geq 1$). $Z_n$ es el conjunto de los restos obtenidos al dividir cualquier entero por $n$. Es decir, $Z_n = {0, 1, 2, ..., n - 1}$. 
$\bullet$ $\text{Si } (A,+,\cdot)$ es un anillo conmutativo, entonces $(A[X],+,\cdot)$ es un anillo conmutativo con las operaciones usuales de polinomios.
****
Al igual que en el caso de los grupos, también pueden probarse propiedades que poseen todos los anillos:
Sea $(A, +, ·)$ un anillo, y sea $0$ el elemento neutro de +. Entonces $0 · a = 0, ∀ a ∈ A$. Luego se tiene que
$$0 \cdot a = (0 + 0) \cdot a = 0 \cdot a + 0 \cdot a.$$
Si $b$ es el inverso aditivo de $0 · a$, resulta $$ 0 = 0 \cdot a + b = (0 \cdot a + 0 \cdot a) + b = 0 \cdot a + (0 \cdot a + b) = 0 \cdot a. $$Luego, $0 · a = 0$ 

En un anillo cualquiera no es cierto que $a \cdot b = 0 \Rightarrow a = 0 \text{ o } b = 0$. Por ejemplo, en $\mathbb{Z}_4$, se tiene que $2 \cdot 2 = 0$, pero $2 \neq 0$.