## 4.4. Web Applications UX/UI Design

Esta sección documenta el diseño UX/UI de las superficies autenticadas de Nexa: la **Web Application interna** para los segmentos **S1 — Commercial Coordination** y **S2 — Operations / Account Owner**, y el **Buyer Portal** para **S3 — B2B Buyer Portal**. Estas superficies comparten el sistema visual definido en 4.1 y la arquitectura de información descrita en 4.2, pero se diferencian por densidad, navegación, nivel de detalle y responsabilidad de negocio.

La Web Application interna está orientada a operación diaria. S1 necesita validar solicitudes, revisar clientes, convertir purchase requests en purchase orders y gestionar documentos comerciales. S2 necesita controlar inventario, lotes, despacho, evidencias, analítica operativa, promociones, customer portals y administración de empresa/tenant. El Buyer Portal está orientado a autoservicio del comprador B2B: catálogo, request builder, solicitudes, pedidos, documentos visibles y seguimiento.

El diseño UX/UI se organiza por user goals y no únicamente por pantallas. Cada recorrido responde a una pregunta del dominio: qué solicitud debe validarse, qué pedido está bloqueado, qué lote requiere atención, qué despacho debe prepararse, qué evidencia falta y qué estado puede consultar el comprador. Por ello, esta sección presenta wireframes, wireflows, mockups y user flows como artefactos conectados.

> *Nota:* las evidencias visuales disponibles en este reporte se concentran principalmente en S1 y S2. El repositorio de la Web Application incluye rutas y vistas para S3; sin embargo, los wireframes y mockups específicos del Buyer Portal deben incorporarse como evidencia visual adicional cuando el equipo actualice los assets del reporte. No se agregan capturas inexistentes ni enlaces inventados.

### 4.4.1. Web Applications Wireframes

Los wireframes actuales de la Web Application se organizan por segmento operativo y por flujo de trabajo. La evidencia visual disponible cubre principalmente S1 y S2, mientras que S3 se documenta con estructura funcional y queda pendiente de actualización con wireframes específicos del Buyer Portal.

*Tabla: Wireframes de la Web Application por segmento*

| Segmento | Pantallas documentadas | Recorrido cubierto | Estado de evidencia |
|---|---|---|---|
| S1 — Commercial Coordination | Login, dashboard comercial, clientes, detalle de cliente, pedidos, creación de pedido, selección de productos, resumen, detalle de pedido y reportes | Ingreso, revisión comercial, gestión de clientes, registro de pedido, selección de productos, confirmación, seguimiento y consulta de reportes | Evidencia visual disponible |
| S2 — Operations / Account Owner | Login, dashboard logístico, inventario general, inventario por lote, detalle de lote, revisión operativa de pedido, despacho, registro de salida, notificación, confirmación y reportes operativos | Ingreso, control de inventario, revisión por lote, preparación de despacho, registro operativo, confirmación de salida y lectura de reportes | Evidencia visual disponible |
| S3 — B2B Buyer Portal | Home, Product Catalog, Product Detail, Request Builder, My Requests, My Orders, Business Documents, Premium y Profile | Consulta de catálogo, armado de solicitud, revisión de solicitudes, seguimiento de pedidos y documentos visibles | Pendiente de actualización con wireframes específicos |

> *Nota:* Los wireframes de S1 y S2 provienen de los artefactos visuales incluidos en el reporte. Para S3, el flujo funcional existe dentro de la Web Application, pero esta subsección debe complementarse con wireframes del Buyer Portal cuando el equipo los exporte desde Figma o la herramienta correspondiente.

#### S1 — Commercial Coordination

El recorrido S1 cubre el trabajo de Valeria Sánchez desde el ingreso a la plataforma hasta la consulta de reportes comerciales. La secuencia prioriza captura clara de pedidos, revisión de cliente, validación comercial, selección de productos y trazabilidad del pedido creado.

*Figura. Wireframe de login para S1*

![Wireframe de login para S1](../assets/images/chapter-4/webapp/wireframes/s1-coordinacion-comercial-ventas-internas/wireframe-login.jpg)

> *Nota:* La pantalla de ingreso separa el acceso autenticado del recorrido público de la Landing Page. Elaboración propia.

> *Nota:* Wireframe de dashboard comercial para S1*

![Wireframe de dashboard comercial para S1](../assets/images/chapter-4/webapp/wireframes/s1-coordinacion-comercial-ventas-internas/wireframe-dashboard.jpg)

> *Nota:* El dashboard reúne estado de pedidos, alertas comerciales y accesos a tareas frecuentes. Elaboración propia.

*Figura. Wireframe de lista de clientes para S1*

![Wireframe de lista de clientes para S1](../assets/images/chapter-4/webapp/wireframes/s1-coordinacion-comercial-ventas-internas/wireframe-clientes-lista.jpg)

> *Nota:* La lista permite ubicar clientes y revisar información comercial antes de iniciar o validar un pedido. Elaboración propia.

*Figura. Wireframe de detalle de cliente para S1*

![Wireframe de detalle de cliente para S1](../assets/images/chapter-4/webapp/wireframes/s1-coordinacion-comercial-ventas-internas/wireframe-detalle-cliente.jpg)

> *Nota:* El detalle concentra condiciones, datos relevantes y contexto necesario para decidir si el pedido puede avanzar. Elaboración propia.

*Figura. Wireframe de lista de pedidos para S1*

![Wireframe de lista de pedidos para S1](../assets/images/chapter-4/webapp/wireframes/s1-coordinacion-comercial-ventas-internas/wireframe-pedidos-lista.jpg)

> *Nota:* La bandeja de pedidos ordena estados, prioridades y acceso rápido al detalle. Elaboración propia.

*Figura. Wireframe de creación de pedido para S1*

![Wireframe de creación de pedido para S1](../assets/images/chapter-4/webapp/wireframes/s1-coordinacion-comercial-ventas-internas/wireframe-crear-pedido.jpg)

> *Nota:* La captura inicial del pedido separa cliente, condiciones y datos base para reducir ambigüedad. Elaboración propia.

*Figura. Wireframe de selección de productos para S1*

![Wireframe de selección de productos para S1](../assets/images/chapter-4/webapp/wireframes/s1-coordinacion-comercial-ventas-internas/wireframe-crear-pedido-productos.jpg)

> *Nota:* La selección de productos ayuda a revisar cantidades, disponibilidad y composición del pedido. Elaboración propia.

*Figura. Wireframe de resumen de pedido para S1*

![Wireframe de resumen de pedido para S1](../assets/images/chapter-4/webapp/wireframes/s1-coordinacion-comercial-ventas-internas/wireframe-crear-pedido-resumen.jpg)

> *Nota:* El resumen permite confirmar información antes de registrar o convertir el pedido. Elaboración propia.

*Figura. Wireframe de detalle de pedido para S1*

![Wireframe de detalle de pedido para S1](../assets/images/chapter-4/webapp/wireframes/s1-coordinacion-comercial-ventas-internas/wireframe-detalle-pedido.jpg)

> *Nota:* El detalle sostiene seguimiento comercial y lectura del historial de la orden. Elaboración propia.

*Figura. Wireframe de reportes para S1*

![Wireframe de reportes para S1](../assets/images/chapter-4/webapp/wireframes/s1-coordinacion-comercial-ventas-internas/wireframe-reportes.jpg)

> *Nota:* Los reportes comerciales consolidan información para revisar actividad, pedidos y desempeño del flujo. Elaboración propia.

#### S2 — Operations / Account Owner

El recorrido S2 cubre el trabajo de Roberto García desde el ingreso a la plataforma hasta la lectura de reportes operativos. La secuencia prioriza inventario, lotes, criterio FEFO, despacho, registro de salida, confirmación, evidencias y control operativo. Además, S2 asume la administración de empresa, cuenta, accesos y tenant, sin crear un segmento Admin separado.

*Figura. Wireframe de login para S2*

![Wireframe de login para S2](../assets/images/chapter-4/webapp/wireframes/s2-jefatura-logistica-coordinacion-operativa/wireframe-login.jpg)

> *Nota:* El acceso mantiene la separación por rol antes de entrar a módulos operativos. Elaboración propia.

*Figura. Wireframe de dashboard logístico para S2*

![Wireframe de dashboard logístico para S2](../assets/images/chapter-4/webapp/wireframes/s2-jefatura-logistica-coordinacion-operativa/wireframe-dashboard-logistica.jpg)

> *Nota:* El dashboard logístico prioriza pedidos en riesgo, inventario, preparación y despacho. Elaboración propia.

*Figura. Wireframe de inventario general para S2*

![Wireframe de inventario general para S2](../assets/images/chapter-4/webapp/wireframes/s2-jefatura-logistica-coordinacion-operativa/wireframe-inventario-vista-general.jpg)

> *Nota:* La vista general muestra disponibilidad, clasificación y señales operativas de inventario. Elaboración propia.

*Figura. Wireframe de inventario por lote para S2*

![Wireframe de inventario por lote para S2](../assets/images/chapter-4/webapp/wireframes/s2-jefatura-logistica-coordinacion-operativa/wireframe-inventario-por-lote.jpg)

> *Nota:* La lectura por lote facilita priorización FEFO y revisión de riesgo. Elaboración propia.

*Figura. Wireframe de detalle de lote para S2*

![Wireframe de detalle de lote para S2](../assets/images/chapter-4/webapp/wireframes/s2-jefatura-logistica-coordinacion-operativa/wireframe-detalle-lote.jpg)

> *Nota:* El detalle permite revisar condiciones específicas del lote antes de tomar acción operativa. Elaboración propia.

*Figura. Wireframe de creación o revisión operativa de pedido para S2*

![Wireframe de creación o revisión operativa de pedido para S2](../assets/images/chapter-4/webapp/wireframes/s2-jefatura-logistica-coordinacion-operativa/wireframe-crear-pedido-v2.jpg)

> *Nota:* Esta pantalla conecta información de pedido con revisión operativa y disponibilidad. Elaboración propia.

*Figura. Wireframe de despacho con pedidos listos para salir*

![Wireframe de despacho con pedidos listos para salir](../assets/images/chapter-4/webapp/wireframes/s2-jefatura-logistica-coordinacion-operativa/wireframe-despacho-listos-para-salir.jpg)

> *Nota:* El tablero de despacho agrupa pedidos listos y facilita priorizar salida. Elaboración propia.

*Figura. Wireframe de registro de salida para S2*

![Wireframe de registro de salida para S2](../assets/images/chapter-4/webapp/wireframes/s2-jefatura-logistica-coordinacion-operativa/wireframe-despacho-modal-registro.jpg)

> *Nota:* El registro recoge datos necesarios para dejar constancia del despacho. Elaboración propia.

*Figura. Wireframe de notificación de despacho para S2*

![Wireframe de notificación de despacho para S2](../assets/images/chapter-4/webapp/wireframes/s2-jefatura-logistica-coordinacion-operativa/wireframe-despacho-notificacion.jpg)

> *Nota:* La notificación confirma que el cambio de estado fue comunicado dentro del flujo. Elaboración propia.

*Figura. Wireframe de confirmación de despacho para S2*

![Wireframe de confirmación de despacho para S2](../assets/images/chapter-4/webapp/wireframes/s2-jefatura-logistica-coordinacion-operativa/wireframe-despacho-confirmacion.jpg)

> *Nota:* La confirmación permite cerrar el paso operativo de salida y mantener trazabilidad. Elaboración propia.

*Figura. Wireframe de reportes operativos para S2*

![Wireframe de reportes operativos para S2](../assets/images/chapter-4/webapp/wireframes/s2-jefatura-logistica-coordinacion-operativa/wireframe-reportes-operativos-v2.jpg)

> *Nota:* Los reportes operativos consolidan indicadores de inventario, despacho y cierre. Elaboración propia.

#### S3 — B2B Buyer Portal

El recorrido S3 corresponde a Elena Litano como compradora B2B. En la Web Application, este segmento se materializa mediante el Buyer Portal, cuyo propósito es reducir dependencia de WhatsApp, llamadas o coordinación manual para consultar catálogo, enviar solicitudes y revisar pedidos.

| Vista del Buyer Portal | Propósito UX | Ruta canónica |
|---|---|---|
| Home | Mostrar resumen de actividad, pedidos, solicitudes y accesos frecuentes | `/portal/home` |
| Product Catalog | Permitir búsqueda y selección de productos disponibles | `/portal/product-catalog` |
| Product Detail | Revisar información del producto antes de solicitarlo | `/portal/product-catalog/:id` |
| Request Builder | Confirmar productos, cantidades y datos de solicitud | `/portal/request-builder` |
| My Requests | Revisar solicitudes enviadas y su estado | `/portal/purchase-requests` |
| Request Detail | Consultar trazabilidad inicial, comentarios y estado de solicitud | `/portal/purchase-requests/:id` |
| My Orders | Revisar órdenes confirmadas | `/portal/purchase-orders` |
| Order Detail | Consultar tracking, documentos y estado operativo | `/portal/purchase-orders/:id` |
| Business Documents | Acceder a documentos visibles para el comprador | `/portal/business-documents` |
| Profile | Revisar datos de cuenta del comprador | `/portal/profile` |

> *Pendiente de actualización con evidencia real:* esta subsección debe complementarse con wireframes exportados del Buyer Portal.

### 4.4.2. Web Applications Wireflow Diagrams

Los wireflows conectan pantallas, decisiones y estados de interfaz. En Nexa se organizan por user goal para mantener trazabilidad entre el needfinding, la arquitectura de información, los mockups y la implementación.

*Tabla: Wireflows por user goal*

| User goal | Segmento y persona | Task flow resumido | Evidencia | Explicación |
|---|---|---|---|---|
| Registrar o asistir un pedido B2B validando cliente, condición comercial, disponibilidad de productos y seguimiento posterior | S1 — Commercial Coordination — Valeria Sánchez | Login → Dashboard comercial → Clientes → Detalle de cliente → Pedido asistido → Selección de productos → Resumen → Confirmación → Detalle de pedido → Reportes | Lucidchart S1 | El recorrido conecta la revisión comercial del cliente con la captura asistida del pedido y su seguimiento posterior, evitando que la coordinación dependa de mensajes dispersos |
| Supervisar inventario, lotes, riesgos FEFO, despacho, cierre operativo y reportes | S2 — Operations / Account Owner — Roberto García | Login → Dashboard logístico → Inventario general → Inventario por lote → Detalle de lote → Revisión operativa de pedido → Despacho → Registro de salida → Notificación → Confirmación → Reportes operativos | Lucidchart S2 y wireflow S2 documentado como figura | El recorrido conecta lectura de inventario, priorización FEFO, despacho y cierre simulado para sostener trazabilidad operativa |
| Consultar catálogo, enviar solicitud, revisar pedido y acceder a tracking/documentos visibles | S3 — B2B Buyer Portal — Elena Litano | Login → Portal Home → Product Catalog → Product Detail → Request Builder → My Requests → My Orders → Order Detail / Tracking → Business Documents | Flujo funcional documentado; wireflow visual pendiente | El recorrido representa la experiencia de autoservicio del comprador B2B y debe incorporarse como wireflow visual cuando el equipo actualice la evidencia |

*Figura. Wireflow principal para S2 — Operations / Account Owner*

![Wireflow S2 principal](../assets/images/chapter-4/webapp/wireflows/wireflow-s2-jefatura-logistica-coordinacion-operativa.png)

> *Nota.* El wireflow muestra la continuidad visual entre dashboard logístico, inventario, lote, despacho, confirmación y reportes operativos. Elaboración propia.

*Figura. Wireflow complementario para S2 — Operations / Account Owner*

![Wireflow S2 complementario](../assets/images/chapter-4/webapp/wireflows/wireflow-s2-jefatura-logistica-coordinacion-operativa-alt.png)

> *Nota.* Esta vista complementa el recorrido S2 con una variante de lectura del flujo operativo disponible en los artefactos actualizados. Elaboración propia.

> *Pendiente:* Agregar wireflow de S3 cuando el Buyer Portal cuente con artefactos visuales exportados.

### 4.4.3. Web Applications Mock-ups

Los mockups representan pantallas seleccionadas de alta fidelidad para la dirección visual de la Web Application. Se agrupan por segmento y user goal para mostrar evidencia visual sin convertir el capítulo en una galería extensa. La evidencia visual disponible cubre S1 y S2. Para S3, se documenta la cobertura funcional del Buyer Portal y se deja pendiente la incorporación de mockups exportados.

| Grupo de mockups | Segmento | User goal | Pantallas incluidas | Propósito |
|---|---|---|---|---|
| S1 — Commercial Coordination | Valeria / S1 | Crear y seguir un pedido asistido | Login, dashboard, cliente, pedido, detalle, reportes | Evidenciar captura comercial guiada, validaciones y trazabilidad |
| S2 — Operations / Account Owner | Roberto / S2 | Controlar inventario, despacho y POD mock | Dashboard, inventario, lote, despacho, POD mock, reportes | Evidenciar monitoreo FEFO, operación logística y cierre simulado |
| S3 — B2B Buyer Portal | Elena / S3 | Comprar y hacer seguimiento desde portal B2B | Mockups pendientes de incorporación | Evitar declarar capturas inexistentes y dejar trazabilidad del pendiente visual |

#### S1 — Commercial Coordination: mockups de pedido asistido

![S1 Login Valeria selected](../assets/images/chapter-4/webapp/mockups/s1-01-login-valeria-selected.png)

![S1 Dashboard coordinación comercial](../assets/images/chapter-4/webapp/mockups/s1-02-dashboard-commercial.png)

![S1 Client detail drawer](../assets/images/chapter-4/webapp/mockups/s1-04-client-detail-drawer.png)

![S1 Assisted order products step](../assets/images/chapter-4/webapp/mockups/s1-07-assisted-order-products-step.png)

![S1 Order detail created by Valeria](../assets/images/chapter-4/webapp/mockups/s1-10-order-detail-created-by-valeria.png)

![S1 Reportes coordinación comercial](../assets/images/chapter-4/webapp/mockups/s1-12-commercial-reports.png)

> *Nota:* Este grupo muestra el recorrido comercial desde la selección de perfil hasta la evidencia de pedido y reportes. Las pantallas se eligieron porque cubren los puntos decisivos del user goal: acceso por rol, lectura de estado, revisión de cliente, armado de pedido, trazabilidad por creador y análisis comercial. Elaboración propia.

#### S2 — Operations / Account Owner: mockups de operación logística

![S2 Dashboard jefatura logística](../assets/images/chapter-4/webapp/mockups/s2-02-dashboard-logistics.png)

![S2 Inventory overview](../assets/images/chapter-4/webapp/mockups/s2-03-inventory-overview.png)

![S2 Lot detail drawer](../assets/images/chapter-4/webapp/mockups/s2-05-lot-detail-drawer.png)

![S2 Dispatch board](../assets/images/chapter-4/webapp/mockups/s2-07-dispatch-board.png)

![S2 POD mock modal](../assets/images/chapter-4/webapp/mockups/s2-09-pod-mock-modal.png)

![S2 Operational reports](../assets/images/chapter-4/webapp/mockups/s2-12-operational-reports.png)

> *Nota.* Este grupo resume el recorrido operativo desde monitoreo hasta cierre simulado de entrega. Las pantallas seleccionadas cubren dashboard, inventario, lote, despacho, POD mock y reportes operativos, que son las evidencias visuales más representativas del flujo S2. Elaboración propia.

#### S3 — B2B Buyer Portal: mockups pendientes de incorporación

El Buyer Portal forma parte de la Web Application y responde al flujo de S3. Su experiencia debe mostrar catálogo, detalle de producto, constructor de solicitud, solicitudes, pedidos, documentos y perfil del comprador. Sin embargo, esta subsección no agrega imágenes porque los assets visuales de S3 no están incluidos en el reporte actual.

### 4.4.4. Web Applications User Flow Diagrams

#### Criterios de resolución de flujo

Para mantener trazabilidad entre investigación, diseño e implementación, los recorridos de la Web Application se documentan en cuatro niveles: User Goal, Task Flow, Wireflow y User Flow. La lectura se mantiene por segmento para no mezclar responsabilidades entre coordinación comercial, operaciones/account owner y comprador B2B.

*Tabla: Niveles de resolución de flujo aplicados en Nexa*

| Nivel | Aplicación en Nexa | Evidencia en esta sección |
|---|---|---|
| **User Goal** | Objetivo operativo de cada persona dentro del flujo B2B refrigerado | Objetivos de S1, S2 y S3 derivados del needfinding |
| **Task Flow** | Secuencia de acciones necesarias para completar solicitud, validación, despacho o seguimiento | Tabla por segmento |
| **Wireflow** | Continuidad visual entre pantallas de la Web Application | Lucidchart S1, Lucidchart S2 y figuras de wireflow S2 |
| **User Flow** | Decisiones, rutas alternativas y estados del recorrido | Diagramas visuales Lucidchart para S1/S2 y flujo documentado para S3 |

*Tabla: User Goals, Task Flows y referencias de flujo por segmento*

| Segmento | Persona | User Goal | Resumen de task flow | Wireflow | User Flow |
|---|---|---|---|---|---|
| S1 — Commercial Coordination | Valeria Sánchez | Registrar o asistir un pedido B2B validando cliente, condición comercial, disponibilidad de productos y seguimiento posterior | Login — perfil Valeria → Dashboard comercial → Clientes → Detalle de cliente → Validación de condición comercial → Pedido asistido → Selección de productos → Validación de disponibilidad → Confirmación del pedido → Detalle y seguimiento del pedido → Reportes comerciales | [Wireflow S1 en Lucidchart](https://lucid.app/lucidchart/4aeb3b33-353d-4b0c-b978-5bed19d4fdca/edit?viewport_loc=-11%2C-11%2C3028%2C1465%2C0_0&invitationId=inv_c95b5cdc-7bd7-46ad-aa88-0fa213649397) | Userflow S1 en Lucidchart |
| S2 — Operations / Account Owner | Roberto García | Supervisar inventario, lotes, riesgos FEFO, despacho, cierre operativo, evidencias y administración de empresa | Login — perfil Roberto → Dashboard operativo → Inventario → Detalle de lote → Revisión FEFO y stock → Priorización operativa → Tablero de despacho → Confirmación de despacho → POD mock → Validación de evidencia → Reportes operativos → Company Administration si corresponde | [Wireflow S2 en Lucidchart](https://lucid.app/lucidchart/6573c628-5545-4360-8fb2-3bb444c7e648/edit?viewport_loc=-298%2C-263%2C3315%2C1788%2C0_0&invitationId=inv_5e548793-b34d-43ed-b8fc-0f9dd7cf81a5) | Userflow S2 en Lucidchart |
| S3 — B2B Buyer Portal | Elena Litano | Consultar catálogo, enviar solicitud, revisar pedidos, acceder a documentos y seguir el estado del despacho con mayor autonomía | Login — perfil Elena → Portal Home → Product Catalog → Product Detail → Request Builder → My Requests → My Orders → Order Detail / Tracking → Business Documents | Pendiente de wireflow visual | Flujo comprador documentado en Mermaid como placeholder técnico |

> *Nota:* Los user goals provienen de la síntesis complementaria de Needfinding. S1 y S2 están respaldados con mockups y evidencia visual disponible. S3 está respaldado por la estructura funcional del Buyer Portal, pero requiere incorporación de wireframes, wireflows y mockups visuales en el reporte.

#### User Flow S1 — Commercial Coordination: validación y pedido asistido

El user flow de S1 representa el recorrido de Valeria, responsable de coordinación comercial, desde el acceso al sistema hasta la creación y seguimiento de un pedido asistido. El flujo incluye validaciones de condición comercial, disponibilidad de productos y rutas alternativas para restricciones de cliente o cantidad insuficiente.

[Ver userflow S1 en Lucidchart](https://lucid.app/lucidchart/8f6d6af2-f229-47f8-ba02-86b27cdc6fed/edit?invitationId=inv_09391266-7e11-4614-8edf-12cf979cdabf)

![S1 User flow coordinación comercial](../assets/images/chapter-4/webapp/user-flows/s1-commercial-userflow-lucid.png)

Figura. User flow visual para S1 — Commercial Coordination.

#### User Flow S2 — Operations / Account Owner: inventario, despacho y cierre

El user flow de S2 representa el recorrido de Roberto, responsable de operaciones y cuenta, desde la revisión de inventario y lotes con criterio FEFO hasta la gestión de despacho y cierre con POD simulado. El flujo incluye rutas alternativas para riesgo operativo, despacho no listo, evidencia incompleta y administración de empresa cuando corresponde al account owner.

[Ver userflow S2 en Lucidchart](https://lucid.app/lucidchart/b91c8e98-a38b-456a-92e5-f942be7e8439/edit?invitationId=inv_5c030713-67e5-4e84-90bf-661b26cef528)

![S2 User flow jefatura logística](../assets/images/chapter-4/webapp/user-flows/s2-logistics-userflow-lucid.png)

Figura. User flow visual para S2 — Operations / Account Owner.

#### User Flow S3 — B2B Buyer Portal: solicitud, pedido y seguimiento

El user flow de S3 representa el recorrido de Elena como compradora B2B. El flujo conecta catálogo, detalle de producto, request builder, solicitudes, pedidos confirmados, documentos visibles y tracking. Este flujo debe convertirse en wireflow visual y mockups cuando se actualicen los assets del reporte.

```mermaid
flowchart LR
    A["S3 — B2B Buyer Portal"] --> B["Login"]
    B --> C["Portal Home"]
    C --> D["Product Catalog"]
    D --> E["Product Detail"]
    E --> F["Request Builder"]
    F --> G["Submit Request"]
    G --> H["My Requests"]
    H --> I{"Request confirmed?"}
    I -->|"No"| J["Review status or comments"]
    I -->|"Yes"| K["My Orders"]
    K --> L["Order Detail / Tracking"]
    L --> M["Business Documents"]
```

Figura. User flow documentado para S3 — B2B Buyer Portal. Elaboración propia.

#### Tabla de consistencia: User Goals, wireflows y user flows

| User goal | Persona | Wireflow | User flow | Evidencia visual | Estado documental |
|---|---|---|---|---|---|
| Registrar pedido asistido validando cliente, condición comercial y disponibilidad de producto | Valeria Sánchez (S1) | [Wireflow S1 en Lucidchart](https://lucid.app/lucidchart/4aeb3b33-353d-4b0c-b978-5bed19d4fdca/edit?viewport_loc=-11%2C-11%2C3028%2C1465%2C0_0&invitationId=inv_c95b5cdc-7bd7-46ad-aa88-0fa213649397) | Userflow S1 en Lucidchart | Lucidchart + mockups S1 seleccionados | Documentado con evidencia visual |
| Supervisar inventario FEFO, coordinar despacho, cerrar entrega con POD mock y administrar empresa/tenant cuando corresponde | Roberto García (S2) | [Wireflow S2 en Lucidchart](https://lucid.app/lucidchart/6573c628-5545-4360-8fb2-3bb444c7e648/edit?viewport_loc=-298%2C-263%2C3315%2C1788%2C0_0&invitationId=inv_5e548793-b34d-43ed-b8fc-0f9dd7cf81a5) + figura de wireflow S2 | Userflow S2 en Lucidchart | Lucidchart + mockups S2 seleccionados | Documentado con evidencia visual |
| Explorar catálogo, enviar solicitud, revisar pedidos, documentos y tracking desde Buyer Portal | Elena Litano (S3) | Pendiente de wireflow visual | User flow documentado en Mermaid | Pendiente de wireframes/mockups exportados | Pendiente de actualización con evidencia real |

> *Nota:* Esta sección evita afirmar capturas o wireflows que todavía no están en los assets del reporte. La actualización posterior agregará evidencia visual real de S3, sin crear un segmento Admin separado y manteniendo S2 como responsable de administración, configuración y tenant.
