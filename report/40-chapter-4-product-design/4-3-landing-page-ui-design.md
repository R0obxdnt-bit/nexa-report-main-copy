## 4.3. Landing Page UI Design

La Landing Page es la superficie pública de entrada al ecosistema Nexa. Su función principal es comunicar la propuesta de valor, explicar el problema operativo que resuelve la plataforma, segmentar visitantes por tipo de operación y dirigirlos hacia una demostración, contacto comercial o acceso autenticado al producto.

Esta sección traduce las decisiones definidas en **4.1 Style Guidelines** y **4.2 Information Architecture** hacia una propuesta visual concreta. La Landing Page no replica las pantallas internas de la Web Application ni del Buyer Portal; su objetivo es presentar el valor de Nexa con una narrativa clara, jerarquía visual consistente, CTAs visibles, lenguaje profesional y adaptación responsive.

La referencia pública de implementación de la Landing Page se encuentra en: [https://upc-pre-202610-1asi0730-12242-king.github.io/nexa-website/](https://upc-pre-202610-1asi0730-12242-king.github.io/nexa-website/).

> *Nota:* La evidencia formal de despliegue, ejecución y validación debe documentarse en el Capítulo V. Esta sección se concentra en la propuesta UI, wireframes y mockups de la Landing Page.

Cada elemento del sitio público mantiene continuidad con alguna capacidad del producto, pero sin inventar flujos que todavía no estén implementados. Las páginas de **Solutions** funcionan como rutas comerciales para empresas interesadas; no reemplazan los segmentos funcionales del producto. Los segmentos operativos definitivos siguen siendo **S1 — Commercial Coordination**, **S2 — Operations / Account Owner** y **S3 — B2B Buyer Portal**.

| Elemento de la Landing Page | Intención de diseño | Continuidad en el producto | Superficie relacionada |
|---|---|---|---|
| CTA `Request a demo` / `Solicitar una demostración` | Convertir el interés del visitante en contacto comercial | Contacto guiado, revisión de operación y explicación del demo | Landing Page / Company contact |
| CTA `Log in` / `Ingresar` | Permitir acceso a usuarios autenticados | Entrada al sistema mediante login | `#/auth/login` |
| Home | Presentar el problema, la promesa de valor y el recorrido principal | Introduce el flujo transversal: S3 solicita, S1 valida y S2 ejecuta | Landing Page |
| Platform | Explicar capacidades de catálogo, pedidos, inventario, despacho y trazabilidad | Conecta la propuesta pública con dashboards y módulos internos | `/ops/commercial/dashboard`, `/ops/operations/dashboard`, `/portal/home` |
| Solutions Hub | Segmentar la comunicación por tipo de empresa interesada | Permite que importadores, distribuidores y operadores de almacenamiento entiendan el valor según su operación | Landing Page |
| Importers & Wholesalers | Comunicar valor para operaciones con abastecimiento, stock y lotes | Relaciona validación comercial, disponibilidad e inventario | `/ops/commercial/purchase-requests`, `/ops/operations/inventory-control` |
| Distributors | Comunicar el flujo principal de pedido B2B, FEFO, despacho y evidencia | Relaciona Buyer Portal, purchase requests, purchase orders y dispatch orders | `/portal/product-catalog`, `/ops/commercial/purchase-requests`, `/ops/operations/dispatch-orders` |
| Cold Storage Operators | Comunicar control de almacenamiento, trazabilidad y operación refrigerada | Relaciona inventario, lotes, analítica operativa y monitoreo como alcance progresivo | `/ops/operations/inventory-control`, `/ops/operations/operational-analytics` |
| Company | Generar confianza y presentar el contexto del equipo | Refuerza credibilidad antes del contacto comercial | Landing Page |
| FAQ | Reducir fricción antes de solicitar una demostración | Responde dudas sobre implementación, seguridad, datos, alcance y roadmap | Landing Page |
| Footer / Contact support | Ofrecer canales de contacto y navegación de soporte | Facilita acceso a email, contacto, FAQ y soluciones | Landing Page |

### Decisiones UI aplicadas en la Landing Page

| Decisión de diseño | Aplicación en la Landing Page | Relación con arquitectura de información |
|---|---|---|
| Jerarquía visual | Hero con mensaje principal, subtítulo, CTAs y bloques de valor | Prioriza comprensión rápida antes de navegación profunda |
| Navegación global | Navbar con acceso a Platform, Solutions, Company, FAQ y CTAs | Refuerza el sistema de navegación definido en 4.2 |
| Segmentación comercial | Solutions organiza rutas para importadores, distribuidores y operadores de cámaras frías | Permite explicar la propuesta por tipo de empresa interesada |
| Consistencia visual | Uso de colores, tipografía, cards, botones y espaciado definidos en 4.1 | Mantiene continuidad con el Design System de Nexa |
| Diseño inclusivo | Texto legible, contraste, CTAs identificables, labels claros y navegación simple | Reduce fricción para visitantes con distintos niveles de familiaridad tecnológica |
| Responsive design | Adaptación de hero, navegación, cards y secciones a una lectura vertical en mobile | Permite que la experiencia pública funcione en desktop y mobile |
| Continuidad con producto | CTAs y mensajes conectan con login, demo, catálogo, solicitudes, pedidos e inventario | Evita que la Landing Page sea un artefacto aislado |

### 4.3.1. Landing Page Wireframe

La Landing Page de Nexa se trabajó primero en **Figma** mediante wireframes de baja fidelidad. En esta etapa se ordenaron contenido, jerarquía de secciones, navegación, rutas por tipo de visitante y puntos de conversión antes de pasar a mockups de mayor detalle.

Los wireframes permiten validar la arquitectura de información sin distraer la revisión con colores, imágenes o estilos finales. La prioridad fue comprobar que el visitante pueda entender el problema, reconocer el tipo de operación al que pertenece, revisar la plataforma y encontrar una vía clara de contacto o acceso.

La revisión se hizo para **Desktop Web Browser** y **Mobile Web Browser**, manteniendo la misma lógica de lectura: propuesta de valor, explicación de capacidades, segmentación comercial, confianza y conversión.

#### A. Desktop Web Browser

| Wireframe | Propósito de validación |
|---|---|
| Home | Validar la jerarquía inicial: problema, propuesta de valor, CTA y bloques principales |
| Platform | Validar la explicación funcional de la plataforma sin entrar a pantallas autenticadas |
| Solutions Hub | Validar la separación de rutas comerciales por tipo de operación |
| Company | Validar confianza, contexto del equipo y acceso al contacto |
| Distributors | Validar la comunicación del flujo principal B2B: pedido, inventario, despacho y evidencia |
| Importers & Wholesalers | Validar el mensaje para operaciones con abastecimiento, stock y lotes |
| FAQ | Validar agrupación de dudas frecuentes y reducción de fricción previa al contacto |

*Figura. Wireframe desktop de Home*

![Wireframe desktop de Home](../assets/images/chapter-4/landing/wireframes/desktop/home-wireframe.jpg)

> *Nota:* La portada organiza hero, propuesta principal, CTA y primeros bloques de valor para un visitante que llega por primera vez al sitio. Elaboración propia.

*Figura. Wireframe desktop de Platform*

![Wireframe desktop de Platform](../assets/images/chapter-4/landing/wireframes/desktop/platform-wireframe.jpg)

> *Nota:* La página Platform ordena módulos, beneficios funcionales y lectura general de la solución sin entrar todavía a pantallas autenticadas. Elaboración propia.

*Figura. Wireframe desktop de Solutions*

![Wireframe desktop de Solutions](../assets/images/chapter-4/landing/wireframes/desktop/solutions-wireframe.jpg)

> *Nota:* El hub de Solutions separa rutas públicas para visitantes interesados en distribución, importación, mayoristas y cámaras frías. Elaboración propia.

*Figura. Wireframe desktop de Company*

![Wireframe desktop de Company](../assets/images/chapter-4/landing/wireframes/desktop/company-wireframe.jpg)

> *Nota:* La página Company da contexto institucional al proyecto, presenta confianza y mantiene una vía clara hacia el contacto comercial. Elaboración propia.

*Figura. Wireframe desktop de Distribuidores*

![Wireframe desktop de Distribuidores](../assets/images/chapter-4/landing/wireframes/desktop/distributors-wireframe.jpg)

> *Nota:* La ruta para distribuidores enfatiza coordinación de pedidos, visibilidad operativa, despacho y continuidad de atención. Elaboración propia.

*Figura. Wireframe desktop de Importadores*

![Wireframe desktop de Importadores](../assets/images/chapter-4/landing/wireframes/desktop/importers-wireframe.jpg)

> *Nota:* La ruta para importadores y mayoristas prioriza abastecimiento, disponibilidad, lotes e inventario para operaciones B2B. Elaboración propia.

*Figura. Wireframe desktop de FAQ*

![Wireframe desktop de FAQ](../assets/images/chapter-4/landing/wireframes/desktop/faq-wireframe.jpg)

> *Nota:* La página FAQ organiza dudas frecuentes sobre acceso, uso, alcance del producto, seguridad, implementación y contacto comercial. Elaboración propia.

#### B. Mobile Web Browser

La versión móvil conserva la misma secuencia pública, pero reduce densidad visual y concentra navegación, lectura de propuesta y CTA en una estructura vertical más compacta. La prioridad mobile es que el visitante pueda comprender rápidamente qué hace Nexa, acceder al menú, revisar el mensaje principal y llegar al CTA sin depender de una pantalla amplia.

| Criterio mobile | Aplicación esperada |
|---|---|
| Navegación | Menú colapsado con acceso a rutas principales |
| Lectura | Secciones en stack vertical con títulos breves |
| CTA | Botones visibles y con área táctil suficiente |
| Jerarquía | Hero, problema, solución y contacto en orden progresivo |
| Accesibilidad | Contraste, labels claros y elementos interactivos reconocibles |

*Figura. Wireframe mobile de Home*

![Wireframe mobile de Home](../assets/images/chapter-4/landing/wireframes/mobile/home-wireframe.jpg)

> *Nota:* La versión móvil concentra hero, navegación compacta, bloques principales y cierre comercial en una lectura continua. Elaboración propia.

### 4.3.2. Landing Page Mock-up

Una vez validada la estructura, los mockups se desarrollaron en **Figma** para fijar tratamiento visual, jerarquía de botones, ritmo de secciones, color, tipografía e identidad de marca. Los mockups aplican el Design System definido en 4.1 y respetan la arquitectura de información descrita en 4.2.

Las capturas corresponden al recorrido principal en **Desktop Web Browser** y a una muestra de adaptación para **Mobile Web Browser**. En esta etapa se valida la apariencia final de la Landing Page: uso de color, tipografía, espaciado, contraste, cards, CTAs, bloques informativos y consistencia visual entre páginas.

#### A. Desktop Web Browser

| Mockup | Criterio UI validado |
|---|---|
| Home | Mensaje principal, CTA, jerarquía editorial y cierre de conversión |
| Platform | Explicación de capacidades mediante módulos y bloques visuales |
| Company | Confianza, presentación del equipo y soporte de contacto |
| Distributors | Flujo de pedido B2B, FEFO, despacho y visibilidad operativa |
| Importers & Wholesalers | Abastecimiento, lotes, disponibilidad e inventario |
| Cold Storage Operators | Comunicación de almacenamiento, control y trazabilidad refrigerada |
| FAQ | Lectura rápida de dudas frecuentes y reducción de fricción |

*Figura. Mockup desktop de Home*

![Mockup desktop de Home](../assets/images/chapter-4/landing/mockups/desktop/home.jpg)

> *Nota:* Home presenta el mensaje principal, CTA, bloques de capacidades y cierre del recorrido público. Elaboración propia.

*Figura. Mockup desktop de Platform*

![Mockup desktop de Platform](../assets/images/chapter-4/landing/mockups/desktop/platform.jpg)

> *Nota:* Platform muestra la propuesta funcional del producto mediante módulos, beneficios operativos y lectura de plataforma. Elaboración propia.

*Figura. Mockup desktop para operadores de cámaras frías*

![Mockup desktop para operadores de cámaras frías](../assets/images/chapter-4/landing/mockups/desktop/cold-storage-operators.jpg)

> *Nota:* La variante para cámaras frías comunica control, almacenamiento y trazabilidad de productos sensibles, separando el alcance actual de integraciones futuras. Elaboración propia.

*Figura. Mockup desktop de Company*

![Mockup desktop de Company](../assets/images/chapter-4/landing/mockups/desktop/company.jpg)

> *Nota:* Company refuerza el contexto del proyecto y la confianza necesaria antes de iniciar contacto comercial. Elaboración propia.

*Figura. Mockup desktop para distribuidores*

![Mockup desktop para distribuidores](../assets/images/chapter-4/landing/mockups/desktop/distributors.jpg)

> *Nota:* La ruta para distribuidores enfatiza pedido, coordinación, visibilidad operativa y continuidad de atención B2B. Elaboración propia.

*Figura. Mockup desktop para importadores y mayoristas*

![Mockup desktop para importadores y mayoristas](../assets/images/chapter-4/landing/mockups/desktop/importers-wholesalers.jpg)

> *Nota:* La ruta para importadores y mayoristas adapta la propuesta a operaciones con dependencia de abastecimiento, lotes y disponibilidad de stock. Elaboración propia.

*Figura. Mockup desktop de FAQ*

![Mockup desktop de FAQ](../assets/images/chapter-4/landing/mockups/desktop/faq.jpg)

> *Nota:* FAQ reduce fricción previa al contacto mediante respuestas breves, agrupación temática y navegación directa. Elaboración propia.

#### B. Mobile Web Browser

La adaptación móvil mantiene el mismo lenguaje visual del sitio público y prioriza lectura vertical, CTA visible, navegación compacta y bloques más breves para consulta desde teléfono. Esta vista valida que la identidad visual de Nexa no dependa exclusivamente del formato desktop.

| Criterio UI mobile | Aplicación en el mockup |
|---|---|
| Hero compacto | Mensaje principal y CTA visibles al inicio |
| Secciones apiladas | Cards y bloques reordenados en una sola columna |
| Navegación táctil | Menú compacto y botones con mayor área de interacción |
| Continuidad visual | Mismos colores, tipografía y estilo de cards que desktop |
| Claridad | Menor densidad textual y mayor separación entre bloques |

*Figura. Mockup mobile de Home*

![Mockup mobile de Home](../assets/images/chapter-4/landing/mockups/mobile/home.jpg)

> *Nota:* La captura móvil valida hero, navegación compacta, secciones principales y cierre de contacto en una experiencia responsiva. Elaboración propia.
