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

![foto](/practica04DTE/DTEpunto05.jpg)

--------------------------------

</details>

## 🟠 Ejercicio 6. Se desea modelar el funcionamiento de un personaje para un juego electrónico.

El personaje es un guardia medieval de un castillo. Su objetivo es vigilar el castillo y eliminar enemigos que puedan aparecer. El personaje comienza su ronda de vigilancia cuando es creado por el sistema, con el 100% de energía. El modo normal del personaje es vigilar el castillo, mientras no detecte un enemigo. Al detectar uno, el personaje pasa a modo combate. Si el enemigo está fuera del castillo, el personaje saca su arco y flecha. Si el enemigo está dentro del castillo, el personaje saca su espada. Durante el combate, el personaje puede recibir “golpes”, reduciendo su energía 10% por cada uno. Si el personaje gana el combate, recupera el 50% de energía y vuelve con su ronda de vigilancia. Pero si pierde energía hasta quedarse con el 20%, entonces el personaje comienza a huir del enemigo, guardando su arma. Durante la huida el personaje puede seguir recibiendo “golpes”, hasta quedarse sin energía y morir, quedando fuera del juego. Cuando pierde de vista al enemigo, el personaje deja de huir y vuelve con su ronda de vigilancia, ganando un 30% de energía.

<details><summary><code>Respuesta 🖱</code></summary><br>

![foto](/practica04DTE/DTEpunto06.jpg)

--------------------------------

</details>

## 🟠 Ejercicio 7. Modelar mediante un DTE el sistema de voto electrónico para la facultad de informática.

El sistema cuenta con 2 terminales: la mesa de autoridades y la urna electrónica. Cuando un alumno se presenta a votar, le entrega la documentación a la autoridad de la mesa y el encargado del manejo del sistema selecciona la opción ‘Nuevo Votante’. No todos los alumnos tienen su huella dactilar registrada por lo que el sistema presenta 2 opciones: identificación por huella e identificación por número de alumno.

En el caso de que se seleccione la opción identificación por huella se procede a la lectura de la huella del alumno. Si la huella no es identificada por el sistema se cancela la operación. Si la huella es detectada correctamente y el alumno no votó se habilita la urna electrónica que es donde el alumno emite su voto.

En el caso de que se seleccione identificación por número de alumno, el sistema solicita que se ingrese el legajo y luego se continúa con el mismo procedimiento de emisión de voto. Si el legajo no es reconocido por el sistema es informado y se cancela la operación. Para ambos casos, una vez identificado el alumno, si el mismo ya emitió su voto el sistema muestra un mensaje y cancela la operación.

Una vez iniciada la votación, se habilita la pantalla y se muestran las opciones para elegir el tipo de votación: “boleta completa” o “cortar boleta”. Si pasan 30 segundos y el votante no ha decidido su tipo de votación, la maquina emitirá un cartel de alerta donde indica que debe realizar la elección correspondiente, el cartel se mantendrá en pantalla hasta que el votante decida su tipo de votación. 

Una vez elegido el tipo de votación, se pasará a elegir la agrupación a votar, para ello la máquina oculta las opciones anteriores y muestra un listado de los partidos disponibles. Si se eligió cortar boleta, el votante deberá elegir dos agrupaciones, caso contrario, elige solo una agrupación.
Una vez emitido el voto, es decir, que seleccionó la/s agrupación/es correspondiente/s, se oculta el listado, se muestra en toda la pantalla la opción/es elegida/s, se muestra un botón para confirmar y se muestra otro botón para cancelar. Si confirma el voto, el mismo se envía a imprimir, se muestra un mensaje éxito, envía un mensaje a la mesa de autoridades y finaliza la sesión. Si cancela se muestra un mensaje de cancelación y finaliza la sesión.

<details><summary><code>Respuesta 🖱</code></summary><br>

![foto](/practica04DTE/DTEpunto07.jpg)

--------------------------------

</details>

## 🟠 Ejercicio 8. Modelar mediante DTE la búsqueda de un destino para navegación por GPS.

Al seleccionar la opción “ir a destino” el sistema visualiza la “pantalla inicial de búsqueda” con las opciones: “últimos encontrados” y “nuevo destino”. Si el usuario selecciona “últimos encontrados” se muestra una lista con los últimos 5 lugares buscados. Luego, el usuario debe seleccionar un lugar de dicha lista para iniciar la navegación. Si el usuario selecciona “nuevo destino” el sistema visualiza un campo para completar la calle del destino, compuesta por caracteres alfanuméricos, y un botón “siguiente”. Una vez completo el ingreso de la calle y presionado “siguiente” el sistema muestra el campo altura, compuesto por caracteres numéricos, y un botón “confirmar”. Al confirmar el GPS busca la dirección ingresada, si se encuentra dicha dirección se inicia la navegación. Si la dirección no es encontrada por el sistema se informa el error y se retorna a la pantalla de búsqueda.

Para ambos casos, se muestra el mapa de ruta correspondiente y las opciones “Ir” y “Cancelar”. Si se selecciona “Ir”, el GPS comienza con la navegación. Si el usuario cancela se retorna a la “pantalla inicial de búsqueda”. Cuando GPS se encuentra navegando y pierde la señal de satélite entonces se queda a la espera de recepción de señal, cuando logra restablecer la señal continúa con la navegación. Si luego de 3 minutos no logra encontrar señal se cancela automáticamente la navegación y se retorna a la pantalla de búsqueda. Mientras se está navegando el sistema actualiza una vez por segundo la ubicación geográfica, la información de la velocidad, distancia y tiempo restante. Cuando termina la navegación el sistema retorna un mensaje de destino alcanzado. El usuario puede detener la navegación en cualquier momento presionando el botón “detener navegación”, en cuyo caso, el sistema, retorna a la pantalla de inicio con la opción “Ir a destino”.

<details><summary><code>Respuesta 🖱</code></summary><br>

![foto](/practica04DTE/DTEpunto08.jpg)

--------------------------------

</details>

## 🟠 Ejercicio 10. Modelar un sistema para una cinta para correr.

La cinta consta de un display táctil y un botón de encendido/apagado. Cuando se presiona encender, la cinta inicia en un estado de reposo, se habilita el display, se muestra un mensaje de bienvenida, la velocidad de la misma (inicialmente en cero), las opciones “+” y “-“, para aumentar y disminuir dicha velocidad y tres programas predefinidos de entrenamiento (inicial, intermedio y máximo). Una vez encendida la cinta, el usuario debe elegir uno de estos tres programas para comenzar a entrenar. Estando en cualquiera de los tres programas, el usuario, puede cambiar a algún otro programa de entrenamiento, o finalizar el mismo mediante un botón de “fin de programa” volviendo al estado de reposo. Además, puede variar la velocidad del mismo, sin salir del programa en el que se encuentra. La velocidad oscila en un rango de 0 a 9, y aumenta y disminuye en escala de 1. Si la velocidad disminuye a cero, la cinta vuelve al estado de reposo. En cualquier momento se puede apagar la cinta.

<details><summary><code>Respuesta 🖱</code></summary><br>

* Version 1 --> Se repiten muchas transiciones puesto que los estados relacionados a los programas de entrenamiento son muy similares... 

![foto](/practica04DTE/DTEpunto10-version1.jpg)

* Version 2 --> CORREGIDA. Se diagraman los tres programas de entrenamiento en un mismo estado, así el diagrama queda más prolijo y se evita estar repitiendo las transiciones.

![foto](/practica04DTE/DTEpunto10-versioncorregida.jpg)

--------------------------------

</details>