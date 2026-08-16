Esta notación fue un descubrimiento analítico que se gestó durante el siglo XVIII a través del cálculo de series infinitas.

Euler sabía que las funciones exponenciales, senos y cosenos podían escribirse como series infinitas polinómicas:

$$e^x = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + \frac{x^4}{4!} + \frac{x^5}{5!} + \dots$$

$$\cos x = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \dots$$

$$\sin x = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \dots$$

La genialidad de Euler fue evaluar la serie exponencial para un argumento puramente imaginario, sustituyendo $x$ por $i\theta$:

$$e^{i\theta} = 1 + i\theta + \frac{(i\theta)^2}{2!} + \frac{(i\theta)^3}{3!} + \frac{(i\theta)^4}{4!} + \frac{(i\theta)^5}{5!} + \dots$$

Sabiendo que las potencias de $i$ tienen un comportamiento cíclico ($i^2 = -1$, $i^3 = -i$, $i^4 = 1$, etc.), la serie se transforma en:

$$e^{i\theta} = 1 + i\theta - \frac{\theta^2}{2!} - i\frac{\theta^3}{3!} + \frac{\theta^4}{4!} + i\frac{\theta^5}{5!} - \dots$$
Agrupando los términos reales por un lado y los términos imaginarios por otro, Euler obtuvo:

$$e^{i\theta} = \left(1 - \frac{\theta^2}{2!} + \frac{\theta^4}{4!} - \dots\right) + i\left(\theta - \frac{\theta^3}{3!} + \frac{\theta^5}{5!} - \dots\right)$$

Lo que se encuentra exactamente dentro de los paréntesis son las series de Taylor del coseno y el seno. Así nació la **Fórmula de Euler**:
$$e^{i\theta} = \cos \theta + i\sin \theta$$