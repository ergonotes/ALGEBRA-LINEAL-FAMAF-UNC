Siguiendo con la matriz definida en el ejemplo [[E-Matriz Traspuesta]]. 
Teníamos la siguiente matriz que la redefiniremos como $B$ : $$ A^T = \begin{pmatrix} 3 & 2-4i \\ 2+4i & 5 \end{pmatrix} =B$$Y encontraremos su conjugada $\overline{B}$ aplicando la conjugación (le cambiamos el signo a todas las partes imaginarias):
* El 3 y el 5 se quedan exactamente igual (como no tienen $i$, el cambio de signo no les afecta).
* El $2 - 4i$ (arriba a la derecha) vuelve a ser $2 + 4i$.
* El $2 + 4i$ (abajo a la izquierda) vuelve a ser $2 - 4i$.
Finalmente:$$ \overline{B} = \begin{pmatrix} 3 & 2+4i \\ 2-4i & 5 \end{pmatrix} $$
##### **Algo a notar...**
Vemos, revisando el ejemplo citado arriba, que $\overline{B}=A$. Este ejemplo es oportuno para mostrar además, el concepto de **matriz hermítica**, que son aquellas matrices que cumplen $A=A^*$, siendo $A^*$ la matriz resultado de aplicar la operación de **trasponer** y **conjugar** a $A$.  