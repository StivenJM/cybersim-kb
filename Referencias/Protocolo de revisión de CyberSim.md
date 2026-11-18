---
type: guide
status: cerrado
---
# Protocolo de revisión de CyberSim

Fecha de inicio y corte: **2026-11-13**, UTC. Ventana reciente: **2021-11-13 a 2026-11-13**. Los antecedentes anteriores se conservan separados y no completan la cuota reciente.

## Encargo y criterio de cierre

El usuario pide cuatro respuestas, al menos 30 papers examinados por pregunta, cribado de abstract y conclusiones, lectura integral de los prometedores y decisiones de programación fundamentadas. Se interpreta conservadoramente su fórmula `30 × 4` como **120 trabajos distintos**. Un paper útil para varias preguntas tiene una sola identidad y varias relaciones; no se convierte en varios papers.

**Revisión cerrada al corte indicado; cumplimiento y alcances en [[Registro de revisión de CyberSim]].** Un registro localizado, una ficha editorial, el corpus de una revisión ajena y una consulta de buscador no cuentan como un paper cribado por abstract y conclusiones. Solo los recuentos comprobados en el corpus se anuncian como cumplimiento; los accesos parciales quedan fuera.

## Preguntas operacionales

El objetivo del estudio es evaluar competencias de desarrollo seguro ya adquiridas por estudiantes con formación previa. Los escenarios presentan problemas para que demuestren esas capacidades mediante decisiones, soluciones y pruebas. El estudio se centra en la calidad de esa evaluación; enseñar contenidos de seguridad o medir mejoras de aprendizaje queda fuera de su alcance.

Los estudios de enseñanza se mantienen en el registro como antecedentes examinados. De ellos solo se adoptan aportes pertinentes para tareas, evidencias, condiciones de administración y validez de la evaluación; no se incorporan programas de enseñanza, tutoría ni mediciones de mejora de aprendizaje como requisitos del proyecto.

| ID | Pregunta de revisión | Producto necesario |
| --- | --- | --- |
| Q1 | ¿Qué tareas y evidencias en escenarios 3D permiten interpretar competencias específicas de seguridad en estudiantes de ingeniería de software? | Diseño del instrumento, papel del 3D y revisión de AndinaPay |
| Q2 | ¿Qué capacidades observables necesita el perfil objetivo frente a las ocho familias proporcionadas? | Matriz amenaza–tarea–competencia–evidencia–cobertura |
| Q3 | ¿Qué conservar, adaptar y complementar del mapeo general de competencias y de SECAT? | Comparación de marcos y trazabilidad de adaptaciones |
| Q4 | ¿Qué evidencia adicional permite pasar de una actuación a una decisión de competencia del perfil delimitado? | Reglas de inferencia, muestreo de tareas y validación de decisiones |

## Recuperación

Se realizan búsquedas web dirigidas, búsquedas de títulos exactos y seguimiento de editoriales, actas, repositorios institucionales y páginas de autores. No se dispone de una exportación nativa de todas las bases Scopus, Web of Science, ACM e IEEE. No se presenta esta ejecución como una búsqueda exhaustiva de todo el estado del arte ni como una revisión sistemática registrada.

Familias de consultas: `cyber range assessment competencies`; `3D virtual reality cybersecurity assessment`; `secure coding competencies education`; `software engineering competence framework`; `cybersecurity psychometric performance validity`; títulos exactos junto a `abstract`, `conclusion` y `pdf`; gestión de secretos e inyección/poisoning en LLM. El registro de búsquedas conserva fecha, consulta y fuente recuperada cuando la llamada está disponible. Algunos primeros resultados de búsqueda no se guardaron íntegros; no se reconstruyen como consultas auditadas completas.

## Inclusión y exclusión

Incluir estudios empíricos educativos, instrumentos, revisiones y propuestas de marcos relevantes. Distinguir población profesional, universitaria, escolar y ciudadanía. Un paper técnico puede sustentar el mecanismo de una tarea en Q2, pero no demostrar validez de una medida humana. NICE, ECSF y CWE son referencias institucionales separadas del conteo de papers.

Excluir del argumento central marketing, resúmenes automáticos de terceros, resultados sin autoría verificable y fuentes que solo comparten palabras clave. Registrar por separado paywall, 403, 404, CAPTCHA y textos incompletos. Un fracaso de acceso no es una exclusión por calidad ni prueba de inexistencia.

## Niveles de lectura

| Estado | Qué significa | ¿Cubre el cribado exigido? |
| --- | --- | --- |
| localizado | Identidad o ficha encontrada | No |
| extractos | Pasajes parciales, sin ambas secciones completas | No |
| resumen | Abstract original examinado | No |
| resumen-conclusiones | Abstract y cierre del artículo examinados; registrar el acceso | Sí, si fecha y elegibilidad están verificadas |
| secciones | Se han leído secciones adicionales, pero no todo el cuerpo | No automáticamente; revisar si también se leyeron ambas secciones |
| texto-completo | Texto del artículo, método, resultados y discusión examinados | Sí; indicar limitaciones de figuras, anexos y materiales externos |

`Texto-completo` no significa reproducción de experimentos, auditoría de código/datasets ni revisión de cada referencia citada. Las figuras no examinadas visualmente y los suplementos ausentes deben declararse; si afectan la decisión, debe recuperarse antes de usarla como fundamento exclusivo; si no es material, se limita la afirmación y se declara el alcance.

## Lectura crítica de prometedores

Extraer problema, población, tarea, unidad de análisis, condiciones de ayuda, instrumento, evidencia, análisis, resultados, límites y disponibilidad. Contrastar abstract con método y conclusiones. Clasificar por separado los resultados de aprendizaje de los estudios ajenos, la medición de conocimientos, el desempeño técnico y la preparación profesional. Las recomendaciones para CyberSim se limitan a la evaluación de competencias ya adquiridas. Evaluar selección, confusores, medición, pérdidas, independencia de datos y transferibilidad; no reducir todo a una puntuación de calidad inventada.

Una propuesta sin participantes no se registra como ensayo de eficacia; un artículo de dataset no como validación educativa; varias publicaciones con los mismos participantes no como réplicas independientes. Toda recomendación local debe distinguir **hallazgo de fuente**, **inferencia propia**, **decisión de diseño** y **comprobación del instrumento**.

## Cierre por pregunta

1. Al menos 30 trabajos recientes distintos con abstract y conclusiones verificados para esa pregunta.
2. Subconjunto prometedor leído de manera integral, incluidos elementos materiales para la decisión; justificar selección y descartes.
3. Comparación de alternativas y evidencia que podría refutar la decisión.
4. Trazabilidad a código actual y criterios observables de aceptación.
5. Informe explícito de incertidumbre, accesos pendientes y límites de cobertura.

La cuota es un mínimo de cobertura solicitado, no una garantía de saturación. La actualidad de las ocho familias de ataques se toma como entrada del compañero; esta revisión no reproduce ni valida su ranking de frecuencia.

Relacionado: [[Estado del arte]], [[Registro de revisión de CyberSim]], [[Ruta de programación de CyberSim]].

## Ampliación focalizada del 15–16-11-2026

Se abrió una fase específica para fundamentar la selección frente al catálogo de Assyne y otros modelos publicados. El mínimo solicitado es 50 publicaciones distintas con abstract y cierre comprobados, sin imponer que todas sean nuevas o recientes. Se registran por separado las fuentes reexaminadas y las incorporaciones. Una discusión final cumple el criterio de cierre cuando no existe una conclusión separada; se declara el pasaje exacto.

El resultado y la selección de mayor profundidad están en [[Revisión focalizada de competencias de seguridad]]. El cierre histórico de 120 recientes se conserva con su ventana original; no se suman cribados solapados. Las competencias generales, los mecanismos técnicos y los métodos de evaluación desempeñan funciones diferentes en el argumento.
