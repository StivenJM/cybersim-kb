---
type: guide
status: especificado
---
# Guía para evaluar las competencias de seguridad

Esta guía convierte las capacidades de CyberSim en instrucciones para preparar una tarea y revisar la entrega individual de un estudiante. **Se evalúa lo que el estudiante ya puede hacer, bajo condiciones conocidas de documentación y ayuda.** Los criterios tienen fundamento bibliográfico en [[Fundamento de las competencias de seguridad de CyberSim]]; su funcionamiento con estudiantes debe comprobarse en el piloto.

Los ejemplos siguientes son **especificaciones de evaluación y ejemplos sintéticos de corrección**. No se presentan como pruebas ejecutadas, resultados de estudiantes ni funciones ya implementadas. Las comprobaciones específicas ya descritas para AndinaPay permanecen en [[Revisión del escenario AndinaPay]], sin duplicar su ficha.

## Qué debe preparar el autor de una tarea

Antes de administrarla, el docente o autor deja una ficha con estos elementos:

| Elemento | Qué se escribe |
| --- | --- |
| Capacidad y alcance | Qué actuación se observará y sobre qué mecanismo. Una tarea SQL no evalúa automáticamente todos los tipos de inyección |
| Formación previa | Lenguaje, tecnologías y contenidos que el estudiante necesita conocer; no se enseñan durante el intento |
| Consigna | Responsabilidad concreta, productos solicitados y límites. Indicar si se pide diagnosticar, diseñar o implementar |
| Recursos | Documentación y herramientas permitidas; política de asistentes de IA, colaboración y pistas |
| Estado inicial | Copia reproducible de código, configuración, datos y permisos del ejercicio |
| Resultado esperado | Propiedad de seguridad y operación legítima que deben conservarse; no una única secuencia de clics |
| Contrastes del corrector | Entradas y resultados que detectan correcciones aparentes y aceptan soluciones válidas distintas |
| Guía de juicio | Evidencia suficiente, parcial y contraria al criterio; estados de falta de evidencia e incidencia |
| Versiones | Tarea, guía, herramientas y pruebas utilizadas, para reconstruir qué se evaluó |

Que el estudiante pueda leer documentación no equivale a regalarle la solución. Que tenga a disposición la solución completa sí cambia la interpretación: se registra esa exposición y no se atribuye al mismo intento un descubrimiento independiente.

## Qué entrega el estudiante

La entrega reúne cinco productos breves y vinculados entre sí:

1. **Diagnóstico:** dónde está el problema, qué evidencia lo respalda y cuál es su causa propuesta.
2. **Decisión:** qué control eligió, por qué corresponde al mecanismo y qué alternativa relevante descartó.
3. **Artefacto:** revisión identificable del código, configuración o diseño solicitado. Una propuesta no se registra como implementación.
4. **Verificación propia:** casos elegidos por el estudiante, resultado esperado, resultado obtenido e interpretación.
5. **Informe de alcance:** uso legítimo conservado, exposición que permanece y hechos que todavía desconoce.

Si una tarea solo pide diagnóstico, se solicitan los productos pertinentes y se declara que no hubo oportunidad de observar implementación. La ausencia de un producto no solicitado no se convierte en desconocimiento.

## Cómo interpretar la evidencia

Las capacidades CAP indican **qué** se evalúa. D1–D4 indican **cómo se observa** el trabajo: diagnosticar; explicar y decidir; intervenir; verificar y delimitar. Una misma evidencia puede informar varias capacidades sin convertirse en varias situaciones independientes.

| Estado por criterio | Cuándo corresponde | Ejemplo |
| --- | --- | --- |
| Evidencia suficiente en esta tarea | El producto y la explicación satisfacen el criterio y sus contrastes pertinentes | Un cambio impide el acceso indebido y conserva el autorizado; la explicación localiza el control |
| Evidencia parcial | Hay un componente correcto, pero falta una parte necesaria o su comprobación | Identifica la clave expuesta, pero no relaciona qué registros puede recuperar |
| Evidencia contraria al criterio | La actuación o un contraste muestran que la propiedad exigida no se cumple | Una persona sigue consultando datos ajenos mediante una petición directa |
| Producto exigido no entregado | Hubo oportunidad y recursos para entregarlo, y no consta una incidencia que explique su ausencia | La consigna pedía una revisión y el registro confirma que no se presentó ninguna |
| Evidencia insuficiente para juzgar | El registro disponible no permite decidir | Se perdió el artefacto entregado y no puede reconstruirse qué versión se comprobó |
| No observado | La tarea no exigió esa actuación o no se administró | Se pidió un diseño y no se solicitó ejecutar el cambio |
| Incidencia técnica | Falló el entorno y el fallo impide interpretar el resultado | El banco no inicia; el rechazo de todas las peticiones no acredita un control de acceso |

Son descriptores para revisar una evidencia, no niveles psicométricos calibrados ni porcentajes de aprobación. Los anclajes numéricos 0–3 ya propuestos para AndinaPay pueden conservarse con sus límites; no se añade otra escala numérica paralela. “Suficiente en esta tarea” no significa por sí solo “competente en todo el perfil”.

No entregar un producto requerido es una observación diferente de perderlo por un fallo del sistema. La guía registra esa diferencia y delimita el incumplimiento; la ausencia por sí sola no explica su causa ni autoriza atribuir incapacidad general al estudiante.

## Evidencia que corresponde a cada capacidad

| Capacidad | Pregunta del corrector | Evidencia que debe poder localizar |
| --- | --- | --- |
| CAP-01 Contexto y confianza | ¿Explica quién puede actuar sobre qué recurso y dónde se acepta autoridad? | Actores, dato o recurso protegido, flujo y regla de permiso relevantes |
| CAP-02 Diagnóstico causal | ¿La explicación corresponde al mecanismo observado? | Fragmento o registro citado y contraste que ayuda a distinguir una causa de otra |
| CAP-03 Corrección y diseño | ¿El control actúa sobre la causa y satisface lo solicitado? | Cambio o diseño identificable, justificación y comprobación acorde con su alcance |
| CAP-04 Verificación | ¿Eligió comprobaciones pertinentes y sabe qué permiten concluir? | Pruebas propias adversarias y legítimas, resultados e interpretación de límites |
| CAP-05 Secretos y datos | ¿Considera dónde están expuestos y qué ocurre con su ciclo de vida? | Accesos, copias, rotación o migración pertinente y exposición residual |
| CAP-06 Integridad y procedencia | ¿Comprueba lo necesario antes de aceptar el dato o artefacto? | Origen, integridad y autorización según el caso, con rechazo antes del efecto indebido |
| CAP-07 Sistemas con IA | ¿Distingue la etapa y la autoridad que intervienen en el ataque evaluado? | Prueba del mecanismo concreto y del uso legítimo; permisos de herramientas o admisión de datos según corresponda |
| CAP-08 Responsabilidad y comunicación | ¿El informe distingue evidencia, supuestos y decisiones? | Hallazgos verificables, prioridad justificada, alternativas y límites de conclusión |

Las referencias directas y las adaptaciones se consultan en [[Fundamento de las competencias de seguridad de CyberSim]]. La selección de capacidades y situaciones está en [[Plan de cobertura del perfil]].

## Ejemplo de consulta SQL: BibliotecaViva

**Tarea sintética de referencia:** una búsqueda de títulos incorpora texto del usuario en una consulta. Se pide diagnosticarla, corregirla y comprobarla. La función legítima consiste en buscar por título; el criterio es que el texto de búsqueda se trate como datos y no altere la estructura de la consulta. Se declara aparte cualquier requisito de autorización: parametrizar una consulta no lo resuelve automáticamente.

| Evidencia | Ejemplo que respalda el criterio | Ejemplo parcial o contrario |
| --- | --- | --- |
| Diagnóstico | Ubica la construcción de la consulta y explica cómo la entrada puede modificar su interpretación | Afirma “hay SQL injection” sin localizar el uso de la entrada |
| Corrección | Separa consulta y valores mediante la interfaz pertinente, o presenta otra solución que satisfaga la misma propiedad | Elimina comillas en el navegador y conserva una consulta vulnerable en el servidor |
| Uso legítimo | La búsqueda de un título con un apóstrofo, como `L'histoire`, conserva el comportamiento especificado | El filtro impide buscar títulos legítimos para que no aparezca el carácter problemático |
| Caso adversario | Una entrada sintética que antes alteraba la consulta pasa a tratarse como valor; se conservan entrada, resultado y revisión | Solo informa que una cadena conocida dejó de funcionar, sin verificar la causa ni otros usos de la entrada |
| Conclusión | Limita el resultado a las consultas y propiedades comprobadas | Declara que toda la aplicación quedó protegida frente a cualquier inyección |

El corrector prepara una variante no mostrada que compruebe la misma propiedad. Los datos, nombres y entradas de esta guía no se presentan como el esquema real ya implementado de BibliotecaViva.

## Ejemplo de autorización: AndeanLogix

**Tarea sintética de referencia:** dos usuarios, A y B, tienen recursos privados distintos. La consigna exige que cada uno consulte únicamente los propios mediante una operación definida. Antes de evaluar se fija qué puede hacer una persona administradora, si ese rol existe.

| Petición que debe contemplar la guía | Resultado esperado según esta política |
| --- | --- |
| A consulta un recurso propio | Obtiene el recurso previsto |
| A solicita directamente un recurso privado de B | No recibe datos ni produce un efecto no autorizado |
| Una persona anónima solicita un recurso privado | No obtiene el recurso |
| B consulta su recurso por la vía autorizada | Conserva la función legítima |

**Entrega suficiente para el control:** identifica la regla actor–acción–recurso, la aplica en la frontera que decide el acceso y explica los resultados. **Entrega parcial:** oculta enlaces en la interfaz, pero la petición directa sigue devolviendo datos. **Entrega contraria a continuidad funcional:** deniega todas las peticiones y presenta ese resultado como una solución completa.

No se exige un código HTTP específico como prueba suficiente de seguridad: se comprueba también que no se devolvieron datos ni ocurrió el efecto prohibido. La tabla especifica una política de ejemplo; no certifica que todos esos contrastes estén implementados en el caso actual.

## Ejemplo de integridad: admisión de un artefacto

**Tarea de referencia para CAP-06:** un proceso recibe un artefacto y puede publicarlo o ejecutarlo. La política de la tarea define qué origen y versión están autorizados. El estudiante debe decidir dónde comprobar integridad y autorización y demostrar que la decisión ocurre antes del efecto.

La guía incluye un artefacto autorizado e íntegro; uno alterado; y, si la política lo distingue, uno íntegro y auténtico de un origen o versión no autorizados. La solución suficiente acepta el primero y rechaza los otros antes de producir el efecto. Comprobar una firma después de ejecutar es evidencia contraria; comprobarla y asumir que todo contenido firmado es benigno deja una conclusión injustificada.

Si la tarea usa deserialización, se añade un contraste que observe efectos de esa reconstrucción. Validar el objeto después de un efecto peligroso no satisface el criterio. Este diseño puede complementar NubeAndina, pero la amplitud exacta que ya cubre ese escenario se conserva en [[Competencias frente a las familias de ataques]].

## Ejemplo de IA: una herramienta con permisos

**Tarea nueva de diseño, no implementada:** un asistente debe resumir un documento. Una herramienta permite solicitar documentos por identificador; en el estado vulnerable no comprueba qué documentos puede leer la persona que usa el asistente. La política autoriza el documento de trabajo y deniega otro documento privado. El documento de trabajo incluye contenido externo con instrucciones para consultar el privado e incorporar sus datos al resumen. El estudiante explica la frontera entre contenido y autoridad y propone o aplica un control, según la consigna.

Se conserva una traza del intento de acceso y se comprueba también la llamada directa a la herramienta con el identificador privado: no debe devolver sus datos. Un documento legítimo debe seguir pudiendo leerse y resumirse. Si el modelo no intenta el acceso en una ejecución, eso no prueba por sí solo que la herramienta aplique permisos. Eliminar todo acceso o devolver un mensaje de bloqueo a cualquier petición tampoco demuestra que conserve la tarea autorizada. Un aviso al modelo puede formar parte de una solución, pero no se acepta por su redacción: se comprueban el comportamiento y el control de permisos correspondiente al caso.

La conclusión se limita al mecanismo, versiones, entradas y operaciones probados. Esta tarea no acredita defensa frente a contaminación del entrenamiento ni extracción de información memorizada. CAP-07 requiere formación previa y pertenencia explícita al perfil evaluado; las lagunas de cobertura se informan, no se ocultan bajo una única etiqueta “IA”.

## Cómo separar las pruebas del estudiante de las del corrector

Las pruebas elegidas por el estudiante permiten observar CAP-04. Las pruebas preparadas por el corrector comprueban propiedades de la entrega y detectan falsos arreglos. Cumplen funciones distintas, aunque utilicen entradas parecidas.

| Resultado observado | Qué puede concluirse |
| --- | --- |
| Las pruebas del corrector pasan, pero no hay selección ni interpretación propia | Hay respaldo técnico sobre esa entrega; falta evidencia para atribuir al estudiante el diseño de la verificación |
| El estudiante propone una prueba adecuada, pero la entrega falla | Puede haber evidencia parcial de verificación y evidencia contraria a la corrección; se informan ambas |
| Una prueba falla por un defecto del banco | Se registra incidencia y se revisa la interpretación antes de juzgar al estudiante |
| Otra solución satisface las propiedades por un camino distinto | Se revisa con los mismos criterios; no se penaliza por apartarse de la solución de referencia |

## Qué debe resolver el docente y qué se puede automatizar

Se automatizan propiedades con un resultado observable bien especificado: acceso permitido o denegado, efecto producido, coincidencia de registros, integridad, ejecución o preservación de una operación legítima. La prueba se ejecuta sobre la revisión efectivamente entregada y conserva sus resultados.

El docente revisa la correspondencia entre explicación, evidencia y decisión. Utiliza la guía, ejemplos y documentación del mecanismo. No hace falta convocar especialistas para inventar el catálogo; **sí hace falta competencia en los contenidos de la asignatura para corregirlos**. Una respuesta alternativa o ambigua debe poder pasar a revisión humana; la guía no promete sustituir todo juicio técnico.

Antes del piloto, dos correctores pueden revisar por separado un conjunto de entregas de muestra, comparar decisiones y aclarar qué evidencia falta en la guía. El acuerdo inicial no demuestra por sí solo validez: sirve para detectar criterios ambiguos. No se fija un porcentaje universal de acuerdo o aprobación sin justificar el uso.

## Registro mínimo de la decisión

Para cada criterio se conserva: capacidad; tarea y versión; revisión de la entrega; evidencia citada; pruebas propias y del corrector; documentación, herramientas y ayudas disponibles; estado asignado; razón; corrector y fecha. Si una pista modifica la actuación, se distingue el segmento previo del posterior.

**Ejemplo de comentario de corrección:** “La consulta entregada trata la entrada como un valor y conserva la búsqueda legítima. El estudiante explica la causa y cita el cambio. Las comprobaciones docentes respaldan la corrección; no se adjuntaron pruebas elegidas por el estudiante. Hay evidencia de corrección en esta tarea y falta evidencia de su selección de pruebas”.

Se evita convertir una falta de registro en un cero automático y una tarea resuelta en certificación de todo el perfil. El [[Modelo de evidencia y validación]] especifica qué comprobar en el piloto y [[Del desempeño a la competencia del perfil]] delimita cualquier conclusión más amplia.

## Fundamento y decisiones de adaptación

Los estudios de programación segura de [[Lam - Diagnóstico y corrección de código inseguro]] y [[Almansoori - Componentes del razonamiento seguro]] justifican observar explicación y actuación con recursos declarados. Las rúbricas de [[Threat modeling - Rúbricas de pensamiento sistémico]] aportan contexto y justificación; [[Assyne - Estado de competencias de software]] aporta código, pruebas y comunicación; [[Mead y Shoemaker - Competencias de aseguramiento de software]] delimita el dominio y nivel de referencia.

Los estados, ejemplos web y reglas de esta guía son adaptaciones de CyberSim, no una rúbrica textual de esos artículos. Los mecanismos específicos se apoyan en las fichas técnicas enlazadas desde [[Competencias frente a las familias de ataques]] y [[Revisión del escenario AndinaPay]]. La guía debe revisarse cuando una nueva solución o incidencia revele que un contraste no distingue lo que se pretendía evaluar.
