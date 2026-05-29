# ERGO | Wikipedia Colaborativa
![Logo](docs/assets/logo.png)

ERGO es una plataforma de notas y apuntes colaborativos para estudiantes STEM. El objetivo es centralizar el conocimiento de una clase en particular, facilitar el acceso a material de estudio gratuito y fomentar la colaboración entre estudiantes. Para FAMAF y quién sabe dónde más.
****
## **Características Principales**
* **Contenido Curado:** Sección "Oficial" con material revisado por administradores.
* **Comunidad Abierta:** Cualquier estudiante puede subir sus propios apuntes o ejercicios resueltos.
* **Editor Web Integrado:** No necesitás saber Git para colaborar. Podés usar nuestro panel de **Decap CMS** para escribir desde el navegador.
* **Soporte LaTeX:** Renderizado impecable de fórmulas matemáticas mediante KaTeX/MathJax.
* **Feedback Directo:** Comentarios en cada página para correcciones o sugerencias.
---
### Para usuarios
Podés acceder a la versión publicada del sitio aquí:  

👉 **[{{ config.site_url }}]({{ config.site_url }})**
### Para colaboradores
¿Querés sumar tu apunte?
> 💡 Consultá la **[Guía de Contribución](docs/contribution-guide.md)** para conocer los detalles técnicos (uso de carpetas, previsualización de fórmulas, etc).

---
## **Estructura del Proyecto**
* `docs/oficial/`: Contenido validado y estructurado por unidades.
* `docs/comunidad/`: Apuntes libres, resúmenes y ejercicios. También pudiendo seguir una estructura.
* `docs/(comunidad u oficial)/assets`: Imágenes, capturas de pantalla y contenido en notas.
* `hooks.py`: Lógica de procesamiento de Markdown y configuración dinámica del CMS.

---
## **Licenciamiento (Híbrido)**

Este proyecto protege tanto la libertad del código como la autoría del contenido:
1.  **Código Fuente:** Licenciado bajo **[GNU AGPLv3](LICENSE)**. Si usás o mejorás esta infraestructura para tu propio sitio, estás obligado a mantenerlo abierto.
2.  **Contenido (Apuntes):** Todo el material de estudio se distribuye bajo **[CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)** (Atribución - No Comercial - Compartir Igual).
---
## **Apoyo y Mejoras**
Este sitio se mantiene gracias al esfuerzo del desarrollador. Si te sirve el material, podés ayudar de varias formas:
* **Desarrollo:** Reportando bugs o mejorando cualquier aspecto del código actual, o del que se está desarrollando para la próxima versión.
* **Contenido:** Corrigiendo errores de tipeo en las fórmulas o subiendo nuevos finales resueltos.
* **Sustento:** Cualquier ayuda para mantener la infraestructura y el dominio es bienvenida.
---
*Creado por [Tomás](https://github.com/tomasccc).*
