---
type: paper
year: 2024
lectura: texto-completo
preguntas: [Q1, Q2, Q3, Q4]
revision_competencias: "2026-11-16"
---
# Threat modeling - Rúbricas de pensamiento sistémico

**P023. Introducing Systems Thinking as a Framework for Teaching and Assessing Threat Modeling Competency.**

[Fuente original o ficha de autor](https://arxiv.org/abs/2404.16632) · Consulta: 13-11-2026.

## Aporte

Propone rúbricas de STRIDE y pensamiento sistémico; aplica a entregables de tres cohortes de ingeniería de software.

## Límite y valoración

No asumir que la rúbrica de un curso se transfiere validada a los casos CWE o que las cohortes identifican causalidad.

## Decisión para CyberSim

Evaluar fronteras de confianza y efectos entre componentes; no solo identificar etiquetas CWE. Esta aplicación es una inferencia de diseño local; no un resultado experimental en CyberSim.

## Alcance de lectura

**texto-completo**. Cuenta en la cuota reciente.

PDF de 31 páginas: cuerpo, tablas 1-4, seis figuras y apéndice A con rúbricas completas; líneas 0-1183

Tablas: Tablas 1-4 y A1-A2 leídas, escalas beginner/intermediate/advanced y cero por ausencia

Figuras: Figuras 1-6 inspeccionadas en PDF local, páginas 9-10 y 15-19

## Análisis crítico propio

Quince proyectos de equipos, cinco por cohorte, no quince estudiantes. Cambiaron simultáneamente instrucción, herramienta y consignas; cohortes históricas y uso permitido de LLM impiden atribuir las diferencias a systems thinking solo. El 94% de acuerdo porcentual tras refinamiento no establece validez de las inferencias ni equivale a kappa. Las respuestas más extensas pueden reflejar la nueva consigna. Una frontera de confianza describe un límite; no bloquea ataques por dibujarla, aunque el artículo use esa expresión. STRIDE no es incapaz por definición de analizar flujos o interacciones.

**Aplicación adoptada:** Adoptar preguntas sobre activos, flujos, interacciones, decisiones y límites; corroborar implementación con pruebas y no solo con un informe convincente.

La lectura del artículo no implica reproducir sus experimentos, auditar sus datos ni leer íntegramente todos los trabajos citados. Los materiales externos no recuperados se declaran en [[Registro de revisión de CyberSim]].

[PDF original conservado](<Threat modeling - Rúbricas de pensamiento sistémico.pdf>)

## Relaciones

[[Evaluación de competencias en escenarios 3D|Q1]] · [[Competencias frente a las familias de ataques|Q2]] · [[Selección y adaptación de marcos de competencias|Q3]] · [[Del desempeño a la competencia del perfil|Q4]] · [[Registro de revisión de CyberSim]]

## Revisión focalizada de competencias · 16-11-2026

**Función en la selección:** fundamento directo de tareas. Tomar activos, flujos, actores, fronteras y justificación de mitigaciones de las rúbricas; sus proyectos de equipos no acreditan automáticamente desempeño individual.

Pasajes comprobados: Abstract p. 1; Conclusion p. 23; apéndice A pp. 27–31. [Acceso consultado](https://arxiv.org/pdf/2404.16632). Esta nueva comprobación de abstract y cierre no implica una segunda lectura íntegra de todos los materiales declarados en la fase anterior.

[[Fundamento de las competencias de seguridad de CyberSim]] · [[Revisión focalizada de competencias de seguridad]]
