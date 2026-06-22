##### **Definición 1.6** Sea $K$ un conjunto, y sean $+$ y $\cdot$ operaciones de $K$. Se dice que $(K, +, \cdot)$ es un _cuerpo_ si $(K, +, \cdot)$ es un anillo conmutativo y todo elemento no nulo de $K$ tiene inverso multiplicativo. Es decir:
1) $(K, +)$ es un grupo conmutativo,
2) $(K - {0}, \cdot)$ es un grupo conmutativo, y
3) vale la propiedad distributiva de $\cdot$ con respecto a $+$.
****
**Para recordarlo de forma más simple.**
Un **cuerpo** (field) es un **anillo conmutativo con una propiedad extra**:
> Todo elemento distinto de cero **tiene inverso multiplicativo**.

Ahora, volviendo a la definición de dominio de integridad, todo cuerpo **es un dominio de integridad**, ya que en un cuerpo:
• Cada elemento $a \ne 0$ **tiene inverso multiplicativo** $a^{-1}$, así que si $a \cdot b = 0$, podemos multiplicar por $a^{-1}$ y obtener:
$$ a^{-1}(a \cdot b) = (a^{-1}a) \cdot b = 1 \cdot b = b = 0, $$
lo que implica que $b = 0$. Por lo tanto, 
> En un cuerpo, no hay forma de que dos elementos distintos de cero se multipliquen y den cero → **no hay divisores de cero**.

**Ejemplos.**  
- $(\mathbb{Q}, +, \cdot),\ (\mathbb{R}, +, \cdot)$ y $(\mathbb{C}, +, \cdot)$ son cuerpos
- $(\mathbb{Z}_p, +, \cdot)$ es un cuerpo $\iff\ p$  es primo.

