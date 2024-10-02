# Ingeniería de Software 1 - Practica 3: Casos de Uso

## Parte I: Definiciones generales

a) Describir qué es el desarrollo centrado en el usuario.

b) Definir qué son los casos de uso y describa cómo se utilizan.

c) Definir qué es un actor y un escenario.

d) Definir las relaciones que pueden presentarse en el diagrama de casos de uso. Describa cuándo se utiliza cada una.

e) Enumerar los beneficios de modelar requerimientos del sistema con casos de uso.

<details><summary> <code> Respuesta 🖱 </code></summary><br>

### a) **Desarrollo centrado en el usuario (UCD)**

El **desarrollo centrado en el usuario** es un enfoque de diseño y desarrollo de productos o sistemas que se basa en las necesidades, objetivos y experiencias de los usuarios finales. Su objetivo es asegurar que el producto cumpla con las expectativas de los usuarios, ofreciendo soluciones eficientes, usables y satisfactorias. El proceso de UCD generalmente implica investigación y pruebas con usuarios reales durante todo el ciclo de vida del producto, lo que permite iterar y ajustar el diseño en función del feedback obtenido.

--------------------------------

### b) **Casos de uso**

Un **caso de uso** es una técnica de modelado que describe cómo un sistema o software interactúa con actores externos (usuarios o sistemas). Representa una secuencia de acciones realizadas por un usuario o actor para lograr un objetivo específico dentro del sistema. Cada caso de uso detalla los pasos que sigue el usuario y las respuestas del sistema ante distintas situaciones.

Los **casos de uso** se utilizan para:

1. Capturar y definir los requerimientos funcionales del sistema.

2. Proporcionar una base para la estimación del esfuerzo de desarrollo.

3. Facilitar la comunicación entre desarrolladores, analistas y clientes.

Cada caso de uso incluye una descripción de cómo el sistema responde a los diferentes eventos o acciones iniciadas por los actores. A menudo, se presentan en forma de diagramas y se acompañan de una narrativa detallada.

--------------------------------

### c) **Actor y escenario**

- **Actor**: Un actor es cualquier entidad externa que interactúa con el sistema, ya sea un usuario, otro sistema o incluso el tiempo. Los actores realizan acciones o reciben respuestas del sistema. Los actores no forman parte del sistema en sí, pero influyen en él y pueden ser:

  - **Actores primarios**: Aquellos que inician una interacción con el sistema (por ejemplo, un usuario humano).

  - **Actores secundarios**: Aquellos que participan como parte de la interacción iniciada por un actor primario (como un sistema de pagos).

- **Escenario**: Un escenario es una secuencia de acciones que describe un caso particular de uso. Un escenario puede representar:

  - **Escenario principal**: La secuencia estándar y exitosa de acciones que el sistema sigue para cumplir con el objetivo del caso de uso.

  - **Escenario alternativo**: Situaciones donde el flujo principal se desvía, como errores o excepciones.

--------------------------------

### d) **Relaciones en el diagrama de casos de uso**

Existen varias relaciones que pueden aparecer en un diagrama de casos de uso:

1. **Asociación**: Representa una interacción entre un actor y un caso de uso. Se usa cuando un actor participa directamente en el caso de uso.

   - **Cuándo se usa**: Para describir la relación básica entre actores y casos de uso.

2. **Generalización**: Indica una relación de herencia entre actores o entre casos de uso. Un actor o caso de uso puede heredar características de otro.

   - **Cuándo se usa**: Cuando un actor o caso de uso hijo extiende o especializa el comportamiento de uno padre. Por ejemplo, un actor "Cliente preferencial" hereda características de "Cliente".

3. **Inclusión**: Un caso de uso incluye a otro cuando siempre que el caso de uso principal ocurre, el caso de uso incluido también debe ejecutarse.

   - **Cuándo se usa**: Cuando hay comportamiento común que debe ser reutilizado por múltiples casos de uso. Por ejemplo, un caso de uso "Iniciar sesión" puede ser incluido en otros casos como "Realizar compra" o "Consultar saldo".

4. **Extensión**: Un caso de uso puede extender a otro cuando añade comportamiento opcional que se ejecuta bajo ciertas condiciones.

   - **Cuándo se usa**: Para modelar variaciones en el comportamiento. Por ejemplo, un caso de uso "Realizar compra" puede ser extendido por un caso de uso "Aplicar descuento" que solo ocurre si el cliente tiene un cupón válido.

--------------------------------

### e) **Beneficios de modelar requerimientos con casos de uso**

1. **Facilitan la comunicación**: Los casos de uso son fáciles de entender tanto por usuarios técnicos como por no técnicos, lo que mejora la colaboración entre equipos de desarrollo y stakeholders.

2. **Capturan los requisitos funcionales**: Ayudan a documentar lo que el sistema debe hacer desde la perspectiva del usuario, alineando los requerimientos del sistema con las expectativas del cliente.

3. **Mejoran la planificación**: Proporcionan una base clara para la estimación de tiempo y recursos, lo que facilita la planificación del desarrollo.

4. **Enfocan el desarrollo en el usuario**: Al centrarse en las interacciones del usuario con el sistema, se asegura que el producto final atienda las necesidades y objetivos del usuario.

5. **Promueven la trazabilidad**: Cada caso de uso puede estar vinculado a requisitos funcionales específicos, lo que facilita el seguimiento y la validación de que los requisitos han sido cubiertos durante el desarrollo.

6. **Ayudan en la identificación de errores y excepciones**: Los escenarios alternativos y extensiones permiten identificar y manejar situaciones no estándar que pueden generar errores.

</details>