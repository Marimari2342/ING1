# Ingeniería de Software 1 - Practica 5: Redes de Petri (RP)

En esta carpeta se encuentra la resolución de ejercicios de la práctica de Redes de Petri y también ejercicios de parcial de este tema.

## Enunciados de examen

* ***Enunciado1 (1ra Fecha 2024)***

***Modele con una red de Petri el funcionamiento de una linea de producción de motocicletas. Existen 
tres tipos de componentes que ingresan a la linea de produccion por diferentes carriles. En el primer
carril ingresan motores, en el segundo carril ingresan cuadros y en el tercer carril ingresan ruedas.***

***Todos los componentes son revisados. En el carril de motores existen 2 puestos de revisión y 2 
operarios. Cada operario puede trabajar en cualquiera de los dos puestos y revisa de a un motor por 
vez cada uno. No es posible que haya 2 operarios revisando motores en el mismo puesto.***

***En el caso de los cuadros, también existen dos puestos de trabajos pero en cada puesto hay un 
operario que siempre trabaja en el mismo puesto y que revisa de a un cuadro por vez.***

***En el caso de las ruedas, existe un puesto automático que permite la evaluación de tres ruedas por 
vez como máximo. Una vez revisados los componentes se procede al armado de las motos. Para poder 
armar una moto, es necesario un motor, un cuadro y dos ruedas. Una vez armadas las motos son 
agrupadas para subir al camión. Se arman lotes de 5 motos y se suben al camión cada lote.***

<details><summary><code>Respuesta 🖱</code></summary><br>

![foto](/practica05RP/examen01RP.jpg)

--------------------------------

</details>


* ***Enunciado2***

***Se desea modelar con Redes de Petri un semáforo inteligente en un cruce peatonal. El semáforo
puede detectar cuando llegan vehiculos (por la calle) y cuando llegan peatones (por la vereda) al
cruce. El objetivo del semáforo es dejar pasar sólo un tipo de entidad a la vez, pero de a grupos.
Para habilitar el cruce de vehículos deben llegar como mínimo cuatro vehículos al semáforo. En este
caso, si no hay peatones cruzando, se habilita hasta que pasen los cuatro vehiculos. Para que crucen
los peatones se debe cumplir la misma regla, pero alcanza con que haya dos peatones en el cruce. Nunca pueden cruzar peatones si hay vehículos cruzando, ni viceversa.***

<details><summary><code>Respuesta 🖱</code></summary><br>

![foto](/practica05RP/examen02RP.jpg)

El enunciado no indica alternancia entre el cruce de peatones y vehículos, así que lo supongo así.

--------------------------------

</details>

* ***Enunciado3***

***Se desea modelar con Redes de Petri un semáforo inteligente en un cruce peatonal. El semáforo debe
dejar pasar autos o peatones al llegar al cruce. Para que los autos puedan pasar, deben juntarse 3
autos en un grupo, para pasar todo el grupo al mismo tiempo. Para los peatones debe funcionar igual,
pero esperando sólo 2 peatones. Por último, el semáforo debe dar paso siempre alternadamente, primero
un grupo de vehículos, luego un grupo de peatones, y así sucesivamente. Luego de pasar el cruce, las
entidades se retiran de forma individual.***

<details><summary><code>Respuesta 🖱</code></summary><br>

![foto](/practica05RP/examen03RP.jpg)

En este caso, el enunciado SI indica alternancia entre el cruce de peatones y vehículos, por eso el gráfico queda distinto.

--------------------------------

</details>

* ***Enunciado4***

***Se desea modelar con Redes de Petri el funcionamiento de una linea automática de empaquetado, en
una fábrica de alfajores. Existen dos cintas transportadoras por las que llegan dos tipos de alfajores: por una llegan alfajores de chocolate y por otra de fruta.***

***En la linea de empaquetado existen dos máquinas que trabajan al mismo tiempo del siguiente modo:
al tener 3 alfajores de chocolate y 3 de fruta se activan las dos máquinas, una confecciona la caja
mientras que la otra envuelve los alfajores. Ambas máquinas funcionan en paralelo y no se puede
comenzar una nueva caja hasta que terminen de trabajar ambas máquinas.***

***Una vez terminada, la caja es depositada en otra cinta, donde una máquina las empaqueta en grupos
de a 6. Luego, el pack de 6 cajas es depositado en un depósito para posterior despacho.***

<details><summary><code>Respuesta 🖱</code></summary><br>

![foto](/practica05RP/examen04RP.jpg)

--------------------------------

</details>

* ***Enunciado5***

***Modelar con una red de Petri el modo de trabajo que posee una fábrica de bicicletas. A la fábrica
llegan cajas cerradas con los componentes para armar bicicletas de distintos proveedores. La fábrica
sólo funciona por pedidos. Existe un encargado de tomar el pedido y administrar las cajas con los
componentes de las bicicletas. Su tarea es tomar el pedido y una caja, y delegar el trabajo a dos
armadores, dejando cada caja con el número de pedido en el área de armado. Uno de los armadores se
encarga de armar las ruedas y el otro se encarga de armar el cuerpo con el resto de los componentes de la bicicleta. Los dos armadores trabajan en forma paralela. Una vez que los dos armadores hayan
terminado sus respectivos trabajos, el cuerpo y las ruedas pasan al área de ensamblado, donde el
ensamblador se encarga de finalizar la bicicleta. Los dos armadores sólo comienzan una nueva
bicicleta cuando ambos hayan terminado la que están haciendo. Una vez finalizada la bicicleta,
se coloca en el contenedor de despacho. La bicicleta queda lista para su distribución. Tenga en
cuenta que cada empleado sólo realiza de una tarea por vez.***

<details><summary><code>Respuesta 🖱</code></summary><br>

![foto](/practica05RP/examen05RP.jpg)

El enunciado no me dice que cada armador se dedica específicamente a una tarea (es decir pueden turnarse y a veces armar el cuerpo y otras veces las ruedas). Como interpreto eso lo hago así, sino modelaría cada armador por separado y el área de armado para indicar que trabajan en paralelo...

--------------------------------

</details>

* ***Enunciado6***

***Modelar con una red de Petri el sector de revisión de una fábrica de motocicletas. Al sector
llegan elementos de dos tipos: cuadros y motores. Cada elemento llega desde un sector distinto y
pasa directamente a su correspondiente línea de inspección. Existe un grupo de 5 empleados que 
pueden verificar tanto cuadros como motores del siguiente modo:***

***En la línea de inspección de cuadros se verifican que las soldaduras sean correctas. Para esto es
necesario un empleado que inspeccionará de a un cuadro por vez. Puede haber como máximo 2 empleados 
revisando cuadros.***

***En la línea de inspección de motores se verifica que encienda correctamente. Para esto es necesario que dos empleados trabajen simultáneamente. Puede haber como máximo 4 empleados revisando motores a la vez.***

***Luego de las verificaciones se envían los elementos a la espera del embalaje. En la sección de 
embalaje debe esperarse a que lleguen un cuadro y un motor para ser embalados juntos con un sello 
de revisión. Luego la caja revisada es derivada al depósito.***

<details><summary><code>Respuesta 🖱</code></summary><br>

![foto](/practica05RP/examen06RP.jpg)

--------------------------------

</details>

* ***Enunciado7***

***Se desea modelar el funcionamiento de una central de telefonía IP con una red de Petri. A la central llegan llamados los cuales se encolan para ser atendidos. La central cuenta con 5 líneas las cuales pueden trabajan de manera simultánea pero cada línea puede atender de a un llamado a la vez. Luego que la central atiende un llamado los mismos son derivados a cualquiera de las 2 operadoras. La primera operadora puede atender como máximo 2 llamados a la vez. La segunda operadora también puede atender como máximo 2 llamado en simultaneo, pero debe esperar a que lleguen 2 llamados para empezar a atender (hasta que no termina de atender los 2 llamados no puede atender otra tanda). Luego que los llamados pasan por la operadora son derivados al interno finalizando el trabajo de la central.***

<details><summary><code>Respuesta 🖱</code></summary><br>

![foto](/practica05RP/examen07RP.jpg)

--------------------------------

</details>

* ***Enunciado8***

***Se desea modelar a través de una red de Petri una línea de producción de quesos. A la línea ingresan diferentes recipientes de leche. Cada recipiente deberá ser controlado en cualquiera de los cuatro puestos. En cada puesto hay un operario el cual puede controlar de a un recipiente por vez. Luego de controlados los recipientes pasan a una cola común antes de la pasteurización de la leche. Para dicha tarea existe un operario que puede pasteurizar un recipiente cada vez. Luego de dicho proceso, se necesitan 5 recipientes de leche para la realización de 1 queso. Una vez realizado el queso es despachado.***

* ***Enunciado9***

***Se desea modelar con una red de Petri el funcionamiento de una plaqueta eléctrica. A la red llegan pulsos de tensión. Cada pulso de tensión es derivado a alguno de los dos canales posibles. Si es derivado al canal A, un pulso de tensión se convierte en 3 pulsos, los cuales son encolados para que el sistema verifique si cada uno de estos tres pulsos generados tienen el voltaje adecuado. El sistema verifica de a un pulso a la vez y si el pulso tiene el voltaje esperado es enviado al procesador y consumido.***

***Los pulsos que se envíen al canal B, deberán esperar la llegada de 4 pulsos para ser verificados. Una vez que llegan los 4 pulsos para ser verificados, el sistema verifica su voltaje. En el canal B, el sistema puede verificar de a 2 pulsos a la vez y si los pulsos tienen el voltaje esperado son enviados al procesador y consumidos.***

* ***Enunciado10***

***Se desea modelar la primera etapa de una línea de fabricación de galletitas veganas. A la línea de producción entran, continuamente, por 3 secciones separadas los ingredientes para generar la masa (agua, harina y componentes de la fórmula del sabor). Luego, los ingredientes ingresan en una máquina que los mezcla y separa en 4 bollos. Esta máquina no puede procesar nuevos ingredientes hasta finalizar con los actuales.***

***En la siguiente etapa los bollos pueden pasar a cualquiera de las 2 máquinas para ser aplanados y cortados simultáneamente en 6 galletitas mediante una plantilla con forma de estrellas. Los recortes sobrantes son enviados a la sección de descarte donde finalmente se almacenan para ser reciclados.
Las galletitas ya cortadas pasan a una cinta transportadora común para ser enviadas a la sección de cocción que forma parte de una segunda etapa.***

* ***Enunciado11***

***Modelar el funcionamiento de una línea de llenado y empaque de desodorantes. Los envases vacíos de desodorantes ingresan a la línea principal donde deben esperar para su llenado. A partir de este punto cada envase pasa a una de las 2 líneas de llenado. Para distribuir equitativamente la carga de trabajo, los envases son desviados alternadamente a cada línea. Una vez llenados pasan a la etapa de empaque dentro de cada línea donde se recubren con un plástico retráctil que agrupa de a 6 envases.***

***En la siguiente etapa, las 2 líneas convergen en la sección de empaque general donde se colocan en cajas de cartón que agrupan 4 empaques (24 desodorantes). Finalmente, las cajas se envían a la sección de transporte para ser almacenadas.***

* ***Enunciado12***

***Se desea modelar el funcionamiento de una barcaza que transporta vehículos. La barcaza hace primero un recorrido del lado "A al lado "B" del río y luego el recorrido del lado "B" al lado "A", siempre cargando 3 vehículos.***

***Cuando los vehículos llegan esperan a que la barcaza esté del lado correspondiente del río. Cuando esto sucede, se cargan 3 vehículos de forma simultánea a la barcaza. Una vez cargados, se realiza el viaje al otro lado del río. Finalizado el recorrido, los autos bajan juntos y la barcaza queda disponible para repetir el proceso con los vehículos de ese lado.***

* ***Enunciado13***

***Se desea simular el funcionamiento de un circuito de carreras a pie. La carrera consta de 3 etapas y se corre en parejas de 2 equipos diferentes. Los corredores de cada equipo llegan a su fila de salida y esperan a que haya un oponente del otro equipo en la línea de partida. Cuando hay 1 corredor de cada equipo listo, inician la carrera y pasan por la etapa 1.***

***En la etapa 2 hay dos circuitos independientes A y B. El primer corredor en llegar pasa por el circuito A directamente. El segundo corredor en llegar pasa por el circuito B con una penalización. El circuito B tiene la particularidad de que un corredor no puede terminarlo hasta que llegue un segundo corredor de la siguiente pareja. Cuando esto sucede, los 2 corredores del circuito B continúan por la siguiente etapa. Finalmente, los corredores pasan por la etapa 3 y terminan la carrera.***

* ***Enunciado14***

***Se desea modelar a través de una red de petri una línea de producción de quesos. A la línea ingresan diferentes recipientes de leche. Cada recipiente deberá ser controlado en cualquiera de los dos puestos existentes. Para controlar los recipientes existe alternando el control en cada puesto de un único inspector que puede controlar de a un recipiente por vez y que deberá trabajo, comenzando en el puesto 1, luego controlando en el puesto 2, luego en el 1 y así siguiendo.***

***Luego de controlados los recipientes pasan a una cola común antes de la pasteurización de la leche. Para dicha tarea existen dos operarios que pueden pasteurizar un recipiente cada vez. Cada operario tiene un puesto de trabajo diferente. Luego de la pasteurización, la leche está lista para la realización del queso. Es necesario juntar 2 recipientes pasteurizados para el armado de un queso. Luego los quesos son despachados.***

<br>
<br>
<br>

<p><img align="center" src="https://github.com/Marimari2342/Marimari2342/blob/main/firmagith.png" alt="marigit"/></p>