---
type: decision
status: propuesto
---
# Plan de cobertura del perfil

Este plan especifica capacidades fundamentadas y adaptadas de la literatura para el perfil declarado. El origen de cada capacidad y la selección de Assyne se documentan en [[Fundamento de las competencias de seguridad de CyberSim]] y [[Correspondencia de competencias de Assyne con CyberSim]]. Las ocho etiquetas locales no se presentan como ocho factores descubiertos por un paper. Los IDs CAP-01 a CAP-08 distinguen capacidades de las comprobaciones técnicas C1-C5 de AndinaPay.

La referencia de población es un estudiante al final de la carrera con formación previa; no se homologa todo el plan al nivel L2 del modelo de aseguramiento. CAP-07 se administra como extensión de IA con prerrequisitos declarados. Para afirmar cobertura del perfil extendido se necesita su evidencia; el perfil base puede definirse sin esa extensión antes de administrar las tareas.

| Capacidad | Afirmación que se quiere sostener | Muestreo de tareas propuesto | Evidencia discriminante | Base |
| --- | --- | --- | --- | --- |
| CAP-01 Contexto y confianza | Modela activos, actores, flujos y autoridad relevantes | Un caso de aplicación y otro de integración/IA con fronteras distintas | Explica relaciones y riesgo concreto; no solo dibuja cajas | P023; P139; P001 |
| CAP-02 Diagnóstico causal | Distingue mecanismo y explicaciones competidoras | Historial de secretos, consulta inyectable y configuración/autorización | Prueba que discrimina hipótesis, con fuentes y límites | P135/P022; P001; P023 |
| CAP-03 Corrección y diseño seguro | Corrige mecanismo y previene recurrencia sin romper negocio | Parche, política/configuración y revisión preventiva de un cambio | Artefacto recuperable y justificación del control | P135/P022; P023; P001 |
| CAP-04 Verificación | Elige pruebas de seguridad y regresión e interpreta resultados | Cada mecanismo en condiciones positivas/negativas y una variante no practicada | Entradas, resultados, interpretación y límites del oráculo | P001; P135; P139; P038. Validez del verificador: P108 |
| CAP-05 Secretos y datos | Gestiona custodia, exposición, rotación/migración y minimización | AndinaPay más otra exposición con una credencial o canal diferente | Alcance, permisos, recuperación operacional y riesgo histórico | P036/P037; P038/P039; CWE-321 |
| CAP-06 Integridad y procedencia | Verifica artefactos y datos antes de darles autoridad | Deserialización, descarga/actualización y admisión de datos | Rechazo antes del efecto y aceptación auténtica autorizada | P139 e informe SEI, adquisición; P137; fuentes técnicas de Q2 |
| CAP-07 Sistemas con IA | Distingue entrenamiento, inferencia, herramientas y exposición | Prompt injection indirecta, poisoning y fuga con utilidad legítima | Ataque/defensa en sandbox, autorización externa al modelo, explicación | P079; P042/P044; P031 como actividad complementaria |
| CAP-08 Responsabilidad y comunicación | Justifica prioridades y expresa incertidumbre sin exceder evidencia | Informe individual y una decisión con coste/riesgo contrapuesto | Hechos citados, decisión, riesgo residual y límites | P001; P139; P023 |

“Otro caso” es una necesidad de variación, no una prescripción de que exactamente dos tareas acrediten competencia. El tamaño final del banco y cuántas muestras requiere cada capacidad se justifican con pilotaje y precisión del uso. Este blueprint no reemplaza la matriz por CWE de [[Competencias frente a las familias de ataques]].

## Banco inicial y ampliación

Primero se completa la integración de AndinaPay, BibliotecaViva, TalentoAndino, AndeanLogix y NubeAndina. Esos nombres no se contabilizan como ocho familias cubiertas: sus mecanismos y evidencias deben acreditarse individualmente. Después se agregan las lagunas de canal/uso criptográfico, XSS/comandos, SSRF, autenticidad/descarga, IA y exposición de datos.

Para cada tarea se autoriza una ficha con: capacidad y contenido; condición inicial; herramientas; artefactos; propiedad legítima; propiedad de seguridad; falso positivo; falso arreglo; evidencias D1-D4; ayudas; versión; riesgos de administración; contraste de transferencia. Un nuevo CWE exige un mecanismo nuevo o una justificación de cobertura, no una nueva etiqueta.

## Diferencia entre cobertura y dominio

La matriz de diseño informa qué oportunidades ofrece el banco. El expediente individual informa qué oportunidades recibió la persona y qué demostró. Si la tarea no se administró, no hay observación; si el sistema falló, hay incidencia; si hubo oportunidad y desempeño insuficiente, puede haber evidencia de nivel no demostrado. No sustituir estos estados por un porcentaje de casillas marcadas.

Para cada candidato a veredicto global se guarda: estándar y versión, capacidades esenciales, suficiencia de evidencia, condiciones de ayuda, desacuerdos, resolución y fecha. La validez se evalúa sobre el uso de ese resultado, no sobre el nombre de la plataforma.

## Criterios técnicos para construir tareas y corregirlas

Estos criterios permiten preparar una guía sin posponer el contenido a un panel. Se concretan con entradas y resultados conocidos para cada mecanismo; no son por sí solos un corte de aprobación profesional.

| Capacidad | Ejemplo de evidencia suficiente para la tarea delimitada | Contraejemplo que no basta |
| --- | --- | --- |
| CAP-01 | Identifica dato protegido, usuario autorizado, flujo y punto donde se acepta autoridad indebida | Dibuja componentes sin explicar qué permiso o frontera está comprometido |
| CAP-02 | Cita un fragmento o registro y ejecuta un contraste que distingue la causa propuesta de una alternativa plausible | Repite un CWE o pega un aviso del escáner sin explicar el mecanismo |
| CAP-03 | Entrega una revisión identificable donde el efecto adversario deja de ocurrir y el uso autorizado se conserva | Oculta el botón, bloquea toda la función o describe un parche sin entregar la implementación solicitada |
| CAP-04 | Elige y justifica un caso adversario y uno legítimo pertinentes, conserva resultados y limita la conclusión a lo comprobado | Usa solo pruebas docentes ya elegidas por el sistema y afirma haber diseñado su verificación |
| CAP-05 | Reconstruye dónde se expuso la credencial, limita accesos y justifica rotación/migración y riesgo de copias anteriores según el caso | Elimina la clave de la última versión y declara resuelto el historial |
| CAP-06 | Verifica integridad, origen y autorización antes del efecto, rechazando también un artefacto auténtico no autorizado cuando corresponda | Comprueba una firma después de ejecutar o asume que firmado significa benigno |
| CAP-07 | Identifica la etapa atacada y muestra un control que limita el efecto prohibido conservando una tarea legítima en ese mecanismo | Bloquea palabras o desactiva todo el agente y generaliza a poisoning o fuga no evaluados |
| CAP-08 | Distingue hechos y supuestos, justifica prioridad y alternativas, e informa impacto y riesgo residual con referencias a la entrega | Informe convincente sin evidencia, atribuciones causales inventadas o afirmación de seguridad total |

Las entradas se diseñan con datos sintéticos y un resultado esperado independiente del estudiante. La guía debe aceptar soluciones diferentes que satisfagan las propiedades, conservar un ejemplo válido y uno insuficiente por criterio y señalar cuándo es necesaria revisión de una respuesta no prevista. Si un solo caso no exige una capacidad, no se declara observada por completar ese caso.

No se puntúan por separado todos los rótulos que coinciden en una misma actuación: corregir y verificar una clave puede aportar a CAP-03/04/05, pero sigue siendo una sola situación. La generalización requiere variación de mecanismos y condiciones.

## Guía de aplicación

[[Guía para evaluar las competencias de seguridad]] concreta qué prepara el autor, qué entrega el estudiante y cómo registrar el juicio. Incluye criterios, ejemplos sintéticos de consultas SQL, autorización, admisión de artefactos e integración con IA. AndinaPay conserva su especificación canónica y sus contrastes en [[Revisión del escenario AndinaPay]]. Los ejemplos de la guía no se contabilizan como nuevas tareas implementadas o validadas.
