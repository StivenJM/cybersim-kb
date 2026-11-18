---
type: paper
year: 2024
lectura: texto-completo
preguntas: [Q2]
---
# AgentDojo - Seguridad y utilidad por separado

**P042. AgentDojo: A Dynamic Environment to Evaluate Prompt Injection Attacks and Defenses for LLM Agents.**

[Fuente original](https://proceedings.neurips.cc/paper_files/paper/2024/hash/97091a5177d8dc64b1da8bf3e1f6fb54-Abstract-Datasets_and_Benchmarks_Track.html) · Consulta: 13-11-2026.

## Aporte

Entorno de evaluación de agentes que separa tareas legítimas y propiedades de seguridad.

## Límite y valoración

Una defensa que bloquea todo puede evitar el ataque y fallar la tarea. El benchmark no mide competencia humana.

## Decisión para CyberSim

Reutilizar el principio de dos oráculos: función legítima y seguridad; no trasladar sus puntuaciones. La aplicación educativa es una inferencia local, no un resultado experimental en CyberSim.

## Alcance de lectura

**texto-completo**. Cuenta en la cuota reciente.

Artículo completo en HTML y PDF arXiv v3: introducción, secciones 2–5, checklist y apéndices A–F. Código y prompts que no aparecían en la conversión HTML se examinaron visualmente en PDF.

Tablas: Tablas 1–5 leídas, incluidos intervalos y desgloses por modelo/defensa.

Figuras: Figuras 1–21 inspeccionadas visualmente en el PDF original; incluyen definiciones de código, prompts y resultados. No se ejecutaron el repositorio ni sus trazas externas.

## Análisis crítico propio

AgentDojo distingue utilidad legítima y éxito de un objetivo adversario sobre un estado ejecutable. Los 629 casos proceden de combinar 97 tareas de usuario y 27 objetivos de inyección: no son 629 contextos independientes ni observaciones humanas. La proporción de salida controlada y los permisos disponibles cambian mucho entre suites; una tasa global puede ocultarlo. El ataque Max selecciona entre un conjunto limitado, no representa al adversario óptimo. El filtro de herramientas ayuda especialmente cuando basta lectura para la tarea legítima y el ataque requiere escritura; falla si ambos necesitan las mismas herramientas o si no pueden planificarse de antemano. El paper no cubre plenamente sesiones largas con tareas sucesivas. La tabla 1 dice 70 herramientas en su leyenda, pero sus filas suman 74 y el cuerpo también dice 74; hay además texto inicial heredado sobre utilidad menor a 66% que no describe todas las filas de la versión ampliada. No se importan esas cifras como rendimiento actual en 2026. Los oráculos son especificados manualmente y también requieren auditoría de suficiencia. El estudio evalúa agentes y defensas de 2024; no valida una rúbrica ni un aprendizaje de estudiantes.

**Aplicación adoptada:** Para CAP-07, conservar tareas legítimas y objetivos prohibidos independientes, cambios de estado observables y autoridad de herramientas limitada fuera del prompt. Evaluar la explicación y la intervención del estudiante; el porcentaje de éxito del agente es evidencia técnica del artefacto, no una nota humana.

La lectura no implica reproducción ni lectura íntegra de todos los trabajos citados.

[PDF original conservado](<AgentDojo - Seguridad y utilidad por separado.pdf>)

## Relaciones

[[Competencias frente a las familias de ataques|Q2]] · [[Registro de revisión de CyberSim]]
