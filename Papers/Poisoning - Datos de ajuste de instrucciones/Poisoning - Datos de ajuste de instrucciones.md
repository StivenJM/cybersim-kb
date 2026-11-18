---
type: paper
year: 2023
lectura: texto-completo
preguntas: [Q2]
---
# Poisoning - Datos de ajuste de instrucciones

**P044. Poisoning Language Models During Instruction Tuning.**

[Fuente original](https://proceedings.mlr.press/v202/wan23b.html) · Consulta: 13-11-2026.

## Aporte

Muestra contaminación del ajuste por ejemplos maliciosos y degradación de tareas bajo disparadores.

## Límite y valoración

Ataque de entrenamiento distinto de la inyección durante inferencia; un filtro de inputs no es defensa general de la cadena.

## Decisión para CyberSim

Evaluar procedencia del dataset, permisos, integridad y comprobación de comportamiento tras entrenamiento. La aplicación educativa es una inferencia local, no un resultado experimental en CyberSim.

## Alcance de lectura

**texto-completo**. Cuenta en la cuota reciente.

PDF editorial de 13 páginas completo: cuerpo, método de contaminación, experimentos, defensas, limitaciones, discusión y apéndices A–D.

Tablas: Tablas 1–5 leídas, con modelos, datos, ejemplos y resultados.

Figuras: Figuras 1–12 inspeccionadas visualmente, incluidas las tres figuras de los apéndices. No se reprodujeron entrenamientos ni se auditaron los datos externos.

## Análisis crítico propio

El atacante debe conseguir que sus ejemplos entren en el ajuste por instrucciones; ese supuesto no prueba que cualquier dato enviado a un servicio comercial se use para entrenar. Algunos ejemplos conservan etiquetas aparentemente correctas: validación de formato, hashes o firma de origen no garantizan ausencia de contaminación semántica. Se estudian T5/Tk-Instruct de 770M a 11B y tareas de 2023, no todos los modelos actuales. La afirmación de que los mayores son más fáciles de contaminar depende del objetivo: el patrón de polaridad no se generaliza al ataque de respuestas arbitrarias, donde 11B resulta más robusto que 3B en la figura 7b. Solo algunas condiciones tienen tres semillas; no debe presentarse una ley universal o monótona del tamaño. La sustitución de entidades deja referencias de resumen sin adaptar, limitación que afecta la interpretación absoluta de métricas. Las defensas basadas en pérdida dependen del checkpoint y del compromiso con datos legítimos; ninguna es garantía suficiente. La evidencia es sobre comportamiento de modelos, no sobre medición de competencia humana.

**Aplicación adoptada:** Diseñar un caso distinto de prompt injection: admisión/versionado de datos, hipótesis de acceso del atacante, comparación limpia/contaminada y pruebas con disparador y tareas benignas. Usar un experimento pequeño reproducible o snapshots precomputados claramente identificados; no exigir entrenar un modelo de 11B dentro de CyberSim.

La lectura no implica reproducción ni lectura íntegra de todos los trabajos citados.

[PDF original conservado](<Poisoning - Datos de ajuste de instrucciones.pdf>)

## Relaciones

[[Competencias frente a las familias de ataques|Q2]] · [[Registro de revisión de CyberSim]]
