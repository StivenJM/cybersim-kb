---
type: reference
status: revisado
---
# Estado comprobado del código de CyberSim

Corte de inspección estática: 13-11-2026. Proyecto: `C:\Users\stive\Documents\CyberSim`. No se ejecutó la aplicación, no se modificó código del producto y no se realizaron migraciones. “Existe” no significa validado empíricamente ni verificado en ejecución en esta revisión.

## Hallazgos

| Superficie | Evidencia local examinada | Interpretación |
| --- | --- | --- |
| Contrato de intento | `packages/scenario-contract/src/attempt.ts` | Versiones, diagnóstico sellado, pruebas, ayudas, entrega, adjudicación e incidencias ya tienen representación |
| Reglas del agregado | `packages/attempt-ledger/src/ledger.ts` | Conserva restricciones de estado y distinción entre pruebas del alumno/docente |
| Informe | `packages/attempt-ledger/src/report.ts` | Existe generador por dimensiones, estados, ayudas y límites; no se debe proponer su creación desde cero |
| Casos técnicos | `packages/exercises/src/andinapay/model.ts` y estructura de los otros cuatro casos | Modelos y verificadores implementados; AndinaPay inspeccionado en detalle; los otros cuatro se revisaron para cobertura y estructura, sin auditoría exhaustiva de cada rama |
| UI de AndinaPay | `apps/frontend/src/visual/features/ejercicios/components/AndinaPayCaseWorkspace.tsx` | Existe un espacio de trabajo amplio con expediente, repositorio, banco, recuperación e informe |
| Persistencia de UI | `apps/frontend/src/visual/features/ejercicios/hooks/useAndinaPayAttempt.ts` | Adaptador best-effort; puede continuar sin backend; guarda hashes y pruebas enviadas desde cliente |
| Entrega en backend | `apps/backend/src/attempt/infrastructure/AttemptController.ts` | Rechaza batería docente enviada por cliente, pero usa `server-battery-pending` con pruebas vacías |
| Referencia visible | `apps/frontend/src/visual/features/ejercicios/pages/VistaEjercicio.tsx` | Contiene botón para verificar solución de referencia; debe comprobarse su exposición por rol/modo antes de evaluar |
| Documentación | `docs/project/ejercicios/plan-implementacion.md`, `implementacion.md`, `docs/architecture/escenarios-investigativos.md` | Algunas listas mantienen “todo pendiente” mientras otros documentos y código muestran avances |

## Diferencias con consecuencias de evaluación

### Persistencia y recibo

El hook captura fallos y devuelve `null`; funciones públicas de guardado/entrega exponen `Promise<void>`. Esto exige revisar el flujo del componente antes de afirmar que una entrega visible siempre cuenta con recibo persistido. La evidencia observada permite señalar una **brecha a verificar**, no demostrar una pérdida de datos ya ocurrida.

Registrar solo el hash de la revisión no permite reconstruir por sí mismo el artefacto para corregirlo en servidor. Si existe otro almacenamiento de snapshots debe integrarse y comprobarse; no se identificó esa garantía en los archivos aquí examinados.

### Autoridad del verificador

El router distingue la batería docente y no acepta sus resultados del navegador, lo cual evita atribuirle falsamente una comprobación confiable. Pero una batería vacía pendiente tampoco acredita la corrección del artefacto. Para usar resultados calificatorios deberá ejecutarse una comprobación sobre el snapshot entregado en un entorno confiable.

### Autoría de las pruebas

`recordTests` recorre todos los checks de un `ExerciseReport`. Debe comprobarse si cada check representa realmente una prueba elegida por el estudiante o una batería automática de la UI. No equiparar ambos por conveniencia de serialización.

### Ayudas y exposición a soluciones

El contrato permite ayudas y el informe las representa. La interfaz pública del hook inspeccionado no expone una operación específica para registrarlas. Esto no prueba que ningún otro componente lo haga: requiere seguir los adaptadores y eventos de cada vista.

La solución de referencia puede utilizarse en autoría y revisión docente; debe quedar excluida del acceso del estudiante durante la evaluación. Si se produce una exposición, debe registrarse para interpretar qué desempeño puede atribuirse al estudiante. Es necesario verificar rutas, roles e integración, no resolverlo ocultando un botón solamente.

## Implicación

El siguiente trabajo es una integración verificable de capacidades existentes y cierre de brechas. La arquitectura futura debe construirse a partir del estado real, no de checklists desactualizadas. Véase [[Ruta de programación de CyberSim]].
