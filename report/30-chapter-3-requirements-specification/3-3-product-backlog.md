## 3.3. Product Backlog

El Product Backlog de Nexa organiza las User Stories definidas en la sección 3.1 según valor de negocio, dependencia funcional e impacto operativo. La priorización se orienta al flujo principal del producto: catálogo gourmet, solicitud de compra, validación comercial, reserva de inventario, preparación FEFO, despacho, tracking, documentos comerciales y proceso de pago simulado.

El orden del backlog favorece primero las capacidades que permiten registrar demanda B2B, validar solicitudes, comprometer inventario y completar la atención operativa con trazabilidad. Las capacidades de administración, configuración, mantenimiento de catálogo, gestión de clientes, portales externos, inventario detallado y analítica se ubican después del flujo central porque sostienen la operación, pero no reemplazan el valor principal entregado al comprador y al equipo comercial-logístico.

La estimación utiliza la escala de **1, 2, 3, 5 y 8 Story Points**. El valor 1 representa una acción muy menor; 2, una consulta, filtro, estado visible o notificación simple; 3, una acción funcional pequeña con validación o persistencia; 5, un flujo medio con reglas de negocio o impacto operativo claro; y 8, un flujo crítico o transversal que cambia estado de negocio, cruza actores o depende de varias reglas.

**Product Backlog de Nexa**

| # Orden | User Story Id | Título | Descripción | Story Points (1 / 2 / 3 / 5 / 8) |
|---:|---|---|---|---:|
| 1 | US01 | Consultar catálogo gourmet autorizado | **Como** comprador B2B, **deseo** consultar el catálogo gourmet refrigerado autorizado para mi cuenta, **para** identificar productos disponibles antes de preparar una solicitud de compra. | 5 |
| 2 | US02 | Buscar productos por nombre comercial o código interno | **Como** comprador B2B, **deseo** buscar productos por nombre comercial o código interno, **para** encontrar con rapidez los productos que necesito reabastecer. | 2 |
| 3 | US03 | Filtrar productos por categoría gourmet | **Como** comprador B2B, **deseo** filtrar productos por categorías como quesos, charcutería, fiambres premium, lácteos gourmet o mantequillas especiales, **para** revisar grupos alineados a mi necesidad de compra. | 2 |
| 4 | US04 | Revisar ficha comercial del producto | **Como** comprador B2B, **deseo** revisar la ficha de un producto gourmet refrigerado, **para** decidir considerando precio, unidad, conservación, presentación y disponibilidad comercial. | 3 |
| 5 | US05 | Reconocer disponibilidad comercial limitada | **Como** comprador B2B, **deseo** reconocer cuándo un producto tiene disponibilidad comercial limitada, **para** evitar asumir que toda cantidad solicitada será confirmada automáticamente. | 2 |
| 6 | US12 | Visualizar ofertas según plan y cuenta | **Como** comprador B2B, **deseo** visualizar ofertas disponibles para mi cuenta y plan comercial, **para** aprovechar condiciones vigentes al preparar una solicitud. | 2 |
| 7 | US13 | Iniciar solicitud desde productos seleccionados | **Como** comprador B2B, **deseo** iniciar una solicitud con productos seleccionados del catálogo, **para** preparar un pedido sujeto a validación comercial. | 5 |
| 8 | US14 | Ajustar cantidades solicitadas | **Como** comprador B2B, **deseo** ajustar cantidades de cada producto, **para** adecuar la solicitud a la demanda real de mi negocio. | 3 |
| 9 | US15 | Registrar observaciones de compra | **Como** comprador B2B, **deseo** registrar observaciones sobre entrega, prioridad o condiciones esperadas, **para** ayudar a que la distribuidora evalúe mejor mi solicitud. | 3 |
| 10 | US16 | Revisar resumen antes de enviar solicitud | **Como** comprador B2B, **deseo** revisar productos, cantidades y total estimado antes de enviar una solicitud, **para** reducir errores de abastecimiento. | 3 |
| 11 | US17 | Enviar solicitud de compra | **Como** comprador B2B, **deseo** enviar mi solicitud de compra a la distribuidora, **para** recibir validación de disponibilidad, cliente y condiciones comerciales. | 8 |
| 12 | US18 | Recibir constancia de solicitud enviada | **Como** comprador B2B, **deseo** recibir una constancia inicial de solicitud enviada, **para** saber que aún no es una orden confirmada y que será revisada. | 2 |
| 13 | US19 | Consultar mis solicitudes | **Como** comprador B2B, **deseo** consultar mis solicitudes enviadas, **para** revisar su estado sin depender de llamadas o mensajes externos. | 3 |
| 14 | US20 | Revisar detalle de solicitud | **Como** comprador B2B, **deseo** revisar el detalle de una solicitud, **para** entender productos, observaciones, estado y acciones pendientes. | 3 |
| 15 | US21 | Responder observaciones comerciales | **Como** comprador B2B, **deseo** responder observaciones o ajustes solicitados por coordinación comercial, **para** desbloquear la evaluación de mi solicitud. | 5 |
| 16 | US25 | Actualizar datos operativos de comprador | **Como** comprador B2B, **deseo** actualizar datos operativos de mi perfil, dirección de entrega y preferencias de notificación, **para** reducir errores de atención en solicitudes y órdenes futuras. | 3 |
| 17 | US22 | Cancelar solicitud no confirmada | **Como** comprador B2B, **deseo** cancelar una solicitud que aún no fue confirmada como orden, **para** evitar la atención de una compra que ya no necesito. | 3 |
| 18 | US23 | Consultar órdenes confirmadas | **Como** comprador B2B, **deseo** consultar mis órdenes confirmadas, **para** diferenciar solicitudes en revisión de compras aceptadas por la distribuidora. | 3 |
| 19 | US24 | Revisar detalle de orden confirmada | **Como** comprador B2B, **deseo** revisar el detalle de una orden confirmada, **para** conocer productos aprobados, cantidades, estado operativo y documentos asociados. | 3 |
| 20 | US26 | Revisar bandeja de solicitudes | **Como** coordinadora comercial, **deseo** revisar la bandeja de solicitudes de compra, **para** priorizar las solicitudes enviadas por compradores B2B. | 5 |
| 21 | US27 | Filtrar solicitudes por estado | **Como** coordinadora comercial, **deseo** filtrar solicitudes por estado, **para** atender primero las que requieren validación, ajuste o respuesta al comprador. | 2 |
| 22 | US28 | Validar cliente de una solicitud | **Como** coordinadora comercial, **deseo** validar el cliente asociado a la solicitud, **para** confirmar que la compra corresponde a una cuenta B2B atendible. | 5 |
| 23 | US29 | Validar RUC y datos comerciales | **Como** coordinadora comercial, **deseo** revisar RUC, razón social y datos de contacto, **para** reducir errores antes de confirmar una orden. | 3 |
| 24 | US30 | Revisar condiciones comerciales del cliente | **Como** coordinadora comercial, **deseo** revisar crédito, forma de pago y condiciones pactadas, **para** decidir si la solicitud puede avanzar comercialmente. | 5 |
| 25 | US31 | Consultar disponibilidad visible para validar | **Como** coordinadora comercial, **deseo** consultar disponibilidad comercial visible durante la validación, **para** comunicar al comprador si la solicitud requiere ajuste. | 3 |
| 26 | US32 | Solicitar ajuste al comprador | **Como** coordinadora comercial, **deseo** solicitar ajustes sobre productos, cantidades o datos, **para** completar solicitudes antes de rechazarlas o convertirlas en orden. | 5 |
| 27 | US33 | Rechazar solicitud con motivo | **Como** coordinadora comercial, **deseo** rechazar una solicitud con motivo claro, **para** cerrar solicitudes que no pueden atenderse sin dejar ambigüedad al comprador. | 3 |
| 28 | US34 | Confirmar validación comercial | **Como** coordinadora comercial, **deseo** confirmar que cliente y condiciones comerciales fueron validados, **para** habilitar la reserva operativa antes de la orden. | 5 |
| 29 | US35 | Convertir solicitud validada en orden | **Como** coordinadora comercial, **deseo** convertir una solicitud validada en orden de compra, **para** formalizar la atención comercial después de validar cliente e inventario reservado. | 8 |
| 30 | US36 | Comunicar confirmación al comprador | **Como** coordinadora comercial, **deseo** comunicar la confirmación de una orden al comprador, **para** informar el compromiso comercial aceptado. | 3 |
| 31 | US37 | Mantener conversación con comprador | **Como** coordinadora comercial, **deseo** mantener mensajes asociados a solicitud u orden, **para** resolver dudas sin perder trazabilidad. | 3 |
| 32 | US52 | Consultar inventario operativo | **Como** jefatura logística, **deseo** consultar inventario operativo por producto, **para** evaluar disponibilidad real antes de preparar o confirmar órdenes. | 3 |
| 33 | US61 | Reservar inventario para solicitud validada | **Como** jefatura logística, **deseo** reservar inventario para una solicitud validada, **para** asegurar disponibilidad antes de convertirla en orden. | 8 |
| 34 | US63 | Aplicar criterio FEFO en reserva | **Como** jefatura logística, **deseo** aplicar criterio FEFO al reservar inventario, **para** priorizar lotes con vencimiento más cercano. | 8 |
| 35 | US64 | Preparar orden con lotes trazables | **Como** jefatura logística, **deseo** asociar lotes a la preparación de la orden, **para** mantener trazabilidad desde inventario hasta despacho. | 5 |
| 36 | US65 | Bloquear confirmación sin reserva | **Como** jefatura logística, **deseo** impedir que una orden avance sin reserva suficiente, **para** evitar compromisos comerciales sin respaldo operativo. | 8 |
| 37 | US62 | Liberar reserva no confirmada | **Como** jefatura logística, **deseo** liberar reservas de solicitudes rechazadas o canceladas, **para** devolver disponibilidad al inventario operativo. | 3 |
| 38 | US66 | Crear orden de despacho | **Como** responsable operativo, **deseo** crear una orden de despacho a partir de una orden confirmada, **para** iniciar la preparación de entrega. | 5 |
| 39 | US67 | Consultar tablero de despachos | **Como** responsable operativo, **deseo** consultar despachos por estado, **para** organizar la operación diaria de salida y entrega. | 2 |
| 40 | US68 | Asignar responsable de entrega | **Como** responsable operativo, **deseo** asignar una entrega a una persona encargada, **para** mantener responsabilidad trazable durante el despacho. | 3 |
| 41 | US69 | Programar entrega | **Como** responsable operativo, **deseo** programar fecha y ventana de entrega, **para** coordinar preparación y recepción del comprador. | 5 |
| 42 | US70 | Iniciar salida de despacho | **Como** responsable operativo, **deseo** marcar el inicio de salida de una entrega, **para** actualizar el tracking visible de la orden. | 3 |
| 43 | US71 | Actualizar estado de despacho | **Como** responsable operativo, **deseo** actualizar estados de despacho, **para** informar a comercial y comprador sobre el avance operativo. | 5 |
| 44 | US72 | Registrar incidencia logística | **Como** responsable operativo, **deseo** registrar incidencias de entrega, **para** dejar constancia de retrasos, diferencias o problemas de recepción. | 3 |
| 45 | US73 | Reprogramar entrega | **Como** responsable operativo, **deseo** reprogramar una entrega con motivo, **para** actualizar la planificación cuando exista retraso o incidencia. | 3 |
| 46 | US74 | Monitorear estado logístico para comunicar | **Como** coordinadora comercial, **deseo** monitorear el estado logístico de órdenes, **para** responder al comprador con información vigente. | 3 |
| 47 | US75 | Consultar tracking de orden | **Como** comprador B2B, **deseo** consultar tracking de mi orden, **para** planificar recepción sin depender de consultas manuales. | 3 |
| 48 | US76 | Registrar temperatura referencial | **Como** responsable operativo, **deseo** registrar temperatura referencial de despacho, **para** documentar el cuidado de productos refrigerados dentro del alcance del prototipo. | 3 |
| 49 | US77 | Generar alerta por temperatura referencial | **Como** responsable operativo, **deseo** generar alerta cuando la temperatura referencial esté fuera de rango, **para** revisar una posible incidencia de conservación. | 3 |
| 50 | US78 | Completar entrega | **Como** responsable operativo, **deseo** completar una entrega, **para** cerrar el avance logístico y habilitar documentos o evidencias correspondientes. | 5 |
| 51 | US79 | Registrar proof of delivery | **Como** responsable operativo, **deseo** registrar proof of delivery, **para** respaldar que la orden fue recibida por el comprador. | 8 |
| 52 | US80 | Consultar evidencia visible de entrega | **Como** comprador B2B, **deseo** consultar evidencia visible de entrega, **para** confirmar el cierre operativo de mi orden. | 3 |
| 53 | US82 | Consultar resumen de cobro | **Como** comprador B2B, **deseo** consultar el resumen de cobro de mi orden, **para** comprender el importe antes de confirmar un pago o crédito. | 5 |
| 54 | US83 | Ver subtotal, descuentos, envío, IGV y total | **Como** comprador B2B, **deseo** ver subtotal, descuentos, envío, IGV y total, **para** validar el cálculo referencial de mi compra. | 3 |
| 55 | US84 | Seleccionar método de pago | **Como** comprador B2B, **deseo** seleccionar un método de pago, **para** continuar el cierre de pago según las condiciones acordadas con la importadora. | 5 |
| 56 | US85 | Usar tarjeta o billetera digital | **Como** comprador B2B, **deseo** usar Visa, Mastercard, Apple Pay o Google Pay, **para** representar un pago con tarjeta o billetera digital dentro del prototipo. | 3 |
| 57 | US86 | Usar PayPal, Yape o Plin | **Como** comprador B2B, **deseo** usar PayPal, Yape o Plin, **para** representar alternativas de pago frecuentes sin ejecutar una transacción real. | 3 |
| 58 | US87 | Usar transferencia o línea de crédito B2B | **Como** comprador B2B, **deseo** seleccionar transferencia bancaria o línea de crédito B2B cuando aplique, **para** continuar el flujo según mi condición comercial. | 3 |
| 59 | US88 | Confirmar proceso de pago | **Como** comprador B2B, **deseo** confirmar el proceso de pago, **para** cerrar el flujo de compra con un resultado trazable dentro del alcance del prototipo. | 8 |
| 60 | US89 | Recibir resultado de pago | **Como** comprador B2B, **deseo** recibir el resultado de pago, **para** saber si la orden puede continuar según el escenario registrado. | 3 |
| 61 | US90 | Revisar documentos comerciales | **Como** coordinadora comercial, **deseo** revisar documentos comerciales asociados a solicitud u orden, **para** comunicar al comprador el estado documental con claridad. | 5 |
| 62 | US92 | Consultar documentos comerciales visibles | **Como** comprador B2B, **deseo** consultar documentos comerciales visibles de mis órdenes, **para** acceder a factura referencial, guía, CDR o POD permitido según estado. | 3 |
| 63 | US93 | Recibir notificación de documento o pago | **Como** comprador B2B, **deseo** recibir notificación cuando exista actualización de pago o documento, **para** dar seguimiento al cierre de la compra. | 2 |
| 64 | US94 | Consultar estado de pago de la orden | **Como** coordinadora comercial, **deseo** consultar si una orden está pagada, pendiente o fallida, **para** priorizar seguimiento, documentación y comunicación con el comprador. | 3 |
| 65 | US91 | Consultar información de cobros operativos | **Como** company owner, **deseo** consultar información de cobros operativos de la empresa, **para** conocer importes referenciales asociados a la cuenta. | 3 |
| 66 | US06 | Consultar catálogo durante validación | **Como** coordinadora comercial, **deseo** consultar catálogo, precios y disponibilidad comercial visible, **para** validar solicitudes de compra con información alineada al producto ofrecido. | 3 |
| 67 | US59 | Consultar stock visible para comunicación | **Como** coordinadora comercial, **deseo** consultar stock visible sin acceder al inventario interno completo, **para** comunicar posibilidades de atención al comprador. | 3 |
| 68 | US60 | Ver disponibilidad comercial sin inventario interno | **Como** comprador B2B, **deseo** ver disponibilidad comercial general sin detalle interno de almacén, **para** preparar solicitudes con expectativas razonables. | 2 |
| 69 | US38 | Registrar pedido recibido por canal externo | **Como** coordinadora comercial, **deseo** registrar solicitudes recibidas por WhatsApp, llamada o papel, **para** integrarlas al flujo formal de Nexa. | 5 |
| 70 | US39 | Asociar cliente a registro manual | **Como** coordinadora comercial, **deseo** asociar un cliente B2B a un registro manual, **para** aplicar sus datos y condiciones comerciales durante la atención. | 3 |
| 71 | US40 | Completar productos y cantidades manuales | **Como** coordinadora comercial, **deseo** completar productos y cantidades solicitadas por canal externo, **para** evitar pérdida de información comercial. | 3 |
| 72 | US41 | Revisar registro manual antes de enviar | **Como** coordinadora comercial, **deseo** revisar el pedido capturado antes de enviarlo a validación, **para** reducir errores de cliente, producto o cantidad. | 3 |
| 73 | US42 | Diferenciar origen de solicitud | **Como** coordinadora comercial, **deseo** diferenciar si una solicitud nació en el portal o fue capturada manualmente, **para** interpretarla con el contexto correcto. | 2 |
| 74 | US43 | Registrar cliente B2B | **Como** coordinadora comercial, **deseo** registrar clientes B2B con datos mínimos, **para** habilitar atención futura dentro de Nexa. | 3 |
| 75 | US44 | Actualizar datos de cliente B2B | **Como** coordinadora comercial, **deseo** actualizar datos de contacto y atención de un cliente, **para** evitar errores en confirmaciones, documentos o entrega. | 3 |
| 76 | US45 | Clasificar cliente por tipo de negocio | **Como** coordinadora comercial, **deseo** clasificar clientes por tipo de negocio, **para** adaptar la atención comercial y priorizar casos recurrentes. | 2 |
| 77 | US46 | Administrar datos de empresa | **Como** company owner, **deseo** revisar y actualizar datos básicos de la empresa contratante, **para** mantener la cuenta alineada con la operación real. | 5 |
| 78 | US47 | Administrar usuarios internos | **Como** company owner, **deseo** registrar usuarios internos autorizados, **para** asegurar que cada persona trabaje con una cuenta identificable. | 3 |
| 79 | US48 | Asignar responsabilidades de equipo | **Como** company owner, **deseo** asignar responsabilidades a usuarios internos, **para** permitir que cada persona acceda solo a funciones relacionadas con su trabajo. | 3 |
| 80 | US49 | Revisar plan Standard contratado | **Como** company owner, **deseo** revisar la visibilidad del plan Standard contratado, **para** entender capacidades disponibles y restricciones de la cuenta. | 2 |
| 81 | US50 | Consultar capacidades habilitadas por plan | **Como** company owner, **deseo** consultar las capacidades habilitadas por plan, **para** administrar funcionalidades disponibles sin confundir restricciones comerciales con errores del sistema. | 2 |
| 82 | US51 | Gestionar requerimientos operativos de portales externos | **Como** company owner, **deseo** gestionar requerimientos operativos de portales externos por cliente, **para** saber qué documentos o tareas manuales deben atenderse fuera de Nexa. | 5 |
| 83 | US07 | Actualizar información comercial del producto | **Como** company owner, **deseo** actualizar información comercial de productos activos, **para** mantener fichas, precios y visibilidad coherentes con la operación. | 3 |
| 84 | US08 | Agregar producto gourmet al catálogo | **Como** company owner, **deseo** agregar productos gourmet refrigerados al catálogo, **para** ampliar la oferta visible de la empresa contratante. | 3 |
| 85 | US09 | Desactivar producto con control comercial | **Como** company owner, **deseo** desactivar productos que ya no deben ofrecerse, **para** evitar que compradores generen nuevas solicitudes sobre productos no atendibles. | 3 |
| 86 | US10 | Evitar retiro de producto con órdenes activas | **Como** company owner, **deseo** impedir la remoción de un producto asociado a órdenes activas, **para** proteger la trazabilidad comercial y operativa. | 3 |
| 87 | US11 | Gestionar promociones operativas | **Como** company owner, **deseo** gestionar promociones u ofertas estacionales de productos gourmet, **para** orientar la demanda sin depender de mensajes manuales. | 3 |
| 88 | US53 | Revisar detalle de lotes | **Como** jefatura logística, **deseo** revisar lotes por producto, **para** controlar vencimiento, cantidad y condición de conservación. | 3 |
| 89 | US54 | Identificar lotes próximos a vencer | **Como** jefatura logística, **deseo** identificar lotes próximos a vencer, **para** priorizar su rotación y reducir merma. | 3 |
| 90 | US55 | Consultar stock bajo | **Como** jefatura logística, **deseo** identificar productos con stock bajo, **para** anticipar quiebres de disponibilidad en solicitudes nuevas. | 2 |
| 91 | US56 | Actualizar inventario referencial | **Como** jefatura logística, **deseo** actualizar inventario referencial, **para** mantener disponibilidad operativa alineada con el alcance del prototipo. | 3 |
| 92 | US57 | Registrar movimiento de stock | **Como** jefatura logística, **deseo** registrar movimientos de ingreso, salida o ajuste, **para** mantener trazabilidad de cambios operativos de inventario. | 3 |
| 93 | US58 | Justificar ajuste de disponibilidad | **Como** jefatura logística, **deseo** justificar ajustes manuales de disponibilidad, **para** evitar cambios sin explicación operativa. | 2 |
| 94 | US81 | Revisar analítica operativa de despachos | **Como** company owner, **deseo** revisar indicadores de despachos, incidencias y entregas, **para** identificar problemas recurrentes de operación. | 5 |

### Evidencia del Product Backlog en Jira

**Evidencia del Product Backlog en Jira**

![Product Backlog en Jira](../assets/images/chapter-3/jira/product-backlog-jira-tb1.png)

La evidencia visual muestra la gestión del Product Backlog de Nexa en Jira, incluyendo priorización, épicas, estados y estimación de User Stories.

**URL del Product Backlog:** [Jira Backlog — Proyecto Nexa](https://team-nexa.atlassian.net/jira/software/projects/NX/boards/1/backlog)

El Product Backlog prioriza el flujo de negocio que convierte una consulta de catálogo en una solicitud validada, una orden reservada y preparada con trazabilidad, un despacho con seguimiento, documentos visibles y un proceso de pago simulado. Esta organización permite orientar el desarrollo hacia las historias que reducen dependencia de canales informales, errores de redigitación, quiebres operativos y baja visibilidad documental.
