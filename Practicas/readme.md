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

<details><summary><code>Respuesta 🖱</code></summary>
  
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

***Indicar para cada problema quiénes podrían ser los Stakeholders, los puntos de vista y las fuentes de información.***

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

