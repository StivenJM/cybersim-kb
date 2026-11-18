---
type: paper
year: 2022
lectura: texto-completo
preguntas: [Q2, Q3]
revision_competencias: "2026-11-16"
---
# Secretos - Prácticas de gestión

**P036. What are the practices for secret management in software artifacts?.**

[Fuente original o ficha de autor](https://bradreaves.net/publication/bnrw22/) · Consulta: 13-11-2026.

## Aporte

Revisión de literatura gris que identifica 24 prácticas organizadas en seis categorías.

## Límite y valoración

Popularidad de una práctica no es eficacia comparativa ni evidencia sobre evaluación educativa.

## Decisión para CyberSim

AndinaPay debe considerar custodia, despliegue, escaneo y ciclo de vida; no solo borrar el literal. Esta aplicación es una inferencia de diseño local; no un resultado experimental en CyberSim.

## Alcance de lectura

**texto-completo**. Cuenta en la cuota reciente.

PDF completo de ocho páginas; secciones I-VI, referencias y figuras 1-2

Tablas: No hay tablas de resultados adicionales; 24 prácticas y seis categorías leídas en el cuerpo

Figuras: Figuras 1-2 inspeccionadas visualmente en PDF local

## Análisis crítico propio

Es una revisión de 54 artefactos grises, no 54 experimentos: las frecuencias de recomendaciones no estiman eficacia ni adopción. Algunas frases confunden servicios de secretos con módulos hardware y atribuyen capacidades exclusivas sin comparación contemporánea. No importar restricciones de forks como remedio universal, ni asumir que una variable de entorno ya proporciona custodia segura. La vida corta de una credencial de acceso y la pérdida de una clave de cifrado sobre una copia antigua tienen consecuencias distintas.

**Aplicación adoptada:** AndinaPay debe observar historial, custodia, rotación, migración, permisos y prevención verificables. Separar exposición histórica irreversible de recuperación operacional.

La lectura del artículo no implica reproducir sus experimentos, auditar sus datos ni leer íntegramente todos los trabajos citados. Los materiales externos no recuperados se declaran en [[Registro de revisión de CyberSim]].

[PDF original conservado](<Secretos - Prácticas de gestión.pdf>)

## Relaciones

[[Competencias frente a las familias de ataques|Q2]] · [[Selección y adaptación de marcos de competencias|Q3]] · [[Registro de revisión de CyberSim]]

## Revisión focalizada de competencias · 16-11-2026

**Función en la selección:** especialización técnica. Representar exposición, almacenamiento, rotación y recuperación de secretos; las prácticas sintetizadas no son una escala de estudiantes ni una comparación experimental.

Pasajes comprobados: Abstract p. 1; §VI Conclusion. [Acceso consultado](https://bradreaves.net/publication/bnrw22/bnrw22.pdf). Esta nueva comprobación de abstract y cierre no implica una segunda lectura íntegra de todos los materiales declarados en la fase anterior.

[[Fundamento de las competencias de seguridad de CyberSim]] · [[Revisión focalizada de competencias de seguridad]]
