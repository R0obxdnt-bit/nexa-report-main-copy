## 4.5. Web Applications Prototyping.

El prototipado de las aplicaciones web de Nexa permite validar la navegación, interacción y continuidad visual de las superficies autenticadas antes de analizar su implementación. Esta sección documenta el prototipo de la **Web Application interna** para **S1 — Commercial Coordination** y **S2 — Operations / Account Owner**, así como el alcance esperado del **Buyer Portal** para **S3 — B2B Buyer Portal**.

El prototipo se relaciona directamente con la arquitectura de información definida en la sección 4.2 y con los user flows documentados en la sección 4.4. Por ello, la navegación no se organiza solo por pantallas, sino por responsabilidades de negocio: S3 consulta catálogo y envía solicitudes, S1 valida comercialmente y convierte solicitudes en órdenes de compra, y S2 ejecuta inventario, despacho, evidencias y administración de empresa/tenant.

El prototipado constituye **evidencia de diseño interactivo**, no evidencia de despliegue productivo ni de backend real. La evidencia de implementación, ejecución, despliegue y uso de Fake API debe mantenerse en el Capítulo V.

> *Nota de alcance documental:* la evidencia visual disponible en esta sección cubre principalmente los recorridos S1 y S2. El Buyer Portal de S3 forma parte de la Web Application, pero requiere incorporación posterior de screenshot de video y enlace específico de prototipo cuando el equipo genere o exporte esa evidencia. No se agregan capturas ni videos inexistentes.

*Tabla. Criterios aplicados para las decisiones de interacción del prototipo*

| Criterio | Aplicación en Nexa | Relación con arquitectura de información |
|---|---|---|
| Navegación por responsabilidad | S1, S2 y S3 acceden a módulos distintos según su rol y scope | Refuerza la separación entre Commercial Coordination, Operations / Account Owner y Buyer Portal |
| Continuidad de flujo | Los recorridos conectan login, dashboard, entidades de negocio, detalle y confirmación | Evita que las pantallas funcionen como vistas aisladas |
| Progressive disclosure | Los detalles se muestran mediante drawers, modales, pasos guiados o vistas de detalle | Reduce carga cognitiva y mantiene contexto operativo |
| Feedback de estado | Badges, confirmaciones y mensajes permiten entender el avance de solicitudes, pedidos y despachos | Comunica trazabilidad sin depender solo del color |
| Densidad adaptada | La Web Application interna prioriza desktop/tablet por volumen operativo; el Buyer Portal debe priorizar claridad en desktop y mobile | Responde a diferencias de uso entre usuarios internos y compradores B2B |
| Consistencia visual | Se mantienen colores, tipografía, botones, tablas, cards y estados definidos en 4.1 | Asegura continuidad entre diseño visual y prototipo interactivo |

*Tabla. Artefactos de prototipado y evidencia disponible*

| Evidencia de prototipado | Propósito | Estado documental |
|---|---|---|
| [Proyecto Figma del equipo](https://www.figma.com/files/team/1586383034175281439/project/587167294) | Espacio maestro con wireframes, mockups y decisiones visuales del equipo | Disponible |
| [Archivo Figma de la Web Application](https://www.figma.com/design/buDa5VZmYjPNokbl4FEJqx/Web-App?node-id=0-1) | Prototipo navegable con frames conectados de la aplicación | Disponible |
| [Video del prototipo — Web y Móvil](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202323040_upc_edu_pe/IQAOXrLcl2ziRpTDa5QgX__QARetYOg71_XS5G2YR84vlVs?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=MTgzyN) | Recorrido audiovisual del prototipo presentado para TB1 | Disponible como enlace de video; pendiente confirmar publicación final en Microsoft Stream si el docente lo exige explícitamente |
| [FigJam — Userflow y Wireflow S1/S2](https://www.figma.com/board/LjIjtyfoOpeYa5OCSJUYpD/Nexa-Ops-S1-S2-Userflow-Wireflow?node-id=0-1&t=F9ZnAAAzCUpiK4qs-1) | Board de trabajo para validar rutas, flujos y decisiones de interacción | Disponible para S1/S2 |
| Screenshot de video para Web Application interna | Captura de evidencia audiovisual del prototipo | Disponible en esta sección |
| Screenshot de video para Buyer Portal S3 | Evidencia audiovisual específica del portal comprador | Pendiente de actualización con evidencia real |
| Screenshot de Mobile Web Browser para Web Application | Evidencia responsive específica de la aplicación autenticada | Pendiente de actualización con evidencia real |

> *Nota:* El archivo de imagen mobile disponible en la carpeta de prototyping corresponde visualmente a la Landing Page mobile, por lo que no se utiliza como evidencia de Web Applications Prototyping. Debe incorporarse una captura mobile real de la Web Application o del Buyer Portal cuando exista evidencia verificable.

*Tabla. Cobertura de prototipado por flujo y segmento*

| Flujo | Segmento | Cobertura en prototipo | Evidencia | Estado documental |
|---|---|---|---|---|
| Validación y pedido asistido | S1 — Commercial Coordination | Dashboard comercial, clientes, detalle de cliente, pedido asistido, selección de productos, detalle de pedido y reportes | Figma, FigJam y userflow S1 | Documentado con evidencia visual disponible |
| Inventario, despacho y cierre operativo | S2 — Operations / Account Owner | Dashboard operativo, inventario, lotes, despacho, registro de salida, POD mock y reportes operativos | Figma, FigJam, wireflow y userflow S2 | Documentado con evidencia visual disponible |
| Catálogo, solicitud, pedido y seguimiento | S3 — B2B Buyer Portal | Home, catálogo, detalle de producto, request builder, solicitudes, pedidos, documentos y perfil | Flujo funcional definido en 4.2 y 4.4 | Pendiente de screenshot de video y prototipo visual específico |

*Captura referencial del prototipo de la Web Application interna*

![Captura del prototipo de la web application](../assets/images/chapter-4/webapp/prototyping/prototyping.jpeg)

> *Nota:* Captura del video de prototipo mostrando la sección de clientes y el drawer de perfil del cliente dentro del flujo S1. Elaboración propia.

### 4.5.1. Sistema de navegación aplicado al prototipo

El prototipo aplica un sistema de navegación diferenciado por superficie y responsabilidad de negocio. La **Web Application interna** utiliza navegación lateral persistente, top bar y vistas de detalle para que S1 y S2 puedan trabajar con información operativa sin perder contexto. El **Buyer Portal** debe utilizar una navegación más simple, orientada a catálogo, solicitudes, pedidos, documentos y perfil del comprador.

| Superficie | Segmento | Navegación principal | Propósito |
|---|---|---|---|
| Web Application interna | S1 — Commercial Coordination | Dashboard comercial, catálogo, purchase requests, purchase orders, manual order entry, client accounts y business documents | Validar solicitudes, revisar clientes, crear o convertir pedidos y gestionar documentos comerciales |
| Web Application interna | S2 — Operations / Account Owner | Dashboard operativo, inventory control, inventory lots, dispatch orders, proof of delivery, operational analytics, promotions, customer portals y company administration | Controlar inventario, lotes, despacho, evidencias, operación y configuración de empresa/tenant |
| Buyer Portal | S3 — B2B Buyer Portal | Home, product catalog, request builder, my requests, my orders, business documents, premium y profile | Permitir autoservicio del comprador para solicitar productos, revisar pedidos, documentos y tracking |

La navegación es **role-aware**: el usuario autenticado accede a una experiencia según su perfil y scope. S1 y S2 comparten la consola interna, pero no necesariamente comparten la misma prioridad de módulos. S3 utiliza el Buyer Portal como superficie separada para evitar exposición innecesaria de información operativa interna.

### 4.5.2. Interacciones principales del prototipo

El prototipo utiliza patrones de interacción consistentes con la arquitectura de información y los user flows. Las interacciones no se plantean como animaciones decorativas, sino como respuestas a decisiones del negocio: validar un cliente, confirmar productos, revisar disponibilidad, despachar una orden o consultar un estado.

| Patrón de interacción | Uso en el prototipo | Segmento |
|---|---|---|
| Login con selección de experiencia | Permite entrar a la superficie correspondiente según usuario autenticado | S1, S2, S3 |
| Dashboard inicial | Resume actividad relevante y accesos frecuentes | S1, S2, S3 |
| Tablas con filtros | Permiten revisar solicitudes, clientes, pedidos, lotes y despachos | S1, S2 |
| Drawers de detalle | Muestran información contextual sin abandonar la vista principal | S1, S2 |
| Flujo guiado por pasos | Permite construir o revisar una solicitud/pedido antes de confirmar | S1, S3 |
| Estados visuales | Comunican avance de solicitud, pedido, inventario o despacho | S1, S2, S3 |
| Confirmaciones | Reducen errores antes de registrar cambios importantes | S1, S2, S3 |
| Tracking y documentos visibles | Permiten al comprador consultar avance y soporte documental | S3 |

### 4.5.3. Paths de prototipo por user goal

Los paths del prototipo siguen los user flows definidos en 4.4. Cada recorrido cubre un objetivo de usuario y una secuencia de interacción esperada.

| Segmento | User goal | Path de prototipo | Estado |
|---|---|---|---|
| S1 — Commercial Coordination | Registrar o asistir un pedido B2B validando cliente, condición comercial y disponibilidad | Login → Commercial Dashboard → Client Accounts → Client Detail → Manual Order Entry → Product Selection → Order Summary → Purchase Order Detail → Commercial Reports | Evidencia visual disponible |
| S2 — Operations / Account Owner | Supervisar inventario, lotes, despacho, POD mock y reportes operativos | Login → Operations Dashboard → Inventory Control → Inventory Lots → Lot Detail → Dispatch Orders → Dispatch Detail → Proof of Delivery → Operational Analytics | Evidencia visual disponible |
| S3 — B2B Buyer Portal | Consultar catálogo, enviar solicitud, revisar pedidos, documentos y tracking | Login → Portal Home → Product Catalog → Product Detail → Request Builder → My Requests → My Orders → Order Detail / Tracking → Business Documents | Pendiente de prototipo visual específico |

### 4.5.4. Evidencia audiovisual requerida por aplicación

Para cumplir completamente con el criterio de prototipado, cada aplicación o superficie debe contar con screenshot de video y enlace al video donde se demuestre la navegación. La evidencia actual permite sustentar S1 y S2, pero debe completarse para S3 y para la demostración mobile específica de Web Application.

| Aplicación / superficie | Desktop Web Browser | Mobile Web Browser | Screenshot de video | Enlace de video | Estado |
|---|---|---|---|---|---|
| Web Application interna — S1/S2 | Disponible en prototipo | Pendiente de evidencia específica si no está cubierta en el video actual | Disponible | [Video del prototipo — Web y Móvil](https://upcedupe-my.sharepoint.com/:v:/g/personal/u202323040_upc_edu_pe/IQAOXrLcl2ziRpTDa5QgX__QARetYOg71_XS5G2YR84vlVs?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=MTgzyN) | Parcialmente completo |
| Buyer Portal — S3 | Pendiente de screenshot específico | Pendiente de screenshot específico | Pendiente | Pendiente de actualización con evidencia real | Pendiente |

> *Pendiente:* agregar un screenshot de video y enlace de prototipo para S3 — B2B Buyer Portal.

### 4.5.5. Relación entre prototipo, user flows e implementación

El prototipo se usa como puente entre diseño e implementación. Su función es demostrar que las rutas de navegación, módulos y decisiones de interacción son coherentes con los user goals definidos para cada segmento.

| Relación | Aplicación en Nexa |
|---|---|
| Information Architecture → Prototyping | Las rutas y módulos del prototipo siguen la organización por S1, S2 y S3 definida en 4.2 |
| User Flow → Prototyping | Los recorridos interactivos siguen los paths definidos en 4.4 |
| Design System → Prototyping | Las pantallas aplican colores, tipografía, componentes, estados y espaciado documentados en 4.1 |
| Prototyping → Implementation | La implementación debe respetar la navegación, estados y tareas validadas en prototipo, sin que esta sección funcione como evidencia de despliegue |
| Prototyping → Validation | Las pruebas con usuarios deben usar estos recorridos para evaluar claridad, navegación, accesibilidad e intención de uso |
