# Ingeniería de Software 1 - Practica 4: Diagramas de Transición de Estados (DTE)

## 🟠 Ejercicio 1. 

Dado el siguiente diagrama que representa el funcionamiento de una Licuadora, corrija los errores existentes. La licuadora tiene 2 velocidades y sólo dos botones: uno para aumentar la velocidad y otro para disminuirla. La licuadora se apaga con el botón disminuir estando en la primera velocidad.

![foto](/cosas/foto01.png)

<details><summary><code>Respuesta 🖱</code></summary><br>

![foto](/practica04DTE/DTEpunto01.jpg)

--------------------------------

</details>

## 🟠 Ejercicio 2. Complete el siguiente diagrama DTE que ilustra el comportamiento de una máquina de gaseosas, en base al siguiente enunciado:

La máquina se activa cuando el usuario ingresa una moneda. Todos los productos tienen el mismo valor. Las monedas son ingresadas de a una y cada una es validada en ese mismo momento, en base a su tamaño, peso y espesor mediante un dispositivo específico. Al mismo tiempo se valida el monto ingresado. Si alguna moneda no es válida, se retorna al usuario, y continúa el proceso normalmente. Como siguiente paso, el usuario debe seleccionar un producto. Si no hay stock de dicho producto entonces debe retornar las monedas y mostrar un mensaje informando tal situación. Si hay stock, se entrega el producto, y en caso de que se haya ingresado un monto superior, la máquina retorna el vuelto correspondiente. El usuario puede cancelar en cualquier momento, dando por finalizado todo el proceso.

![foto](/cosas/foto02.png)

<details><summary><code>Respuesta 🖱</code></summary><br>

![foto](/practica04DTE/DTEpunto02.jpg)

--------------------------------

</details>

## 🟠 Ejercicio 3. 

Se desea modelar con un DTE el acceso a una caja fuerte, la cual posee un código de seguridad con una longitud desconocida. La caja presenta un teclado numérico y un botón “aceptar”. Si el código es incorrecto el sistema debe terminar indicando un error. Analice las siguientes soluciones y discuta las diferencias.

![foto](/cosas/foto03.png)

<details><summary><code>Respuesta 🖱</code></summary><br>

La diferencia entre ambos diagramas está en que el primero considera la validación de un número como un estado, y de ahí se desprenden los dos posibles estados finales (que termine la validación y esta sea correcta, o que termine la validación y sea incorrecta); mientras que en la solución dos directamente cuando se presiona el botón </aceptar/> se pasa a los dos posibles estados finales y la validación del número no es un estado.

Yo creo que ambas soluciones son correctas, pero la primera es más prolija pues un estado identifica un período de tiempo y la validación del código no es automática, sino que abarca un periodo de tiempo hasta que se valida.

--------------------------------

</details>

## 🟠 Ejercicio 4. Realizar el DTE para modelar un turbo ventilador.

Considere un sistema de control de un turbo ventilador que posee tres niveles de velocidad. Para ir de un nivel a otro, ya sea anterior o posterior, se debe girar una perilla en forma secuencial. Inicialmente el ventilador se encuentra apagado. Girando la perilla en el sentido de las agujas del reloj se enciende y se aumenta la velocidad, mientras que girando la perilla en el sentido contrario se disminuye. El ventilador puede ser apagado girando hacia la izquierda en el nivel 1 o hacia la derecha en el nivel 3.

<details><summary><code>Respuesta 🖱</code></summary><br>

![foto](/practica04DTE/DTEpunto04.jpg)

--------------------------------

</details>

## 🟠 Ejercicio 5. Modelar mediante un DTE el ingreso del personal a una empresa.

Para ello existe una máquina en donde un empleado debe registrar el presente. Para iniciar el registro se selecciona la opción “Registrar Asistencia”. Luego, se habilitan dos opciones posibles para registrar su presente: mediante su tarjeta o su huella dactilar.

Si el empleado selecciona “registro por tarjeta”, debe pasar la tarjeta por un lector. Si la tarjeta es válida se habilita un teclado virtual donde debe proceder a ingresar un código de 4 dígitos, en el caso de que la tarjeta fuese inválida se informa el error. Para el ingreso de los 4 dígitos se tienen sólo 3 intentos, pasados los 3 intentos se anula la operación y se retorna la tarjeta.

Si opta por registrar el presente mediante la huella dactilar sólo debe apoyar el dedo en el scanner. 

En cualquiera de los 2 casos si el ingreso es exitoso se muestra en el display la fecha y el horario de entrada y un mensaje de éxito, caso contrario, se visualiza un mensaje de error y se emite un pitido.

<details><summary><code>Respuesta 🖱</code></summary><br>

--------------------------------

</details>