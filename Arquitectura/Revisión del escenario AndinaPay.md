---
type: decision
status: propuesto
---
# Revisión del escenario AndinaPay

## Dictamen de la revisión

AndinaPay es pertinente para evaluar diagnóstico y recuperación frente a claves embebidas si la evidencia exige explicar **por qué se recuperan datos concretos**, qué protege la mitigación y qué exposición histórica permanece. No basta encontrar un texto parecido a una clave ni seguir una ruta de clics.

La ficha canónica actual de CyberSim ya mejora varios problemas del relato aportado: incluye revisiones históricas, claves y registros sintéticos diferenciados, AES-GCM real, recuperación operacional y copia histórica. El análisis siguiente distingue el relato original de lo ya especificado/implementado.

## Coherencia y causalidad

| Elemento del relato recibido | Problema | Tratamiento recomendado y estado local |
| --- | --- | --- |
| El volcado aparece en claro y después se dice que está cifrado | No está claro qué material recibe el analista y qué se debe probar | La ficha actual distingue un aviso con un fragmento y un adjunto cifrado. Mantener artefactos separados y su procedencia |
| “No hay evidencia de intrusión” | Puede interpretarse como prueba de ausencia de acceso | Limitarlo a fuentes y ventana disponibles; permitir que el alumno declare lo desconocido |
| “Algoritmo robusto” | Una pista útil puede convertirse en respuesta sugerida | Aportar especificación del esquema y solicitar contraste sobre clave, modo y uso; no puntuar sospecha inicial del algoritmo como error irreversible |
| “El repositorio está disponible” | Conocer el historial no demuestra cómo salió el volcado | Separar recuperabilidad de datos de explicación de su adquisición; no inventar vector de exfiltración |
| “Contener antes de que salga todo” | Puede prometer recuperar confidencialidad ya perdida | Exigir reducción de exposición futura e inventario de copias; no declarar saneada una copia que ya posee el tercero |
| Ruta esperada fija | Penaliza investigación válida por otro orden | Evaluar evidencia y propiedades finales; el historial de acciones aporta contexto |

Estos son contrastes técnicos y decisiones de autoría. No dependen de asumir una frecuencia de ataques que esta revisión no ha comprobado.

## Matriz de evidencias del caso

| Dimensión vigente | Evidencia suficiente candidata | Falso éxito que debe distinguirse |
| --- | --- | --- |
| D1 Diagnosticar | Cita revisión histórica y relaciona clave concreta con registros | Confundir ID público con secreto; señalar “cifrado inseguro” sin mecanismo |
| D2 Explicar/decidir | Explica acceso a clave + copia cifrada, alcance y límites causales | Afirmar que encontró al intruso o dedujo el canal de fuga sin prueba |
| D3 Intervenir | Custodia restringida, nueva clave, migración verificada y retiro operacional de la anterior | Borrar literal del HEAD, cambiar variable o cambiar algoritmo sin recuperación coherente |
| D4 Verificar/delimitar | Conserva función, compara registros, explica exposición de copia histórica | Un mensaje verde aislado; dejar ilegibles los datos o bloquear toda operación |

Las claves deben ser sintéticas y los permisos del simulador deben declararse como modelo educativo. Los fixtures públicos del navegador no constituyen una bóveda de secretos frente a quien inspeccione el bundle.

## Pruebas de contraste

1. La clave expuesta recupera R01/R02 del snapshot histórico y no R03 de otra clave.
2. Clave, tag o AAD incorrectos fallan sin texto parcial.
3. La operación legítima continúa tras rotación y migración; las referencias apuntan al material correcto.
4. La copia histórica continúa descifrable con K1: rotación no modifica bytes que ya salieron.
5. Cambiar solo HEAD no supera la recuperación ni la prevención de recurrencia.
6. Un fallo técnico del banco no se interpreta como rechazo seguro ni ausencia de conocimiento.
7. Una recuperación alternativa que satisface las propiedades no pierde puntos por su nombre o secuencia.

Varias comprobaciones ya forman parte del modelo/verificador actual; deben conservarse y vincularse a la actuación del estudiante. La batería del corrector no demuestra que el alumno eligió esas pruebas.

## Variantes para generalización

Proponer un segundo caso con mecanismo equivalente y otros nombres/datos, y un contraste con identificador público legítimo. Variar historial, custodias o registros exige comprobar que la dificultad y conocimientos requeridos siguen siendo comparables. Cambiar solo colores, empresa o clave no prueba transferencia.

Si se quiere concluir competencia de desarrollo seguro más amplia, añadir tareas preventivas: revisar un cambio propuesto, justificar una excepción, detectar una implementación que externaliza la clave pero conserva permisos excesivos. Es contenido nuevo sujeto a especificación y revisión, no parte ya acreditada del escenario.

## Fuentes y límites

[[Secretos - Prácticas de gestión]], [[Secretos - Dificultades de desarrolladores]], [[Secretos - Comparación de detectores]] y [[Secretos - Límites de los escáneres industriales]] son antecedentes técnicos; sus niveles de lectura están registrados en las fichas; la revisión de prácticas de secretos se leyó completa. No se atribuyen ensayos educativos a los estudios técnicos. [[Referencias institucionales de CyberSim]] sustenta las definiciones. El estado concreto de producto está en [[Estado comprobado del código de CyberSim]].

## Relato revisado para la vista del estudiante

AndinaPay es una fintech quiteña de doce personas. Su plataforma almacena identificadores y tokens de pago cifrados. La gerencia recibe un aviso con dos registros sintéticos en claro y un archivo adjunto que se presenta como una copia cifrada de la aplicación. Todavía no se ha establecido quién obtuvo esas copias ni por qué medio.

Las fuentes de monitorización disponibles no muestran accesos anómalos durante la ventana que cubren; eso no descarta eventos fuera de ella ni accesos no registrados. El equipo admite una revisión apresurada antes de la demo. Dispones de un repositorio con historial, artefactos de configuración y un banco de comprobación autorizado.

Tu responsabilidad es establecer qué mecanismos de exposición puedes demostrar con estos materiales, qué registros quedan afectados y qué no puedes concluir. Debes proponer y ejecutar en el entorno simulado una recuperación que conserve las operaciones legítimas, justificar las prioridades y comunicar el riesgo residual. La procedencia de la filtración queda abierta salvo que encuentres evidencia suficiente.

Las claves, personas y registros del caso son sintéticos. La jornada del relato es contexto de crisis; el límite real del intento se comunica por separado y se ajusta en el piloto. No se promete que una rotación vuelva confidencial una copia que ya salió de la organización.

## Anclajes de corrección propuestos

| Dimensión | 0: evidencia evaluable insuficiente | 1: parcial | 2: desempeño suficiente candidato | 3: desempeño ampliado |
| --- | --- | --- | --- | --- |
| D1 | Atribuye la causa sin evidencia o no localiza mecanismo | Encuentra un literal pero no lo vincula con uso y datos | Cita historial, uso y relación clave-registros mediante contraste | Además distingue falsos positivos, hipótesis alternativas y cobertura de fuentes |
| D2 | Asegura actor/vector o ruptura del algoritmo sin pruebas | Reconoce clave expuesta sin delimitar impacto | Explica recuperación y separa exposición demostrada de origen desconocido | Prioriza alternativas y explicita supuestos y riesgo histórico |
| D3 | No corrige o inutiliza operación legítima | Retira literal/rota de forma incompleta | Migra y retira uso operativo anterior, con custodia y permisos correctos | Justifica recuperación, fallos parciales y prevención de recurrencia |
| D4 | Declara seguro sin contraste | Ejecuta un ejemplo y generaliza | Elige pruebas adversarias y legítimas sobre la entrega e interpreta alcance | Busca variantes, errores de oráculo y exposición residual con límites precisos |

**NE, incidencia técnica y ausencia de oportunidad son estados separados de 0.** El nivel 2 es un anclaje de autoría que debe contrastarse con entregas de muestra, corrección independiente y pilotaje; no es un umbral profesional validado. Las dimensiones se juzgan por evidencia individual, no por cantidad de texto.

El informe breve responderá: hallazgo y evidencia; mecanismo; registros afectados y comparación; medida y verificación; qué permanece expuesto; qué se desconoce. No exige redactar un informe forense legal ni identificar al atacante.

## Aceptación del diseño del caso

El verificador debe rechazar al menos las falsas soluciones de borrar solo HEAD, rotar sin migrar, bloquear toda lectura y declarar protegida la copia histórica. Debe admitir cambios alternativos que cumplan las propiedades. El piloto incluirá entregas deliberadamente engañosas y soluciones válidas distintas para revisar los anclajes. Esto determina qué falta programar sin atribuir a la literatura una única interfaz o solución.

## Uso de la guía común

[[Guía para evaluar las competencias de seguridad]] explica cómo conservar evidencias, distinguir pruebas del estudiante y del corrector, registrar ayuda y revisar soluciones alternativas. Esta ficha sigue siendo la referencia del mecanismo, relato y anclajes de AndinaPay; la guía común no crea otra rúbrica numérica para el caso.
