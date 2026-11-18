---
type: paper
year: 2025
lectura: texto-completo
preguntas: [Q1, Q2, Q3, Q4]
---
# LLM - Entrenamiento práctico de prompt injection

**P031. Hands-On Training Framework for Prompt Injection Exploits in Large Language Models.**

[Fuente original o ficha de autor](https://doi.org/10.3390/engproc2025108025) · Consulta: 13-11-2026.

## Aporte

Plataforma ensayada con diez equipos; informa consultas adversarias y resistencia del modelo a revelar flags.

## Límite y valoración

La tasa de bloqueo del modelo no mide aprendizaje de personas. Sus defensas por palabras clave no acreditan protección general.

## Decisión para CyberSim

Diseñar tareas de identificación, reparación y comprobación legítima/adversa; separar éxito del ataque de competencia humana. Esta aplicación es una inferencia de diseño local; no un resultado experimental en CyberSim.

## Alcance de lectura

**texto-completo**. Cuenta en la cuota reciente.

Artículo completo, tabla de cinco desafíos y cuatro figuras editoriales.

Tablas: Tabla de instrucciones y objetivos leída completa.

Figuras: Figuras 1-4 inspeccionadas visualmente.

## Análisis crítico propio

Diez equipos y 1126 consultas describen la actividad y respuestas del sistema, no una prueba pre/post de dominio individual. La figura de defensa usa detección de palabras: eso no demuestra una solución robusta a prompt injection. El 88.8% corresponde a respuestas bloqueadas o incorrectas para el atacante bajo ese evento, no a aprendizaje. Las tareas contienen instrucciones deliberadamente contradictorias y no representan por sí solas un agente con herramientas.

**Aplicación adoptada:** Puede inspirar situaciones de ataque y análisis de límites; añadir utilidad legítima, defensa y explicación individual.

La lectura del artículo no implica reproducir sus experimentos, auditar sus datos ni leer íntegramente todos los trabajos citados. Los materiales externos no recuperados se declaran en [[Registro de revisión de CyberSim]].

## Relaciones

[[Evaluación de competencias en escenarios 3D|Q1]] · [[Competencias frente a las familias de ataques|Q2]] · [[Selección y adaptación de marcos de competencias|Q3]] · [[Del desempeño a la competencia del perfil|Q4]] · [[Registro de revisión de CyberSim]]
