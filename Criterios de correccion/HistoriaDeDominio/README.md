## Criterios de Correccion Historias de Dominio

### Temas generales
Se deben desarrollar (graficar) las historias de dominio del escenario descripto en el enunciado. Qué aspectos deben reflejar:
##### a) Temas críticos (pueden invalidar la resolución)
- Se debe aplicar correctamente la técnica. 

- Las historias de dominio deben describir cómo trabajan en conjunto las personas. Hay actores, actividades y objetos de trabajo. No es diseño.
- Se debe describir el dominio del problema, no de la solución. 
- Las historias deben ser PURAS y la granularidad puede variar desde GRUESA hasta MEDIA o FINA.
- Deben estar descriptas desde el punto de vista de los actores.
- El vocabulario empleado debe ser el del dominio.
- Los objetos de trabajo deben representar un objeto del mundo real, una representación (virtual) de un objeto real, el medio a través del cual se intercambia información acerca de un objeto de trabajo. 
##### b) Temas críticos
- Se deben identificar correctamente los subdominios.
- Se deben secuenciar correctamente las actividades.
##### c) Temas menores
- Faltas de ortografía/falta de claridad en la redacción

### 2) Temas particulares
La cantidad de historias puede variar. Lo importante es que tengan el nivel de detalle suficiente para reflejar lo que describe el enunciado. Una posible solución:
##### a) Subdominio actualización de precios de matrículas y cuotas
HdD1) Administración y Cobranzas actualiza precio de matrícula
HdD2) Administración y Cobranzas actualiza precio de cuota(s)
##### b) Subdominio Facturación
HdD3) Administración y Cobranzas emite facturas (puede abrirse en facturas de matrículas y de cuotas) 
HdD4) Administración y Cobranzas envía facturas a los alumnos
##### c) Subdominio cobranzas
HdD5) Alumno paga factura con tarjeta (crédito/débito)
HdD6) Alumno paga factura con transferencia bancaria

B) Comentarios para el alumno:

- Pago con transferencia: hay que desdoblar la actividad de pago de la factura en dos.

- ¿Es la pérdida de regularidad realmente una actividad?


