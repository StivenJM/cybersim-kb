---
type: paper
year: 2022
lectura: texto-completo
preguntas: [Q2, Q3, Q4]
revision_competencias: "2026-11-16"
---
# Lam - Diagnóstico y corrección de código inseguro

**P135. Identifying Gaps in the Secure Programming Knowledge and Skills of Students.**

[Publicación y DOI](https://doi.org/10.1145/3478431.3499391) · Consulta: 15–16-11-2026.

## Aporte

Entrevistas de programación con 21 estudiantes de dos universidades; identifica dificultades al reconocer, explicar y corregir código inseguro.

## Límite y valoración

Estudio pequeño en tareas de C; las mismas entrevistas se reanalizan en P022, por lo que no son dos muestras independientes.

## Decisión para CyberSim

Usar actuaciones de diagnóstico, explicación, prueba y corrección como antecedentes directos de tareas acotadas; no importar umbrales ni generalizar a todo AppSec. Los identificadores CAP son de CyberSim, no del artículo. La aplicación evalúa capacidades previas; no adopta un programa de aprendizaje.

## Alcance de lectura

**texto-completo**. Lectura ampliada el 16-11-2026. Dentro de la ventana reciente histórica.

Siete páginas del manuscrito de autor: introducción, trabajos relacionados, método, resultados, discusión, limitaciones, conclusiones y referencias; texto de figuras tabulares 1 y 2. [Manuscrito de autor](https://majedalmansoori.com/papers/Lam_SIGCSE22.pdf). No se inspeccionó visualmente el PDF ni se leyó íntegro el cuestionario externo; las figuras se examinaron como tablas textuales.

## Revisión focalizada de competencias

Evaluar identificación, explicación, entradas que evidencian fallos y corrección de código inseguro; son tareas acotadas de estudiantes, no una certificación global.

[[Fundamento de las competencias de seguridad de CyberSim]] · [[Revisión focalizada de competencias de seguridad]]

## Dependencia de muestras

P022 reanaliza las mismas 21 entrevistas de este artículo. Son dos publicaciones con aportes diferentes, no dos muestras independientes. La figura 1 del método explicita actuaciones de reconocimiento, explicación, uso de alternativas y corrección. La primera comprobación fue de abstract, cierre y método; la continuación del 16-11-2026 completó el texto del artículo. El historial de ampliación no se cuenta como otro paper.

## Implicación de la lectura completa

El método permitió documentación, búsquedas y entorno de programación. La muestra no exigía haber cursado seguridad; además, la primera pregunta cambió entre sedes. Por ello el estudio respalda observar actuaciones concretas, no fijar un estándar uniforme de egreso. La aplicación en CyberSim distingue recursos permitidos, pistas y solución de referencia y comprueba la propiedad del cambio, sin premiar simplemente el nombre de una función supuestamente más segura.

El formato de entrevista y las preguntas sobre fragmentos pequeños limitan la extrapolación. Las seis áreas del análisis son antecedentes de conocimiento y habilidades; no se adoptan como seis notas o factores calibrados. La mejora formativa propuesta por los autores no se convierte en objetivo de CyberSim.

La adaptación operativa queda en [[Guía para evaluar las competencias de seguridad]].
