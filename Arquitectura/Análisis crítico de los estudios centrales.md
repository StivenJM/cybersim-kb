---
type: analysis
status: propuesto
---
# Análisis crítico de los estudios centrales

En el cierre histórico del 13-11-2026 se seleccionaron 15 artículos por su relación directa con una decisión material: delimitación del perfil, alineación de escenarios, procesos de respuesta, rúbricas, papel del 3D, evaluación técnica o mecanismo de AndinaPay. “Prometedor” significa que merecía lectura completa para decidir si adoptar su propuesta; no que todas sus conclusiones terminaran aceptadas.

| Núcleo | Preguntas | Qué se adopta | Qué impide importar sus resultados |
| --- | --- | --- | --- |
| P001, mapeo de competencias | Q2/Q3/Q4 | Continuidad con ingeniería de software y capacidades transversales | Antigüedad de búsqueda; catálogo sin prueba de suficiencia |
| P007, REWIRE | Q1/Q2/Q3 | Adaptar responsabilidad→tarea→resultado→evidencia | Pesos de priorización de roles y certificados de curso no son notas del alumno |
| P010, NICE-by-design | Q1/Q3 | Auditar oportunidades de observación y cobertura de la evaluación | TKS cubiertos no equivalen a dominio individual |
| P005, psicometría CTF | Q1/Q4 | Examinar funcionamiento empírico de tareas | Unidad colectiva y dependencia de ediciones |
| P013, VR de ciberseguridad | Q1 | Modalidades y familiarización | Medidas declarativas y problemas de cálculo/reporting |
| P022, programación segura | Q1/Q2/Q3 | Observar razonamiento y uso crítico de recursos | Reanálisis de misma muestra y rúbrica específica de C |
| P023, threat modeling | Q1/Q2/Q3/Q4 | Justificación de flujos, interacciones y mitigación | Cambios simultáneos y evaluación de equipos |
| P031, prompt injection práctico | Q1/Q2 | Diseñar una situación de contraste en IA | Salidas de un sistema no demuestran competencia individual |
| P032, revisión de CTF | Q1/Q4 | Separar engagement, confianza y evidencia de dominio | Certeza heterogénea y límites de recuperación/cribado |
| P042, AgentDojo | Q2 | Separar utilidad legítima y efecto adversario con estado comprobable | Tareas combinadas, permisos y ataques limitados; no evalúa competencia humana |
| P044, contaminación del ajuste | Q2 | Separar entrenamiento e inferencia; medir contaminación y función legítima | Supuestos de ingestión, modelos/tareas antiguos y escalado dependiente del objetivo |
| P036, gestión de secretos | Q2 y AndinaPay | Evaluar ciclo de vida y exposición histórica | Recomendación frecuente no es eficacia comprobada |
| P061, procesos de respuesta | Q1/Q3/Q4 | Comprobar lo que realmente moviliza la tarea | Ajuste del modelo y recodificación no son validación independiente |
| P108, jueces y parches | Q1/Q2/Q4 | Verificar seguridad y función con oráculos suficientes | Oráculos incompletos, artefactos y generalización limitada |
| P131, revisión de IVR | Q1/Q3/Q4 | Alinear objetivo, actividad y evidencia | Marco conceptual e inconsistencias de selección/clasificación |

Los análisis detallados, alcances y localizadores están en las fichas canónicas enlazadas al final. No se crea una copia de cada paper por pregunta.

Los estudios sobre enseñanza, tutoría o mejoras de aprendizaje se conservan como antecedentes de la revisión. Sus intervenciones formativas no se adoptan como objetivos ni como requisitos de CyberSim: solo se recuperan aportes pertinentes para diseñar y validar la evaluación de competencias previamente adquiridas.

## Comparación de alternativas para CyberSim

| Alternativa | Qué resuelve | Riesgo para esta aplicación | Decisión |
| --- | --- | --- | --- |
| Lista literal de competencias generales | Vocabulario de antecedentes | Constructos sin oportunidad de observación y omisiones especializadas | Adaptar, no usar como lista de aprobación |
| Puntos/flags/tiempo | Feedback y dinámica competitiva | Premia éxito puntual, velocidad o equipo, sin justificar generalización individual | Solo registro de progreso; no se adopta como medida de competencia |
| Cuestionario conceptual | Conocimiento de mecanismos | No observa corrección ni decisiones bajo condiciones reales | Complemento si hay afirmación de conocimiento específica |
| Autoevaluación/SUS/presencia | Experiencia y confianza | Confusión de constructos al usarlos como dominio técnico | Medidas auxiliares del diseño, fuera del veredicto de competencia |
| Evidencia explícita con verificadores y rúbrica | Producto, razones y actuación situada | Requiere buen oráculo, muestras y correctores | Opción inicial elegida por coherencia con el código actual |
| Inferencia estadística desde telemetría | Modelar patrones y posibles alertas | Identificabilidad, sesgo, coste y etiquetas sin validez | Posponer hasta disponer de diseño y datos adecuados |
| Calificación por LLM | Escalabilidad de feedback | Juicios plausibles, sesgos y acuerdo sin validez | Apoyo revisable; no autoridad final sin validación local |

## Dependencias entre evidencias

Varias revisiones comparten estudios primarios: no se suman sus participantes ni sus hallazgos como réplicas. P022 reanaliza la muestra de su antecedente. Los estudios de detectores que comparten SecretBench no constituyen validaciones independientes por cambiar el clasificador. Las tareas de un mismo equipo, intentos repetidos y parches de la misma vulnerabilidad generan dependencia; el diseño y análisis deben conservar esa estructura.

P011 (SASS) se rebajó como evidencia de validez al comprobar su demostración pequeña y pesos heurísticos. P012 presenta un modelo multimodal sin datos nuevos analizados. Un estudio CyberSense de 2026 ofrece afirmaciones experimentales incompatibles con su declaración de datos. No se adoptaron sus porcentajes como evidencia suficiente. En estudios de ítems generados, ausencia de significación no prueba equivalencia. Se conservaron las fichas y límites, en lugar de elegir solo resultados favorables.

## Fuerza de las decisiones

Hay una justificación convergente para separar cobertura, participación, confianza y desempeño y para alinear tareas con evidencia. La propuesta concreta de ocho capacidades, D1-D4 y sus anclajes es una decisión local; no se presenta como una escala demostrada por esa convergencia. Los pesos y cortes de puntuación, el número suficiente de tareas y la extrapolación profesional permanecen sin demostración para CyberSim y se someten al protocolo de validación de la evaluación. El papel del 3D se revisa por las evidencias que permite obtener y por las barreras que pueda introducir.

Esto no mantiene abierta la revisión encargada: sus respuestas y el diseño derivado se entregan completos. Delimita qué afirmaciones podría sostener el instrumento una vez implementado y validado.

## Fichas de lectura completa

- [[Assyne - Estado de competencias de software]] — P001.
- [[CTF - Límites de la puntuación competitiva]] — P005.
- [[REWIRE - Cursos y certificación por perfil]] — P007.
- [[NICE-by-design - Diseño trazable de escenarios]] — P010.
- [[VR - Comparación de modalidades educativas]] — P013.
- [[Almansoori - Componentes del razonamiento seguro]] — P022.
- [[Threat modeling - Rúbricas de pensamiento sistémico]] — P023.
- [[LLM - Entrenamiento práctico de prompt injection]] — P031.
- [[CTF - Certeza de la evidencia educativa]] — P032.
- [[Secretos - Prácticas de gestión]] — P036.
- [[Modelado - Validación con procesos de respuesta]] — P061.
- [[Parches - Validez del juez frente a ejecución]] — P108.
- [[Programación - Fundamentos pedagógicos del 3D]] — P131.

- [[AgentDojo - Seguridad y utilidad por separado]] — P042.

- [[Poisoning - Datos de ajuste de instrucciones]] — P044.

## Ampliación del fundamento de competencias · 16-11-2026

La ampliación incorpora una lectura integral adicional, [[Mead y Shoemaker - Competencias de aseguramiento de software]] (P139), y comprueba abstract y cierre de 50 publicaciones. El artículo ofrece una referencia explícita de pregrado y aseguramiento de software, más pertinente para el nivel que adoptar todo un rol SOC. Sus niveles no se traducen en puntuaciones ni homologan las ocho CAP. La tabla detallada del informe asociado sitúa ciertas contramedidas en L3; por eso las correcciones se acotan y complementan con tareas de estudiantes de P135/P022.

[[Lam - Diagnóstico y corrección de código inseguro]] (P135) es el antecedente empírico reanalizado por P022: dos publicaciones, una misma muestra de 21 entrevistas. [[Braz y Bacchelli - Seguridad en revisión de código]] (P137) aporta contexto de dependencias e interacciones en profesionales; no un estándar de estudiantes. P079 sustenta contenido de una especialización de IA y declara pendiente su evaluación de resultados. P067 y P076 son síntesis útiles, pero no una escala validada que justifique importar pesos u ocho factores.

La selección y exclusiones frente a Assyne están realizadas; no se presentan como una futura labor genérica de especialistas. Queda por comprobar el instrumento y su posible estándar de aprobación. Los pasajes y los límites de las nuevas lecturas se documentan en [[Revisión focalizada de competencias de seguridad]] y la decisión en [[Fundamento de las competencias de seguridad de CyberSim]].
