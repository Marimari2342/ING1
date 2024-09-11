# Ingeniería de Software 1 - Practica 1: Técnicas de Elicitación de Requisitos

## 🟡 Obtención de los requerimientos

### Parte I Definiciones.

* ***1) Definir brevemente qué es un requerimiento.***

<details><summary> <code> Respuesta 🖱 </code></summary><br>

Al hablar de las necesidades del cliente en términos más técnicos, hablamos de requerimientos. Un Requerimiento es una característica del sistema o una descripción de algo que el sistema es capaz de hacer con el objeto de satisfacer el propósito del sistema.

La IEEE-Std-610 define a los requerimientos como:

a) Condición o capacidad que necesita el usuario para resolver un problema o alcanzar un objetivo.

b) Condición o capacidad que debe satisfacer o poseer un sistema o una componente de un sistema para satisfacer un contrato, un estándar, una especificación u otro documento formalmente impuesto.

c) Representación documentada de los requerimientos, de una condición o capacidad.

</details>

* ***2) Definir requerimientos funcionales y no funcionales.***

<details><summary><code>Respuesta 🖱</code></summary><br>
  
</details>

* ***3) Definir que es un stakeholder.***

<details><summary> <code> Respuesta 🖱 </code></summary><br>

El término stakeholder se utiliza para referirse a cualquier persona o grupo que se verá afectado por el sistema, directa o indirectamente. Entre los stakeholders se encuentran: los usuarios finales, los ingenieros, gerentes y expertos del dominio.

</details>

* ***4) Definir las fuentes más importantes para la obtención de información.***

<details><summary> <code> Respuesta 🖱 </code></summary><br>

Para obtener la información tenemos distintas fuentes, por un lado: 

a) Métodos discretos

* Muestreo de la documentación, los formularios y los datos existentes.
* Investigación y visitas al lugar.
* Observación del ambiente de trabajo.

b) Métodos interactivos

* Cuestionarios.
* Entrevistas.
* Planeación conjunta de Requerimientos (JRP o JAD).
* Lluvia de Ideas - Brainstorming .

</details>

* ***5) Indicar los puntos de vista (de manera genérica) que se pueden reconocer en un proyecto de software.***

<details><summary> <code> Respuesta 🖱 </code></summary><br>

Existen tres tipos genéricos de puntos de vista:

a) Punto de vista de los interactuadores: representan a las personas u otros sistemas que interactúan directamente con el sistema. Pueden influir en los requerimientos del sistema de algún modo.

b) Punto de vista indirecto: representan a los stakeholders que no utilizan el sistema ellos mismos pero que influyen en los requerimientos de algún modo.

c) Punto de vista del dominio: representan las características y restricciones del dominio que influyen en los requerimientos del sistema.

</details>

* ***6) Enumerar tres problemas de comunicación que pueden existir en la elicitación de requisitos.***

<details><summary> <code> Respuesta 🖱 </code></summary><br>

La elicitación de requisitos es una actividad principalmente de carácter social, mucho más que tecnológico. Por lo tanto, los problemas que se plantean son de naturaleza psicológica y social, más que técnicos. Dentro de estos problemas se encuentran los problemas de comunicación, que son:

* Dificultad para expresar claramente las necesidades.
* No ser conscientes de sus propias necesidades.
* No entender cómo la tecnología puede ayudar.
* Miedo a parecer incompetentes por ignorancia tecnológica.
* No tomar decisiones por no poder prever las  consecuencias, no entender las alternativas o no tener una visión global.
* Cultura y vocabulario diferentes.
* Intereses distintos en el sistema a desarrollar.
* Medios de comunicación inadecuados (diagramas que no entienden los clientes y usuarios).
* Conflictos personales o políticos.

</details>

### Parte II Problemas.

***a) Indicar para cada problema quiénes podrían ser los Stakeholders, los puntos de vista y las fuentes de información.***

* ***1) En un sistema de registro de asistencia a través de técnicas biométricas (huella digital) de estudiantes universitarios para la cátedra de Ingeniería I. Este sistema se alimentará de un listado otorgado por la oficina de alumnos de la facultad. Además, necesita la autorización del Jefe de Trabajos Prácticos del turno correspondiente para luego los alumnos poder registrar el presente. También, el profesor a cargo de la materia podrá consultar y listar el estado de cada alumno perteneciente a su cátedra. El sistema sólo se utilizará en el ámbito de la facultad de Informática y deberá adecuarse a la reglamentación sobre privacidad de los datos en el ámbito de la misma.***

<details><summary><code>Respuesta 🖱</code></summary><br>

**Stakeholders**

<p>(a) Oficina de alumnos de la facultad: proporciona el listado de estudiantes que serán registrados en el sistema.</p>
<p>(b) Jefe de Trabajos Prácticos: es el que autoriza el uso del sistema para que cada alumno pueda dar el presente en su turno.</p>
<p>(c) Profesor de la materia: puede consultar y listar el listado de cada uno de sus alumnos en el sistema.</p>
<p>(d) Estudiantes Universitarios: registran su asistencia en el sistema.</p>
<p>(e) Autoridades de la Facultad de Informática: son los que se aseguran que el sistema cumpla con la reglamentación sobre privacidad.</p>
<p>(f) Especialistas en seguridad de datos: asesoran sobre la adecuación del sistema con la reglamentación de privacidad de datos.</p>

**Puntos de vista**

<p>(a) Oficina de Alumnos de la Facultad: necesitan asegurarse de que el sistema pueda integrarse con el listado de estudiantes y que los datos sean precisos y actualizados.</p>
<p>(b) Jefe de Trabajos Prácticos: Requiere que el sistema sea accesible y funcional para la autorización de la asistencia. Debe ser capaz de manejar el registro de asistencia de manera eficiente y acorde con los horarios de los turnos.</p>
<p>(c) Profesor de la Materia: necesita acceso a informes y listados claros sobre la asistencia de los estudiantes para la gestión de su cátedra y la toma de decisiones relacionadas con el rendimiento académico.</p>
<p>(d) Estudiantes Universitarios: quieren un sistema que sea fácil de usar y que garantice que su asistencia se registre correctamente.</p>
<p>(e) Autoridades de la Facultad de Informática: se preocupan por el cumplimiento de las leyes y regulaciones, y la protección de la privacidad y seguridad de los datos personales de los estudiantes.</p>
<p>(f) Especialistas en seguridad de Datos: deben asegurar que el sistema cumpla con las regulaciones sobre la protección de datos personales y privacidad, y que no haya brechas en la seguridad de los datos.</p>

**Fuentes de Información**

<p>(a) Oficina de Alumnos de la Facultad: Listado de estudiantes, datos y registros de los mismos.</p>
<p>(b) Jefe de Trabajos Prácticos: procedimientos para la autorización de la asistencia y requisitos específicos del turno.</p>
<p>(c) Profesor de la Materia: requisitos de la cátedra, informes de asistencia y necesidades de gestión de la clase.</p>
<p>(d) Estudiantes Universitarios: información sobre el uso del sistema.</p>
<p>(e) Autoridades de la Facultad de Informática: políticas y reglamentaciones sobre privacidad y protección de datos, y requisitos legales aplicables.</p>
<p>(f) Especialistas en seguridad de Datos: normativas de privacidad de datos, buenas prácticas en seguridad de datos.</p>

</details>

***b) Habiendo resuelto los problemas presentados, ¿por qué considera que los requerimientos de los distintos stakeholders podrían entrar en conflicto?***

<details><summary><code>Respuesta 🖱</code></summary><br>

<p>Los requerimientos de los distintos stakeholders pueden entrar en conflicto debido a la variedad de intereses, objetivos y limitaciones de cada grupo. Estos conflictos pueden surgir debido a la combinación de diferentes prioridades y restricciones, como la eficiencia operativa, la precisión de los datos, la facilidad de uso, el cumplimiento de las normativas legales y los recursos disponibles. La clave para resolver estos conflictos es encontrar un equilibrio que satisfaga las necesidades de todos los stakeholders, mediante un enfoque colaborativo y una comunicación clara entre todos los involucrados.</p> 
<p>Por ejemplo: los estudiantes necesitan un sistema que sea fácil de usar y que registre su asistencia de manera precisa; mientras que las autoridades de la Facultad deben cumplir con las regulaciones de privacidad y protección de datos, lo que puede requerir medidas adicionales de seguridad y restricciones en el acceso a los datos. Esto podría generar un posible conflicto debido a que los requisitos de privacidad y seguridad pueden llevar a restricciones en el acceso y la gestión de datos, lo que podría complicar el proceso para los estudiantes que simplemente quieren registrar su asistencia sin complicaciones.</p> 

</details>

## 🟡 Entrevistas

### Parte I Definiciones.

* ***1. Describir qué tipo de información puede obtenerse en una entrevista.***

<details><summary><code>Respuesta 🖱</code></summary><br>

<p>La entrevista es una técnica de exploración mediante la cual el analista de sistemas recolecta información de las personas a través de la interacción cara a cara. Es una conversación con un propósito específico, que se basa en un formato de preguntas y respuestas en general, con el propósito de conocer opiniones y sentimientos del entrevistado.</p>
<p>Mediante las entrevistas pueden obtenerse tipos de información tales como opiniones, objetivos, procedimientos informales y sentimientos del entrevistado.</p>

</details>

* ***2. Enumerar y describir brevemente las etapas de la preparación de una entrevista.***

<details><summary><code>Respuesta 🖱</code></summary><br>

(a) Seleccionar los entrevistados: se debe minimizar el número de entrevistas, y los entrevistados deben conocer con antelación el objetivo de la entrevista y las preguntas que se le van a hacer.

(b) Planificación de la entrevista y preparación del entrevistado: establecer fecha, hora, lugar y duración de cada entrevista de acuerdo con el entrevistado.

(c) Selección del tipo de preguntas a usar y su estructura.

</details>

* ***3. Enumerar y describir brevemente qué tipos de preguntas puede contener una entrevista. Detalle ventajas y desventajas de cada una.***

<details><summary><code>Respuesta 🖱</code></summary><br>

Tipos de Preguntas que puede contener una entrevista:

* Abiertas

Permite al encuestado responder de cualquier manera, por ejemplo: ¿Qué opinión tiene del sistema actual? ¿Cómo describe su trabajo?

* Cerradas

Las respuestas son directas, cortas o de selección específica, por ejemplo: ¿Quién recibe este informe? ¿Cuántas personas utilizan el sistema?

* Sondeo

Las mismas ermiten obtener más detalle sobre un tema puntual, por ejemplo: ¿Podría dar detalles sobre tal cosa…? ¿Podría dar un ejemplo de tal cosa…?

</details>

* ***4. Enumerar y describir brevemente qué tipo de estructuras y organización existen para el armado de una entrevista.***

<details><summary><code>Respuesta 🖱</code></summary><br>

Las entrevistas pueden ser:

* Estructuradas (Cerradas)

En este caso el encuestador tiene un conjunto específico de preguntas para hacérselas al entrevistado, se busca dirigir al usuario sobre un requerimiento puntual. Por esto no permite adquirir un amplio conocimiento del dominio.

* No estructuradas (Abiertas)

En este tipo de entrevistas el encuestador lleva un tema en general, y no hay una preparación de preguntas específicas. Se Inicia con preguntas que no dependen del contexto, para conocer el problema, la gente involucrada, etc.

</details>

* ***5. Analizar un formato de la planilla adecuado al momento de armar una entrevista.***

<details><summary><code>Respuesta 🖱</code></summary><br>
  
</details>

* ***6. Analizar un formato de la planilla adecuado al momento de terminar una entrevista.***

<details><summary><code>Respuesta 🖱</code></summary><br>
  
</details>

### Parte II Situaciones.

* ***Situación 1***

***Tiene una entrevista con el gerente de ventas de una empresa el cual desea informatizar dicho sector pero no tuvo tiempo de preparar las preguntas por lo que le pidió a un nuevo empleado que le prepare algunas. Cuando las lee, se da cuenta que son inadecuadas. Leer las preguntas y volver a redactarlas de una manera más apropiada.Especificar por qué le parece inadecuada cada una de ellas.***

***a. Sus subordinados me dijeron que la empresa no anda bien. ¿Es cierto?***

***b. Soy nuevo en esto. ¿Qué he dejado afuera?***

***c. ¿Estará usted de acuerdo con los demás gerentes de ventas, respecto a que computarizar las ventas mensuales y luego realizar un análisis de la tendencia tendría usted grandes mejoras?***

***d. ¿No habrá una mejor manera de hacer proyecciones de sus ventas, que ese procedimiento anticuado que usted utiliza?***

<details><summary><code>Respuesta 🖱</code></summary><br>
  
a. Me parece muy informal y además estoy agregando un juicio de valor en la pregunta, parece una acusación y condiciono al entrevistado con la misma. En lugar de eso puedo preguntar: 

"He oído que ha habido preocupaciones sobre el desempeño actual de la empresa. ¿Podría comentar sobre la situación actual y cómo la empresa está abordando estos desafíos?"

b. No esta bien indicar que uno es nuevo, o no de ese modo. También es muy informal la pregunta en general. Podemos reescribirla como:

"Al ser nuevo en este campo, me gustaría entender mejor los aspectos clave que debo tener en cuenta. ¿Hay áreas importantes o aspectos que pueda estar pasando por alto y que sean cruciales para tener una visión completa?"

c. En primer lugar, está mal redactada, además condiciono al decir "esta usted de acuerdo", la persona puede opinar distinto, mejor ser más imparcial para que el entrevistado no se sienta condicionado a responder. Por ejemplo:

"¿Cuál es su opinión sobre la propuesta de computarizar las ventas mensuales y realizar un análisis de tendencias? ¿Cree que esta estrategia podría ofrecer mejoras significativas en el proceso de gestión de ventas?"

d. La pregunta es un poco brusca al hacer un juicio de valor ante el procedimiento utilizado por el entrevistado, me parece que con esta pregunta se va al choque. En lugar de eso podemos decir:

"¿Existen métodos más modernos o eficientes para hacer proyecciones de ventas que podrían mejorar el procedimiento actual? Me gustaría conocer su perspectiva sobre las alternativas disponibles."

</details>

* ***Situación 2***

***Apenas ha entrado a la oficina de su entrevistado se da cuenta que él no ha dejado de revisar papeles, mirar el reloj y hacer llamadas telefónicas. Usted supone que se siente nervioso porque está atrasado con otro trabajo que tiene que terminar.***

***a. Explicar brevemente cómo resolvería tal situación.***

***b. Qué opciones propone para el caso en que la entrevista no pueda reprogramarse.***

<details><summary><code>Respuesta 🖱</code></summary><br>

Trataría ante todo de mostrar empatía con el entrevistado, para evitar así ponerlo más nervioso. Ofrecería la oportunidad de reprogramar la entrevista, y en caso de no ser posible, buscaría hacer preguntas concisas y puntuales, de modo de priorizar el tiempo de la misma, sin apurar la entrevista, pero buscando abordar los puntos claves por lo cual iba a llevar a cabo la misma. Además dentificaría los temas más importantes para asegurarme de que se traten primero, en caso de que el tiempo de la entrevista se reduzca aún más.

</details>

* ***Situación 3***

***El siguiente es el primer informe de una entrevista realizada por uno de los miembros de su equipo de análisis de sistemas:***

***"En mi opinión, el resultado de la entrevista fue muy bueno. El entrevistado me permitió hablar con él durante una hora y media. Me relató toda la historia del negocio, que fue muy interesante. También mencionó que las cosas no han cambiado desde que él ha estado en la empresa, hace aproximadamente 16 años. En breve nos reuniremos nuevamente para terminar la entrevista, pues, no tuvimos tiempo para analizar las preguntas que preparé".***

***a. Leer atentamente el informe de la entrevista y explicar qué sensación le deja dicho informe.***

***b. Indicar si existe información que es irrelevante en el informe.***

***c. Mencionar tres sugerencias que le haría a su compañero de equipo para que realizara una mejor entrevista la próxima vez.***

<details><summary><code>Respuesta 🖱</code></summary><br>
  
a. Al leer el informe me genera la sensación de que el entrevistador no supo llevar bien la entrevista, puesto que las preguntas que tenía preparadas no pudo realizarlas. Pareciera que el entrevistado es quien habló y llevó las riendas de la conversación, y el entrevistador se limitó a conversar, olvidando que debía entrevistar a su cliente. Por esto mismo se quedó sin tiempo pues no llegó a preguntar lo que había pautado previamente.

b. Hay información irrelevante como el tiempo que duró la entrevista o el juicio de valor ante la conversación que tuvo con el entrevistado. La historia de la empresa, si bien puede ser interesante, por ahí no es tan relevante para una entrevista de análisis de sistemas. Además esta escrita de un modo muy coloquial, palabras como "aproximadamente" o "las cosas" no son apropiadas para un informe. 

c. Cómo sugerencias yo le diría que (1) Enfoque la entrevista en los objetivos específicos, armando una agenda clara con preguntas puntuales para dirigir la conversación siempre hacia esas preguntas. (2) Administrar el tiempo de una manera eficiente, para poder realizar la entrevista de una buena manera abarcando todos los temas que busca abordar en la misma. (3) Documentar la entrevista al finalizar para asegurarse que todos los puntos clave fueron hablados en la entrevista.

</details>

<br>
<br>
<br>

<p><img align="center" src="https://github.com/Marimari2342/Marimari2342/blob/main/firmagith.png" alt="marigit"/></p>