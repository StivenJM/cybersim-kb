---
type: paper
year: 2025
lectura: resumen-conclusiones
preguntas: [Q2]
---
# XSS - Detección semántica y límites

**P105. XSShield: Defending Against Stored XSS Attacks Using LLM-Based Semantic Understanding.**

[Fuente original o ficha de autor](https://www.mdpi.com/2076-3417/15/6/3348) · Consulta: 13-11-2026.

## Aporte

Propone detección de XSS persistente mediante LLM y grafos de dependencias.

## Límite y valoración

Modelo y benchmark concretos; tiempo anunciado excluye comunicación con el modelo.

## Decisión para CyberSim

Distinguir almacenamiento, ejecución y contexto de salida; no sustituir codificación segura por un clasificador. Esta aplicación es una inferencia de diseño local; no un resultado experimental en CyberSim.

## Alcance de lectura

**resumen-conclusiones**. Cuenta en la cuota reciente.

Abstract turn297view0; cierre Hconc0.

Cribado de abstract y cierre, con pasajes adicionales cuando fueron necesarios para comprobar relevancia o limitaciones. No se atribuye lectura completa del cuerpo.

## Relaciones

[[Competencias frente a las familias de ataques|Q2]] · [[Registro de revisión de CyberSim]]
