# Ingeniería de Software 1 - Practica 5: Redes de Petri (RP)

Resolución de ejercicios de la práctica de Redes de Petri y también ejercicios de parcial de este tema.

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

* ***Enunciado2***

***Se desea modelar con Redes de Petri un semáforo inteligente en un cruce peatonal. El semáforo
puede detectar cuando llegan vehiculos (por la calle) y cuando llegan peatones (por la vereda) al
cruce. El objetivo del semáforo es dejar pasar sólo un tipo de entidad a la vez, pero de a grupos.
Para habilitar el cruce de vehículos deben llegar como mínimo cuatro vehículos al semáforo. En este
caso, si no hay peatones cruzando, se habilita hasta que pasen los cuatro vehiculos. Para que crucen
los peatones se debe cumplir la misma regla, pero alcanza con que haya dos peatones en el cruce. Nunca
pueden cruzar peatones si hay vehículos cruzando, ni viceversa.***

* ***Enunciado3***

***Se desea modelar con Redes de Petri un semáforo inteligente en un cruce peatonal. El semáforo debe
dejar pasar autos o peatones al llegar al cruce. Para que los autos puedan pasar, deben juntarse 3
autos en un grupo, para pasar todo el grupo al mismo tiempo. Para los peatones debe funcionar igual,
pero esperando sólo 2 peatones. Por último, el semáforo debe dar paso siempre alternadamente, primero
un grupo de vehículos, luego un grupo de peatones, y así sucesivamente. Luego de pasar el cruce, las
entidades se retiran de forma individual.***

* ***Enunciado4***

***Se desea modelar con Redes de Petri el funcionamiento de una linea automática de empaquetado, en
una fábrica de alfajores. Existen dos cintas transportadoras por las que llegan dos tipos de alfajores:
por una llegan alfajores de chocolate y por otra de fruta.***

***En la linea de empaquetado existen dos máquinas que trabajan al mismo tiempo del siguiente modo:
al tener 3 alfajores de chocolate y 3 de fruta se activan las dos máquinas, una confecciona la caja
mientras que la otra envuelve los alfajores. Ambas máquinas funcionan en paralelo y no se puede
comenzar una nueva caja hasta que terminen de trabajar ambas máquinas.***

***Una vez terminada, la caja es depositada en otra cinta, donde una máquina las empaqueta en grupos
de a 6. Luego, el pack de 6 cajas es depositado en un depósito para posterior despacho.***

* ***Enunciado5***

***Modelar con una red de Petri el modo de trabajo que posee una fábrica de bicicletas. A la fábrica
llegan cajas cerradas con los componentes para armar bicicletas de distintos proveedores. La fábrica
sólo funciona por pedidos. Existe un encargado de tomar el pedido y administrar las cajas con los
componentes de las bicicletas. Su tarea es tomar el pedido y una caja, y delegar el trabajo a dos
armadores, dejando cada caja con el número de pedido en el área de armado. Uno de los armadores se
encarga de armar las ruedas y el otro se encarga de armar el cuerpo con el resto de los componentes de
la bicicleta. Los dos armadores trabajan en forma paralela. Una vez que los dos armadores hayan
terminado sus respectivos trabajos, el cuerpo y las ruedas pasan al área de ensamblado, donde el
ensamblador se encarga de finalizar la bicicleta. Los dos armadores sólo comienzan una nueva
bicicleta cuando ambos hayan terminado la que están haciendo. Una vez finalizada la bicicleta,
se coloca en el contenedor de despacho. La bicicleta queda lista para su distribución. Tenga en
cuenta que cada empleado sólo realiza de una tarea por vez.***

* ***Enunciado6***

***Modelar con una red de Petri el sector de revisión de una fábrica de motocicletas. Al sector
llegan elementos de dos tipos: cuadros y motores. Cada elemento llega desde un sector distinto y
pasa directamente a su correspondiente línea de inspección. Existe un grupo de 5 empleados que 
pueden verificar tanto cuadros como motores del siguiente modo:***

***En la línea de inspección de cuadros se verifican que las soldaduras sean correctas. Para esto es
necesario un empleado que inspeccionará de a un cuadro por vez. Puede haber como máximo 2 empleados 
revisando cuadros.***

***En la línea de inspección de motores se verifica que encienda correctamente. Para esto es necesario
que dos empleados trabajen simultáneamente. Puede haber como máximo 4 empleados revisando motores a 
la vez.***

***Luego de las verificaciones se envían los elementos a la espera del embalaje. En la sección de 
embalaje debe esperarse a que lleguen un cuadro y un motor para ser embalados juntos con un sello 
de revisión. Luego la caja revisada es derivada al depósito.***

<br>
<br>
<br>

<p><img align="center" src="https://github.com/Marimari2342/Marimari2342/blob/main/firmagith.png" alt="marigit"/></p>