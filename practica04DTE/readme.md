# Ingeniería de Software 1 - Practica 4: Diagramas de Transición de Estados (DTE)

## 🟠 Punto 3. 

Se desea modelar con un DTE el acceso a una caja fuerte, la cual posee un código de seguridad con una longitud desconocida. La caja presenta un teclado numérico y un botón “aceptar”. Si el código es incorrecto el sistema debe terminar indicando un error. Analice las siguientes soluciones y discuta las diferencias.

![foto](/cosas/foto01.png)

<details><summary><code>Respuesta 🖱</code></summary><br>

La diferencia entre ambos diagramas está en que el primero considera la validación de un número como un estado, y de ahí se desprenden los dos posibles estados finales (que termine la validación y esta sea correcta, o que termine la validación y sea incorrecta); mientras que en la solución dos directamente cuando se presiona el botón </aceptar/> se pasa a los dos posibles estados finales y la validación del número no es un estado.

Yo creo que ambas soluciones son correctas, pero la primera es más prolija pues un estado identifica un período de tiempo y la validación del código no es automática, sino que abarca un periodo de tiempo hasta que se valida.

--------------------------------

</details>