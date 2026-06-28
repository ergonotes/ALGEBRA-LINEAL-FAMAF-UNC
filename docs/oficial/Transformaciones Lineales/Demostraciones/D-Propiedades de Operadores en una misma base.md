**Corolario.** $V$ espacio vectorial sobre $\mathbb{K}$, $\beta$ base de $V$, $\dim V = n < \infty$. Sean $T: V \to V, S: V \to V$ lineales. Entonces:

1) $[S \circ T]_{\beta} = [S]_{\beta} [T]_{\beta}$

2) Si $\text{Id}: V \to V$ (transformación identidad) $\Rightarrow [\text{Id}]_{\beta} = Id = \text{matriz identidad}$

3) Si $T$ es invertible $\Rightarrow [T]_{\beta}$ es invertible y $[T^{-1}]_{\beta} = [T]_{\beta}^{-1}$
****
**Demostración.**

(1) [[D-La matriz asociada a la composición de dos transformaciones lineales respecto a una única base equivale al producto de las matrices de cada transformación]]

(2) Si $\beta = \{v_1, \dots, v_n\}$ base de $V \Rightarrow \text{Id}(v_j) = v_j = 0v_1 + \dots + 0v_n \Rightarrow [\text{Id}]_{\beta} = \begin{pmatrix} 1 & 0 & \dots & 0 \\ 0 & 1 & \dots & 0 \\ \vdots & \vdots & \ddots & \vdots \\ 0 & 0 & \dots & 1 \end{pmatrix} = \text{matriz identidad}$

(3) Si $T$ es invertible (es **isomorfismo**) $\Rightarrow \exists T^{-1}: V \to V$ lineal y satisface
$T^{-1} \circ T = \text{Id}$
$T \circ T^{-1} = \text{Id}$ (tomando matrices respecto de la base $\beta$)

$\text{Id} = [\text{Id}]_{\beta} = [T^{-1} \circ T]_{\beta} = [T^{-1}]_{\beta} [T]_{\beta}$

Del mismo modo
$\text{Id} = [\text{Id}]_{\beta} = [T \circ T^{-1}]_{\beta} = [T]_{\beta} [T^{-1}]_{\beta}$

$\Rightarrow [T^{-1}]_{\beta} \text{ es la inversa de } [T]_{\beta} \Rightarrow [T^{-1}]_{\beta} = ([T]_{\beta})^{-1}$
****
A partir de esta última proposición, podemos usar la matriz inversa para calcular la preimagen de un vector. 
