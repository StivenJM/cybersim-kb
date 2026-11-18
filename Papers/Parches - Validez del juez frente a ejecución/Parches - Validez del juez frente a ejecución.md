---
type: paper
year: 2026
lectura: texto-completo
preguntas: [Q1, Q2, Q4]
---
# Parches - Validez del juez frente a ejecución

**P108. Fixing, Breaking, or Faking It? An Execution-Calibrated Evaluation of LLM Vulnerability Patching in JavaScript, Python, Go, and Java, and the Limits of LLM-as-Judge.**

[Fuente original o ficha de autor](https://www.mdpi.com/2624-800X/6/5/153) · Consulta: 13-11-2026.

## Aporte

Contrasta jueces LLM con ejecución de parches y distingue neutralización de preservación funcional.

## Límite y valoración

Resultados acotados por oráculos y cobertura de pruebas; no instrumento de competencia humana.

## Decisión para CyberSim

La batería docente debe ejecutar pruebas de seguridad y regresión; acuerdo entre jueces no demuestra validez. Esta aplicación es una inferencia de diseño local; no un resultado experimental en CyberSim.

## Alcance de lectura

**texto-completo**. Cuenta en la cuota reciente.

Artículo completo: secciones 1-7, limitaciones, declaraciones, seis tablas y cuatro figuras; HTML 179-395

Tablas: Tablas 1-6 leídas completas en DOM editorial, incluida matriz de confusión

Figuras: Figuras 1-4 inspeccionadas visualmente

## Análisis crítico propio

El hallazgo útil es la necesidad de contrastar juicios con ejecución suficiente. Su oráculo también falla: pruebas positivas escasas, una sola PoC, celda CSRF frágil y SSRF dependiente de DNS offline. El denominador importa: ocho over-fixes entre 112 neutralizaciones, no ocho entre todas las vulnerabilidades; los autores rebajan a uno o dos tras revisar artefactos. Vul4J conserva una regresión entre 254 intentos bajo cobertura limitada. Hubo parada opcional en Java, muestras intencionales de modelos y posible memorización. No importar porcentajes ni una regla comercial/open ni afirmar que cualquier suite determina verdad absoluta.

**Aplicación adoptada:** Verificador confiable con regresión legítima y ataques variados; LLM como apoyo revisable, no juez final automático de competencia.

La lectura del artículo no implica reproducir sus experimentos, auditar sus datos ni leer íntegramente todos los trabajos citados. Los materiales externos no recuperados se declaran en [[Registro de revisión de CyberSim]].

## Relaciones

[[Evaluación de competencias en escenarios 3D|Q1]] · [[Competencias frente a las familias de ataques|Q2]] · [[Del desempeño a la competencia del perfil|Q4]] · [[Registro de revisión de CyberSim]]
