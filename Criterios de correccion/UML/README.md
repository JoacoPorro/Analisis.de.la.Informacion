## Criterios de corrección UML

Aspectos generales del modelo de dominio:

Muy críticos (invalidan la resolución si no están presentes)

a) En el modelo no debe haber:

a1) Atributos referenciales, es decir, atributos que contengan referencias a otros objetos (para eso están las asociaciones)

a2) Asociaciones reflexivas sin multiplicidades que incluyan condicionalidad (0..1; 0..*)

a3) Temas vinculados a la implementación

b) El modelo debe respetar la notación UML, considerando las particularidades del modelado de dominio:

b1) No puede haber asociaciones que terminen en flecha (indican un aspecto de implementación)

b2) No corresponde indicar cardinalidades/multiplicidades en asociaciones de especialización-generalización

c) No debe modelarse una entidad como un atributo ni viceversa.

d) Se deben indicar cardinalidades en los extremos de asociaciones

e) No se debe modelar aquello que no está especificado dentro del dominio y contexto de la actividad

Críticos (problemas graves)

a) Se debe hacer buen uso de las herramientas de modelado:
Las entidades deben estar correctamente definidas, con sus atributos y con identificador (si corresponde)
Las asociaciones deben tener nombre y multiplicidad
Las entidades asociativas deben estar correctamente definidas: son asociaciones y entidades al mismo tiempo.
b) Modelar la misma asociación dos veces (con dos líneas). En este caso alcanza con una sola línea y se puede indicar arriba y abajo la lectura de la asociación indicando los sentidos en caso de que clarifique la interpretación o indicar roles en los extremos de la asociación cerca de las cardinalidades.
c) No confundir rombo lleno y vacío (el primero indica composición, el segundo agregación) y lado del rombo (va del lado de la entidad contenedora).
d) Se debe indicar el nombre de la asociación y/o el sentido de lectura
e) No se indica con el signo “/“ en los atributos calculados
f) Se deben modelar todos atributos. No debe faltar ninguno.

No críticos (problemas leves)

a) No se deben incluir indicadores de acceso de atributos (signo “+”, signo “-“ por delante de cada propiedad)
b) Se debe indicar si la cardinalidad es 0 o 1 a muchos (no se debe usar solamente el “*”)
c) Se debe respetar el nombre de los atributos indicados en el enunciado/dominio (no se debe utilizar otro idioma)
d) Los nombres de entidades o asociaciones no deben ser confusos.

Recomendaciones

- Modelar las entidades en singular
- Dudar de entidades sin atributos propios/vacías. Verificar que es una entidad fuerte del dominio.
- Agregar pequeñas notas aclaratorias al modelo
- Las asociaciones de agregación/composición deben ser claras y justificadas. En caso contrario, utilizar asociaciones simples
- Una asociación 1 a 1 de una entidad A con una entidad B que tiene un solo atributo tiene alta probabilidad de ser un atributo de la entidad A
- Evitar modelar usuarios del sistema si no se requiere recordar algo de ellos
- Evitar modelar utilizando relaciones n-arias
