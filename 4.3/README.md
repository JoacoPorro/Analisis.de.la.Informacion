## Coregido Nota 80/100

![Joaquín Porro - 9520-Actividad 4 3 (Desarrollo)_page-0001](https://github.com/jporro/AnalisisDeLaInformacion/assets/103942784/35b7e350-96c7-4546-84af-baee108fdd9f)

![4 3 nose](https://github.com/jporro/AnalisisDeLaInformacion/assets/103942784/834a77fa-158f-45b8-bfa8-bd97c2ccdec5)

### Correcciones
![image](https://github.com/jporro/AnalisisDeLaInformacion/assets/103942784/e6a70300-d068-486d-b5f6-ead480260b94)

### Criterio especifico para el ejercicio
#### Aspectos muy críticos que deben estar en el modelo (si no están, invalidan toda la resolución)

* La asociación reflexiva en el objeto Categoría debe ser 0..1 a 0..* (es una jerarquía, no una red) La condicionalidad es clave; si falta, la asociación es infinita (para todas las categorías habría una categoría inferior y otra superior)

* Un producto debe pertenecer a una sola categoría, pero no todas las categorías deben tener productos asociados (multiplicidad condicional)

*  El Stock o la CantidadDepositada debe ser un objeto asociativo entre Depósito y Producto. La asociación debe ser condicional de ambos lados (si no hay stock de un producto, no puede tener asociado un depósito)

* Pedido es un objeto, ÍtemPedido (o ProductoPedido) debe ser un asociativo entre Pedido y Producto. Alternativa menos sugerida en este caso: ítemPedido como un objeto fuerte (es decir, no asociativo) con una relación de composición con respecto al Pedido.

* Factura e ÍtemFactura, ídem anterior.

* Como los pedidos se facturan una vez al mes, los ítems del pedido deben estar relacionados con cero o muchos ítems facturados.

* Es necesario indicar la cantidad facturada en el ítem de la factura (la cantidad pedida se puede distribuir entre varias facturas) y el precio unitario (es el vigente al momento de generar la factura, que no debería variar como sí podría variar el precio incluido en el Producto)



#### Aspectos críticos que deben estar en el modelo (si no están, impactan en la resolución pero no necesariamente la invalidan)

- El objeto Pedido (y, opcionalmente, Factura) debe estar asociado al objeto Cliente.

- En Factura debe incluirse el importe total de la factura (como campo calculado). En el ítem de la factura, el total del ítem (que es el resultado de hacer el precio por la cantidad)

#### Aspectos no críticos que deben estar en el modelo (si no están, impactan levemente en la resolución)

- Si se incluye el campo Stock en Producto, debe estar antecedido con “/” (es un campo calculado que se obtiene de sumar las cantidades en stock del producto en los diferentes depósitos)
