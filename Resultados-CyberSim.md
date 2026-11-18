---
type: report
status: cerrado
---
# Resultados de la investigación de CyberSim

**El objetivo es evaluar competencias de seguridad ya adquiridas por estudiantes con formación previa.** CyberSim les presenta problemas para que demuestren lo que saben hacer. El estudio debe comprobar si las tareas y los criterios permiten evaluar esas capacidades de forma justificada y consistente.

La recomendación es **evaluar la capacidad del estudiante para identificar, corregir y comprobar problemas de seguridad en software**. Para ello, CyberSim debe presentar casos con una organización, personas involucradas y un problema concreto que resolver. El estudiante investiga qué ocurre, explica su causa, propone o aplica una solución y realiza pruebas para comprobarla.

La evaluación se apoya en las evidencias de ese trabajo: el diagnóstico, la justificación de las decisiones, el código o la configuración que entrega y las pruebas que realiza. Las comprobaciones automáticas revisan requisitos concretos de la solución; por ejemplo, que un usuario sin permisos no pueda consultar datos ajenos y que los usuarios autorizados conserven el acceso que necesitan. El docente revisa por qué el estudiante eligió esa solución, qué alternativas consideró y qué permiten concluir sus pruebas.

El entorno 3D sirve para representar el lugar, las personas y las consecuencias del problema. La valoración de la competencia se basa en cómo el estudiante investiga y resuelve el caso, y en las evidencias que permiten comprobar su trabajo.

## ¿Cómo puede CyberSim evaluar competencias en escenarios 3D?

Cada caso debe relacionar una afirmación de capacidad con una tarea que realmente la exija y con evidencia para juzgarla. Se conservan cuatro dimensiones de observación: **D1 diagnosticar, D2 explicar y decidir, D3 intervenir, D4 verificar y delimitar**. No se presentan como cuatro factores psicométricos ya validados.

El estudiante recibe situación y recursos, formula un diagnóstico con fuentes, contrasta hipótesis, propone o aplica una corrección y entrega una revisión identificable junto a su verificación. El sistema conserva artefacto, pruebas elegidas, ayudas e incidencias.

Caminar, abrir un cajón, recoger una flag, repetir el nombre de un CWE o terminar rápido no bastan para demostrar competencia, sino que también se necesita observar cómo identifica el problema, justifica una solución y comprueba su resultado. 

Los elementos simulados del escenario deben permitir investigar el problema, modificar código o configuraciones y ejecutar pruebas, conservando resultados que puedan revisarse. Antes de evaluar, se ofrece una familiarización con los controles de la interfaz, sin explicar el mecanismo de seguridad ni la solución del caso. La validación debe comprobar que el resultado refleja las capacidades del estudiante y que la dificultad para manejar el entorno 3D no distorsiona esa valoración.

El código ya contiene una estructura para representar los intentos, un registro de sus evidencias, comprobaciones automáticas y un informe organizado por dimensiones de evaluación.

Desarrollo: [[Evaluación de competencias en escenarios 3D]], [[Modelo de evidencia y validación]], [[Estado comprobado del código de CyberSim]].

La [[Guía para evaluar las competencias de seguridad]] concreta qué debe entregar el estudiante, qué comprueba el sistema y qué revisa el docente. Incluye ejemplos de evidencia suficiente, parcial y contraria al criterio, y separa falta de registro, ausencia de oportunidad e incidencia técnica. Sus ejemplos son diseños para revisar, no resultados ya obtenidos.

## ¿Qué competencias se requieren frente a las familias de ataques más frecuentes en 2026?

**Las siguientes son las capacidades seleccionadas para evaluar a estudiantes próximos a terminar ingeniería de software, con formación previa en los contenidos del caso.** Tienen antecedentes publicados: el modelo de competencias de aseguramiento de software de Mead y Shoemaker, el catálogo de Assyne y estudios de evaluación de programación segura y modelado de amenazas. Las especializaciones se completan con literatura técnica.

| Capacidad | Qué debe demostrar el estudiante | Fundamento principal |
| --- | --- | --- |
| CAP-01 Contexto y confianza | Explicar qué se protege, quién puede actuar y por dónde circulan datos y permisos | Rúbricas universitarias de modelado de amenazas; arquitectura y visión de conjunto en Assyne |
| CAP-02 Diagnóstico causal | Localizar el problema, explicar su causa y usar una prueba que permita contrastar su explicación | Tareas de estudiantes de Lam y Almansoori; análisis de problemas en Assyne |
| CAP-03 Corrección y diseño | Entregar o proponer un control que resuelva la causa y conserve el uso autorizado | Corrección de código en Lam y Almansoori; evaluación de mitigaciones en modelado de amenazas |
| CAP-04 Verificación | Elegir pruebas de ataque y de uso legítimo, interpretar sus resultados y explicar sus límites | Pruebas en Assyne; evaluación y funcionalidad en Mead y Shoemaker; estudios de límites de detectores |
| CAP-05 Secretos y datos | Identificar exposición, proteger acceso y justificar recuperación, rotación o migración | Estudios de prácticas, dificultades y detección de secretos en repositorios |
| CAP-06 Integridad y procedencia | Comprobar origen, integridad y autorización antes de que datos o artefactos produzcan efectos | Aseguramiento de componentes en Mead y Shoemaker y su informe técnico; revisión de código en Braz y Bacchelli |
| CAP-07 Sistemas con IA | Distinguir amenazas del entrenamiento y de la ejecución, y limitar el uso de datos y herramientas | Dominios de SecureAI; mecanismos y contrastes técnicos de AgentDojo y estudios de contaminación del entrenamiento |
| CAP-08 Responsabilidad y comunicación | Informar hechos, justificar prioridades y alternativas, y expresar riesgo residual e incertidumbre | Comunicación y necesidades del usuario en Assyne; riesgo en Mead y Shoemaker; justificación en las rúbricas de amenazas |

**Cada capacidad tiene antecedentes publicados y una adaptación explícita.** Los IDs y la agrupación en ocho capacidades pertenecen a CyberSim; todavía debe comprobarse cómo funcionan como instrumento de evaluación. CAP-07 es una extensión para los escenarios de IA: se exige formación previa correspondiente y se declara antes de evaluar. No se considera una exigencia universal para todo estudiante de software.

La evaluación se concreta por mecanismo: corregir SQL no acredita XSS; autenticación no acredita autorización; una firma no prueba que el contenido sea benigno; una prueba de prompt injection no acredita defensa frente a contaminación del entrenamiento. La responsabilidad se observa en decisiones e informes, sin inferir personalidad.

La lista de ataques proporcionada contiene **24 entradas y 22 CWE distintos**, porque 502 y 345 se repiten. La frecuencia procede del estudio del compañero; esta revisión no certifica que sean las ocho familias más frecuentes mundialmente. Los cinco escenarios investigativos no cubren todavía todo ese alcance.

Desarrollo y fuentes por capacidad: [[Fundamento de las competencias de seguridad de CyberSim]], [[Competencias frente a las familias de ataques]] y [[Plan de cobertura del perfil]].

## ¿Qué se tomó del paper de competencias y por qué se complementó?

**Sí se utilizan las competencias pertinentes del paper de Assyne:** lectura y construcción de código, pruebas, arquitectura, análisis y resolución de problemas, comunicación, necesidades del usuario y calidad. Se convierten en actuaciones concretas de seguridad. Por ejemplo, “escribir pruebas” se observa cuando el estudiante elige casos de ataque y de uso legítimo y explica qué demuestran.

No se puntúan liderazgo y trabajo en equipo porque esta prueba individual no ofrece evidencia suficiente de esas capacidades. Formación y experiencia son condiciones previas. Motivación, autoestima, diversión u orgullo no se deducen de una entrega. Esto delimita el instrumento; no significa que esas competencias sean irrelevantes para la profesión.

El modelo de aseguramiento de software de Mead y Shoemaker aporta una referencia explícita para pregrado. Los estudios de programación segura y amenazas aportan tareas y criterios; los estudios técnicos fundamentan secretos, integridad e IA. **La selección queda justificada documentalmente ahora**, sin depender de que especialistas inventen después las competencias. Comprobar que el instrumento las evalúa de forma consistente sigue siendo necesario.

Se documentó cada expresión de los once grupos de la tabla 12a de Assyne, con su decisión y razón. El artículo declara 49 competencias; nuestra correspondencia separa 52 expresiones impresas, algunas próximas entre sí, sin atribuir 52 competencias a los autores ni inventar sus identificadores.

La ampliación revisó abstract y cierre de **50 publicaciones distintas**, 47 ya registradas y tres incorporadas. El registro declara lecturas completas, accesos parciales y publicaciones que comparten muestra. SECAT y UComGSP mantienen su acceso parcial y no se usan para atribuir criterios no leídos.

Desarrollo: [[Correspondencia de competencias de Assyne con CyberSim]], [[Fundamento de las competencias de seguridad de CyberSim]] y [[Revisión focalizada de competencias de seguridad]].

## Medir una competencia y declarar competente al perfil

Un intento puede respaldar una observación específica bajo sus condiciones. Una conclusión sobre el perfil requiere especificación de responsabilidades, cobertura representativa y variada, evidencia individual suficiente, ayudas conocidas, juicio consistente y una regla de decisión con estándar justificado.

No se obtiene sumando flags, promediando dimensiones arbitrariamente o exigiendo un 80% sin sustento. Tampoco basta la cobertura del diseño: hay que comprobar qué tareas recibió y resolvió cada estudiante. La selección de competencias y los criterios técnicos ya tienen fundamento bibliográfico. Para establecer un corte de aprobación global hay que justificar además el estándar y comprobarlo mediante revisión de entregas y pilotaje, analizando variación por tarea, corrector y condiciones. Un estudio que informa desempeño por capacidades no necesita presentarse como certificación profesional global.

Se implementarán tres resultados: **evidencia insuficiente**, **nivel aún no demostrado** y **nivel demostrado para el perfil y condiciones declarados**. NE, incidencia y ausencia de oportunidad no son un cero automático. Un resultado positivo indica capacidades, alcance, fecha, versiones, ayudas y límites; no afirma competencia en todos los roles de ciberseguridad.

Desarrollo: [[Del desempeño a la competencia del perfil]], [[Plan de cobertura del perfil]], [[Modelo de evidencia y validación]].

## Dictamen sobre AndinaPay

El mecanismo de clave embebida es apropiado para observar diagnóstico, recuperación y verificación. El planteamiento necesita corregir la contradicción entre el aviso con información en claro y el archivo cifrado que se entrega para trabajar. La ausencia de alertas tampoco es prueba de ausencia de intrusión.

La versión revisada entrega un aviso con muestra sintética en claro y una copia cifrada para contrastar. Encontrar una clave histórica y recuperar registros demuestra una posibilidad de exposición, no quién filtró, el vector exacto ni el origen del volcado. Rotar y recifrar restaura protección operacional, pero no vuelve confidencial la copia histórica que un tercero ya posee junto a su clave.

Se admiten rutas equivalentes. La verificación exige registros afectados y controles negativos, operación legítima conservada, nuevas escrituras con custodia correcta y límites expresos. Borrar el literal de HEAD, bloquear toda lectura o rotar sin migrar son falsos arreglos. La rúbrica 0–3 es una propuesta que se calibra, no un umbral profesional ya validado.

El relato listo para utilizar, la rúbrica y los criterios de aceptación están en [[Revisión del escenario AndinaPay]].

## Qué programar primero

1. **Entrega persistente de AndinaPay:** resultado tipado de guardado/entrega, snapshot recuperable e inmutable, operación idempotente y recibo confirmado en UI.
2. **Comprobación docente confiable:** ejecutar sobre la revisión congelada y separar resultados de las pruebas elegidas por el estudiante. Una batería pendiente vacía no acredita corrección.
3. **Procedencia y revisión:** conservar pistas/referencia, intentos, incidencias y adjudicación con evidencias. Reutilizar el informe existente.
4. **Integración y cobertura:** llevar las herramientas de los otros casos al monitor, crear variantes y ampliar mecanismos que faltan.
5. **Pilotaje y decisión del perfil:** revisar anclajes, oportunidades, consistencia y estándar antes de un veredicto con consecuencias.

La secuencia completa, archivos de partida, dependencias y pruebas decisivas están en [[Ruta de programación de CyberSim]].

## Alcance del cierre

Se entregan cuatro respuestas, análisis de alternativas, fichas, matriz de cobertura, revisión del caso y ruta implementable. La ampliación del 15–16-11-2026 completa el fundamento de las competencias y la correspondencia con Assyne: el inventario actual contiene 137 fichas y 17 textos completos con alcance declarado; el nuevo cribado de 50 se solapa con el corpus anterior. La recuperación fue web dirigida y por fuentes originales, sin una exportación exhaustiva de Scopus/WoS ni doble cribado independiente. No equivale a revisar toda publicación existente o reproducir experimentos. Cada texto completo declara figuras, anexos y materiales externos efectivamente examinados; las limitaciones no se ocultan en un conteo global.

La fase posterior es implementar y validar el instrumento para evaluar competencias ya adquiridas. Sus resultados actuales todavía no permiten acreditar competencia profesional; falta comprobar la calidad de las evidencias, la consistencia de la evaluación y el alcance de las conclusiones sobre cada estudiante.
