Nota 85/100

La resolución es bastante directa a partir de la interpretación del enunciado.

Objetos de dominio: Alumno, Materia, Curso, Carrera, Plan de Estudios, Oferta Académica.

A) Comentarios acerca de la resolución

1) Se debe hacer buen uso de las herramientas de modelado:
a) Los objetos deben estar correctamente definidos, con sus atributos y con identificador (si corresponde)
b) Las asociaciones deben tener nombre y multiplicidad
c) Los objetos asociativos deben estar correctamente definidos: son asociaciones y objetos al mismo tiempo.
d) En el modelo no debe haber:
d1) Atributos referenciales, es decir, atributos que contengan referencias a otros objetos (para eso están las asociaciones)
d2) Asociaciones reflexivas sin multiplicidades que incluyan condicionalidad (0..1; 0..*)
d3) Temas vinculados a la implementación

2) Temas importantes en este ejercicio:
Aclaración importante: el enunciado no describe al FIUBA. Por consiguiente se deben interpretar el enunciado tal como está descripto, sin agregarle condimentos propios de nuestra facultad (que son muchos y variados…)
Los objetos de dominio son los siguientes: Alumno, Materia, Curso, Carrera, Plan de Estudios, Oferta Académica.
Materia debe tener una asociación reflexiva para mostrar el tema de las correlatividades.
Para una materia puede haber varios cursos, que deben, además, estar asociados a la oferta académica. No queda claro si el mismo código de curso se puede repetir en distintos periodos. Ambas interpretaciones son válidas.
Es crítico poder determinar a qué plan de estudios pertenece el alumno, para identificar así correctamente las correlativas. Se pueden establecer dos asociaciones, una entre Alumno y Carrera y otra entre Alumno y Plan de Estudios. De todas maneras, si el Alumno está asociado solamente a Plan de Estudios, y este, a su vez, con Carrera, el requisito se resuelve igual.

B) Comentarios para el alumno.

-Falta asociar el Alumno con el Plan de Estudios. No hay forma de resolver la historia.

Saludos
