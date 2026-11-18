---
type: decision
status: propuesto
---
# Síntesis de decisiones para CyberSim

El objetivo del estudio es evaluar competencias de desarrollo seguro ya adquiridas por estudiantes con formación previa. Los escenarios presentan problemas para que demuestren esas capacidades mediante decisiones, soluciones y pruebas. El estudio se centra en la calidad de esa evaluación; enseñar contenidos de seguridad o medir mejoras de aprendizaje queda fuera de su alcance.

La decisión es construir una **evaluación de desarrollo seguro basada en evidencia**, integrada en los escenarios 3D existentes. Cada escenario presenta una situación, permite investigar y actuar, conserva una entrega y relaciona el juicio con artefactos verificables. El perfil profesional se declara solo sobre competencias, tareas, herramientas y condiciones de ayuda previamente delimitadas.

## Respuestas a las cuatro preguntas

| Pregunta | Respuesta de la revisión | Consecuencia al programar |
| --- | --- | --- |
| Q1. Cómo evaluar desde 3D | El escenario debe provocar diagnóstico, decisión, intervención y verificación. El 3D sitúa actores, recursos y consecuencias; el juicio se apoya en artefactos, razonamiento y pruebas | Integrar herramientas funcionales en el monitor y registrar la revisión que se entrega; conservar rutas alternativas y acceso equivalente |
| Q2. Qué competencias | Analizar confianza, diagnosticar, corregir, verificar, gestionar secretos/datos, preservar integridad, razonar sobre IA y comunicar responsablemente; observarlas mediante tareas específicas de las ocho familias | Aplicar la matriz de 24 entradas/22 CWE y el plan de cobertura. Etiquetar una actividad con un CWE no acredita toda su familia |
| Q3. Fundamento de la selección | Usar el modelo de aseguramiento de software como referencia de dominio y nivel; corresponder las expresiones de Assyne y complementarlas con tareas de estudiantes y mecanismos técnicos | La correspondencia ya está documentada; construir criterios y ejemplos con esas fuentes. La validación del instrumento se distingue de inventar competencias |
| Q4. Cuándo declarar competente | Un intento sustenta una observación. Varias muestras representativas, una puntuación defendible y un estándar justificado permiten una conclusión sobre el perfil delimitado | Primero informes por dimensiones; después una regla de decisión versionada y calibrada. No inferir competencia profesional por terminar cinco escenarios |

## Perfil adoptado para diseñar

Estudiante próximo a finalizar ingeniería de software que puede analizar, corregir y verificar seguridad de aplicaciones y sus integraciones, frente a las ocho familias proporcionadas, con documentación técnica permitida y ayudas declaradas. Debe conservar funcionalidad legítima, justificar decisiones y comunicar alcance e incertidumbre. No se presupone que dirige un SOC ni que cubre todos los roles de seguridad.

Esta formulación concreta el objetivo del usuario. La validación institucional del nivel requerido es una actividad del desarrollo del instrumento, no una búsqueda bibliográfica inconclusa.

## Por qué esta combinación

Los marcos generales aportan continuidad con ingeniería de software; los profesionales especializados aportan responsabilidades y vocabulario; los estudios de evaluación ayudan a diseñar tareas e interpretar resultados; los estudios técnicos fijan mecanismos y contrastes reales. Ninguna de esas piezas, aislada, acredita a una persona. Las lecturas completas y los motivos de selección están en [[Análisis crítico de los estudios centrales]].

El entorno 3D debe permitir observar las competencias previstas sin que el manejo de la interfaz distorsione los resultados. La evidencia permite justificar un diseño explícito de evaluación y comprobarlo localmente. No se encontró un instrumento validado que pueda instalarse sin adaptación y que resuelva exactamente las ocho familias en CyberSim.

## Qué queda decidido

Conservar D1-D4 como dimensiones de observación, el ledger y el generador de informes existentes; completar la evidencia de extremo a extremo antes de añadir puntuación global. Mantener AndinaPay con las correcciones de causalidad y recuperación, incorporar las otras vistas funcionales y ampliar contenidos según lagunas. Separar pruebas del alumno de la batería docente, ayuda de autonomía y falta de evidencia de desconocimiento.

El primer incremento es **AndinaPay con snapshot recuperable, entrega confirmada y comprobación docente confiable**. Después: revisión docente, variantes, pilotaje del instrumento y expansión. El detalle está en [[Ruta de programación de CyberSim]].

## Cierre y límites

El cierre histórico del 13-11-2026 contiene 120 publicaciones recientes distintas cribadas y 15 artículos de texto completo. La ampliación del 15–16-11-2026 comprueba abstract y cierre de 50 publicaciones (47 reexaminadas y tres incorporaciones) y añade dos lecturas integrales; el inventario actual tiene 137 fichas y 17 textos completos. El registro permite comprobar los recuentos por pregunta y el alcance de cada lectura. No equivale a recuperar toda publicación existente ni a reproducir experimentos. Las incertidumbres materiales se traducen en condiciones de diseño o validación específicas, no en una tarea genérica de “seguir investigando”.

## Fundamento completado de las capacidades

[[Fundamento de las competencias de seguridad de CyberSim]] explica el modelo elegido, el nivel de referencia, los estudios directos de tareas y las especializaciones técnicas. [[Correspondencia de competencias de Assyne con CyberSim]] deja una decisión para cada expresión de sus once grupos. [[Revisión focalizada de competencias de seguridad]] permite comprobar las 50 lecturas de esta ampliación. CAP-07 se trata como extensión con formación previa; las demás capacidades no se presentan como una homologación automática del modelo profesional.

## Aplicación de la selección a la corrección

[[Guía para evaluar las competencias de seguridad]] especifica productos, estados y ejemplos de juicio, conservando las propiedades técnicas y las razones del estudiante. No requiere crear el catálogo desde cero con especialistas; requiere corrección competente en los contenidos y revisión de respuestas ambiguas. La continuación añadió la lectura integral de P135, sin alterar los 50 cribados ni las 137 fichas.
