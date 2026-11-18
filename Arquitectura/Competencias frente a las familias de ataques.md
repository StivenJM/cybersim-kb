---
type: moc
status: propuesto
---
# Competencias frente a las familias de ataques

## Perfil de trabajo propuesto

Estudiante de ingeniería de software capaz de **analizar, corregir y verificar propiedades de seguridad de aplicaciones**, dentro de las familias seleccionadas y bajo condiciones explícitas de herramientas, documentación y ayuda. Puede comunicar evidencias, impacto e incertidumbre y justificar medidas de prevención.

Se adopta como especificación de trabajo el final de la carrera, con formación previa en programación, web, bases de datos, Git y los contenidos de seguridad correspondientes a las capacidades evaluadas. El propósito es comprobar el nivel que el estudiante ya puede demostrar. El pilotaje del instrumento y el nivel exigido se acuerdan con la institución antes de utilizar los resultados para aprobar o acreditar. Decir “ingeniero de software competente en tendencias actuales” sin esas precisiones deja indeterminado qué tareas debería resolver y con qué autonomía.

La frecuencia de amenazas es una entrada proporcionada por el compañero. Aquí no se certifica ese ranking ni se lo sustituye. Los CWE describen debilidades y relaciones técnicas; las ocho familias sirven para organizar cobertura, no como ocho dimensiones de competencia ya validadas.

## Competencias observables propuestas

| ID local | Capacidad integrada | Producto o actuación evaluable |
| --- | --- | --- |
| CAP-01 | Analizar activos, flujo de datos, actores y fronteras de confianza | Modelo o explicación de quién puede hacer qué y por qué |
| CAP-02 | Diagnosticar causalmente una debilidad y contrastarla con un caso legítimo | Evidencia ubicada, prueba discriminante y alcance de la conclusión |
| CAP-03 | Diseñar o aplicar una corrección coherente | Cambio de código, configuración, política o flujo verificable |
| CAP-04 | Verificar seguridad y continuidad funcional | Casos adversarios y benignos, resultados e interpretación |
| CAP-05 | Gestionar secretos y datos a lo largo de su ciclo de vida | Custodia, rotación, migración, inventario y límites de recuperación |
| CAP-06 | Preservar integridad y procedencia en la cadena de desarrollo/datos | Verificación de artefactos, permisos de publicación y prevención de recurrencia |
| CAP-07 | Razonar sobre confianza y capacidades de sistemas con IA | Separación de datos/instrucciones, entrenamiento/inferencia y permisos de herramientas |
| CAP-08 | Comunicar y priorizar una respuesta responsable | Hallazgos sustentados, decisión de contención, impacto y límites |

Son capacidades seleccionadas y adaptadas a partir de investigación publicada. El antecedente de nivel es [[Mead y Shoemaker - Competencias de aseguramiento de software]]; código, análisis, pruebas y comunicación se corresponden con [[Assyne - Estado de competencias de software]]; las tareas de estudiantes y los mecanismos técnicos completan el fundamento. La correspondencia por capacidad y sus límites están en [[Fundamento de las competencias de seguridad de CyberSim]]. No se atribuye a un solo paper una lista literal de ocho factores.

CAP-01–CAP-04 y CAP-08 describen actuaciones transversales; CAP-05 y CAP-06 especializan contenidos de seguridad. CAP-07 es una extensión para sistemas con IA que requiere formación previa explícita. Una evaluación del perfil base puede delimitarse sin esa extensión; si se anuncia cobertura de las ocho familias, deben administrarse también tareas de IA pertinentes. No observar IA no equivale automáticamente a fallar el perfil base.

D1–D4 son dimensiones de observación que cruzan las capacidades, no ocho notas nuevas ni una equivalencia con los niveles L1–L5 de un modelo profesional. Ni CAP ni D1–D4 son todavía escalas calibradas.

## Matriz de contenidos y evidencias

| Familia recibida | CWE | Desempeño que se debería observar | Evidencia mínima discriminante | Cobertura actual comprobada |
| --- | --- | --- | --- | --- |
| Cryptographic Failure | 327 | Identificar una elección criptográfica inadecuada según el uso y sustituirla | Riesgo explicado; cambio que preserva función y prueba del uso correcto | Sin caso dedicado comprobado en el conjunto investigativo |
| Cryptographic Failure | 319 | Localizar exposición durante tránsito y aplicar protección del canal | Captura/flujo sintético antes y después; verificación del receptor | Sin caso dedicado en el conjunto investigativo |
| Cryptographic Failure | 321 | Reconstruir exposición de clave y planificar recuperación | Historial, descifrado autorizado, migración y límites de copia histórica | AndinaPay; alcance parcial de CAP-02/04/05/08 |
| Injection | 89 | Separar consulta y datos; controlar identidad y permisos | Ataque deja de alterar semántica; consulta legítima sigue funcionando | BibliotecaViva |
| Injection | 79 | Aplicar tratamiento según contexto de salida | Entrada benigna conservada; ejecución indeseada impedida | Sin caso dedicado comprobado |
| Injection | 78 | Evitar interpretación indeseada por shell y acotar capacidades | Operación permitida funciona; argumento hostil no ejecuta otra acción | Sin caso dedicado comprobado |
| Insecure Design | 269 | Diseñar y aplicar privilegios mínimos adecuados | Acciones autorizadas y denegadas por identidad/capacidad | AndeanLogix toca autorización; no acredita cobertura completa de 269 |
| Insecure Design | 434 | Controlar admisión, almacenamiento y entrega de archivos | Carga legítima accesible a dueño; contenido peligroso o pendiente no publicado | TalentoAndino |
| Insecure Design | 602 | Trasladar al servidor el control relevante | Saltarse la interfaz no concede la acción | AndeanLogix incluye control solo UI como estado vulnerable; no instrumento completo dedicado |
| Security Misconfiguration | 284 | Definir y verificar políticas de acceso sobre recursos concretos | Matriz actor–acción–recurso y efectos observados | Cobertura relacionada en AndeanLogix; 284 es amplio |
| Security Misconfiguration | 306 | Exigir autenticación antes de funciones críticas | Petición anónima rechazada sin efecto; autorizada permitida | AndeanLogix |
| Security Misconfiguration | 918 | Controlar solicitudes del servidor y destinos efectivos | Petición legítima permitida; acceso a destino restringido impedido | Sin caso dedicado comprobado |
| Software and Data Integrity Failures | 502 | Preservar frontera al reconstruir datos no confiables | Validación antes de efectos; rechazo sin publicación parcial | NubeAndina |
| Software and Data Integrity Failures | 494 | Verificar código recibido antes de ejecutarlo/publicarlo | Artefacto auténtico aceptado; alterado no llega a ejecución | Sin caso dedicado comprobado |
| Software and Data Integrity Failures | 345 | Comprobar autenticidad y contexto autorizado | Manipulación detectada; mensaje auténtico pero no autorizado también rechazado | NubeAndina aporta contraste entre MAC y autoridad; cobertura parcial |
| Prompt Injection | 1427 | Distinguir contenido no confiable de instrucciones autorizadas | Datos hostiles no causan acción prohibida; tarea legítima permanece | Fuera de los cinco casos investigativos vigentes |
| Prompt Injection | 77 | Precisar si existe interpretación de comandos y corregir esa frontera | Prueba que identifica el intérprete y efecto evitado | No inferirlo de tener un chatbot; sin caso dedicado |
| Prompt Injection | 94 | Impedir que datos controlados se conviertan en código ejecutable no autorizado | Camino de datos a ejecución y contraste antes/después | No es sinónimo de 1427; sin caso dedicado |
| Training Data Poisoning | 20 | Controlar admisión de datos según esquema y semántica de la tarea | Datos legítimos conservados y contaminación detectada bajo supuestos explícitos | No equivale a cubrir poisoning completo; sin caso dedicado |
| Training Data Poisoning | 502 | Evitar reconstrucción insegura en ingestión de artefactos | Archivo/objeto de ingestión no produce efectos no autorizados | NubeAndina no observa una cadena de entrenamiento |
| Training Data Poisoning | 345 | Verificar origen/integridad y gobierno de datos/modelos | Procedencia y autorización comprobadas; datos contaminados excluidos o gestionados | Sin tarea de entrenamiento dedicada |
| Data Leakage | 200 | Identificar mecanismo, dato, actor y canal de exposición | Evidencia específica de acceso indebido y control que lo elimina | Efecto relacionado con AndinaPay; 200 es demasiado amplio para inferir cobertura total |
| Data Leakage | 359 | Analizar exposición de información privada de personas | Quién obtiene qué datos y por qué falta autorización | Sin caso dedicado comprobado |
| Data Leakage | 201 | Evitar incluir información sensible en datos enviados | Salida legítima conserva utilidad y omite información no autorizada | Sin caso dedicado comprobado |

“Sin caso dedicado comprobado” se refiere al conjunto investigativo de cinco casos revisado. El catálogo 3D legado contiene otros temas, pero su mera existencia no acredita evidencia comparable para estas competencias. Debe auditarse cada tarea antes de sumarla a la cobertura.

## Qué se deduce y qué no

La lista recibida contiene **24 entradas y 22 identificadores CWE distintos**: 502 y 345 aparecen en más de una familia. Ese solapamiento puede ser razonable, pero una misma actuación no debe contarse como dos observaciones independientes para declarar amplitud.

Los cinco casos vigentes cubren tareas específicas, no las ocho familias completas. No basta renombrar una tarjeta con otro CWE. Para ampliar cobertura se requieren nuevas situaciones y evidencias que obliguen a operar sobre el mecanismo de cada debilidad.

La tríada de IA exige distinguir: instrucciones maliciosas durante inferencia, contaminación durante entrenamiento y exposición de información. [[InjecAgent - Fronteras de instrucciones y datos]], [[AgentDojo - Seguridad y utilidad por separado]] y [[Poisoning - Datos de ajuste de instrucciones]] aportan antecedentes técnicos distintos. Sus benchmarks no validan la competencia del estudiante.

MITRE desaconseja usar CWE-200 para mapear vulnerabilidades concretas por su amplitud. Puede conservarse como tema organizativo recibido; el escenario debe especificar el mecanismo. La definición de CWE-1427 tampoco convierte automáticamente CWE-77/94 en subtipos de prompt injection. Véase [[Referencias institucionales de CyberSim]].

## Desarrollo recomendado de contenido

Primero cerrar la observabilidad y corrección de los cinco casos, con variantes. Luego ampliar según una matriz de necesidad y cobertura revisada por especialistas: control de canal/criptografía, XSS/comandos, SSRF, cadena de integridad, IA y exposición de datos. Este orden es de implementación propuesto por reutilización y brechas; no es un nuevo ranking científico de ataques.

Una sola tarea puede observar varias capacidades, pero el informe deberá mostrar qué evidencia respalda cada una y qué no se presentó. Para una decisión sobre el perfil: [[Del desempeño a la competencia del perfil]].

## Decisiones por mecanismo

No se adopta una defensa única de “sanitizar entradas”. SQL necesita separación consulta/datos; XSS depende del contexto de salida; comandos exigen evitar interpretación o limitar estrictamente la invocación. Autenticación no reemplaza autorización por recurso; integridad no equivale a autorización, ni firma del origen demuestra que su contenido sea benigno.

En SSRF se evalúa el destino efectivo y sus redirecciones, no una comparación textual superficial. En cargas se comprueban almacenamiento, entrega y ejecución, además del tipo admitido. En deserialización se observa si datos no confiables adquieren autoridad antes de validarse. Las pruebas concretas dependen del stack y del modelo del caso, sin exponer servicios reales durante la simulación.

En IA se necesitan tres situaciones distinguibles: contenido recuperado que intenta gobernar una herramienta, datos de entrenamiento cuya contaminación altera el comportamiento, y datos que salen a un destinatario no autorizado. Un ejemplo que extrae una flag no acredita prevención de poisoning ni protección de datos. Un sistema que rechaza todo también falla la utilidad legítima. El banco compara variantes de ataque y tareas benignas; las tasas del modelo no se convierten en nota del estudiante.

Las actitudes/responsabilidad se operacionalizan en elecciones observables: preservar evidencia, evitar divulgar secretos fuera del sandbox, justificar un límite de conclusión y comunicar riesgo. No se infiere una disposición estable de personalidad por un clic, ni se sustituye este componente por autoeficacia declarada.

La suficiencia del perfil se decide mediante [[Plan de cobertura del perfil]] y [[Del desempeño a la competencia del perfil]]. La selección de estas ocho familias proviene del encargo; la revisión no demuestra que sean las ocho de mayor frecuencia mundial al corte.
