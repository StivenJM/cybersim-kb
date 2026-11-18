---
type: implementation
status: propuesto
---
# Ruta de programación de CyberSim

## Resultado que debe producir la siguiente versión

Un estudiante puede investigar y resolver un caso en el contexto 3D, entregar un artefacto recuperable, recibir un recibo y obtener un informe con evidencia y límites. El docente puede reconstruir la actuación relevante y revisar decisiones sin confundir exposición previa a soluciones, ayuda o errores técnicos con dominio autónomo.

La ruta es el resultado de la revisión cerrada y de la inspección estática. Es una especificación propuesta para implementar y validar; no una acreditación profesional ya demostrada. El encargo actual se limita a investigación y documentación.

## Secuencia y aceptación

| Prioridad | Trabajo concreto | Reutilizar / superficie | Criterio de aceptación |
| --- | --- | --- | --- |
| 1 | Conciliar inventario de implementación y fijar condiciones de evaluación | Documentos del conjunto 2.0, manifiestos y rutas actuales | Cada capacidad figura como existente, parcial o pendiente con evidencia; el intento evaluativo y la familiarización con la interfaz tienen condiciones explícitas |
| 2 | Cerrar entrega persistente de AndinaPay | `useAndinaPayAttempt`, workspace, contrato y almacén | La UI distingue borrador local, guardado y entrega confirmada; desconexión/reintento no producen confirmación falsa ni pérdida silenciosa |
| 3 | Persistir snapshot y verificarlo en servidor según el uso | `AttemptController`, servicio y verificadores | Se corrige exactamente la revisión entregada, con batería docente versionada; el cliente no declara el resultado docente |
| 4 | Registrar procedencia de pruebas, exposición y ayudas | Ledger y adaptadores UI | Puede distinguirse prueba elegida, batería automática, pista y solución de referencia; reset no borra exposición |
| 5 | Integrar informe docente y revisión humana | `buildAttemptReport`, adjudicación y vistas | Cada nivel remite a evidencia; solución alternativa entra a revisión; quedan estados NE/incidencia y desacuerdos |
| 6 | Añadir trazabilidad de las capacidades evaluadas y variantes | Contrato/manifiestos y autoría de casos | Capacidad y tarea tienen versión; una variante nueva observa la misma afirmación sin regalar el mecanismo |
| 7 | Llevar las vistas específicas de los otros cuatro casos al monitor | ECS/oficina/monitor y dominios existentes | Las acciones generan artefactos/evidencia del caso y acceso por teclado equivalente; no basta una tabla de solución de referencia |
| 8 | Pilotar y corregir el instrumento | Exportación de evidencia, rúbricas y revisión experta | Se documentan interpretación, consistencia, barreras y cambios, sin atribuir a los resultados un alcance de competencia mayor que el comprobado |
| 9 | Ampliar cobertura de amenazas | [[Competencias frente a las familias de ataques]] | Cada nuevo caso tiene mecanismo, propiedad, contraste legítimo/adversario, rúbrica y limitaciones |
| 10 | Implementar decisión del perfil si el uso y la evidencia lo permiten | Resultado agregado versionado | Regla explícita y justificada, cobertura suficiente, incertidumbre y revisión de decisiones |

Las prioridades 2–5 pueden planificarse en incrementos pequeños, pero la aceptación de un intento evaluativo requiere sus dependencias. El piloto sirve para comprobar el instrumento; sus limitaciones deben quedar visibles y sus resultados no deben presentarse como una certificación profesional validada.

## Primer incremento programable

**Objetivo:** AndinaPay de extremo a extremo, con evidencia recuperable y entrega confirmada.

1. Revisar el flujo real entre reducer local y ledger; localizar dónde se pierde o se ignora el resultado del guardado.
2. Hacer que guardado/entrega devuelvan un resultado tipado consumido por la UI. Persistir snapshot o referencia inmutable recuperable además del hash.
3. Mantener `operationId` entre reintentos de la misma operación y tratar explícitamente conflictos de revisión.
4. Ejecutar comprobaciones docentes sobre la revisión congelada; conservar la batería aparte de las pruebas elegidas por el estudiante.
5. Mostrar recibo de entrega confirmado y ofrecer el informe a revisión docente.

Antes de programar, verificar si otra ruta ya aporta snapshots o confirmación; la inspección actual detecta una brecha de garantía, no prueba que no exista ninguna implementación alternativa.

## Verificación técnica relevante

- Fallo antes y después de persistir; reintento de la misma entrega; dos revisiones en conflicto.
- Snapshot y hash corresponden a lo recibido; no puede reemplazarse una entrega cerrada mediante un nuevo cliente.
- Una batería docente manipulada desde el navegador no genera evidencia docente aceptada.
- Una pista revelada, incluso tras reset, permanece en el historial de exposición.
- Ruta alternativa correcta pasa por propiedades; falsa mitigación que rompe negocio falla el contraste.
- Interfaz y acceso por teclado presentan los mismos artefactos y decisiones.

No ejecutar suites que resetean bases reales para esta revisión documental. Las pruebas del código que se implemente después deberán correr en el entorno preparado para esa tarea.

## Qué ve cada participante

El estudiante ve expediente, herramientas del caso, estado de guardado, resultados factuales, ayudas disponibles y entrega. El docente ve evidencias, revisiones, condiciones y adjudicación. El investigador ve datos minimizados y versiones para estudiar el instrumento.

La propuesta se limita a las herramientas necesarias para que el estudiante investigue, resuelva y entregue evidencia del caso. La documentación y cualquier asistencia permitida se definen antes del intento y se registran. La revisión de autoría y las soluciones de referencia deben quedar separadas del acceso del estudiante evaluado.

## Condiciones de ejecución de la siguiente fase

La cuota bibliográfica y las lecturas centrales están completadas con el alcance del [[Registro de revisión de CyberSim]]. El siguiente trabajo es desarrollo y pilotaje, con las siguientes decisiones operativas propuestas: alumnado de final de carrera con formación previa en los contenidos evaluados, pilotaje del instrumento y documentación permitida. Antes de calificar con consecuencias se fija institucionalmente el estándar, las herramientas y la política de asistencia.

## Backlog con dependencias

| Entrega | Dependencia | Archivos de partida | Verificación decisiva |
| --- | --- | --- | --- |
| Persistencia con recibo | Condiciones del intento evaluativo y del pilotaje | `useAndinaPayAttempt.ts`, `AndinaPayCaseWorkspace.tsx`, ledger/store/service | Desconexión antes/después del commit; mismo ID al reintentar; no muestra entregado sin acuse |
| Snapshot congelado | Persistencia | Contrato y almacenamiento de intentos | Hash coincide; reconstrucción del estado exacto; revisión cerrada no se sustituye |
| Batería docente real | Snapshot | `AttemptController.ts`, `verifyAndinaPay` en `model.ts` | Cambiar resultados o revisiones en cliente no modifica la evidencia docente; fallos de infraestructura no pasan como seguridad |
| Procedencia de evidencia | Eventos de tareas | Hook y ledger | Elegir un test registra intención y entrada; una batería automática no cuenta como elección del alumno |
| Ayudas y referencia | Modo y eventos persistentes | `VistaEjercicio.tsx`, exposición del ledger | La referencia queda en autoría/revisión docente; evaluación aplica la política de ayudas también en servidor; recarga/reset no inventa autonomía |
| Informe adjudicable | Evidencia y batería | `packages/attempt-ledger/src/report.ts` | Conserva texto, discrepancias y estados; nivel humano enlaza evidencia y versión; apelación no borra historia |
| Casos y cobertura | Integración AndinaPay | Dominios existentes y manifiestos | Cada vista produce los artefactos de su mecanismo y declara lagunas; variantes revisadas por expertos |
| Pilotaje y decisión del perfil | Instrumento estable | Exportaciones y blueprint | Corrección independiente, análisis de variación, corte documentado y revisión de casos frontera |

Los nombres de servicios nuevos, almacenamiento o rutas HTTP deben decidirse durante implementación según los adaptadores existentes. No se propone una migración concreta sin comprobar antes las garantías del almacén actual.
