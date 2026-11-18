---
type: decision
status: fundamentado
---
# Correspondencia de competencias de Assyne con CyberSim

**La lista de Assyne sí se utiliza.** Esta nota permite comprobar qué elementos se conservan, cómo se especializan en seguridad y por qué otros quedan fuera de la evaluación individual de CyberSim. Las decisiones corresponden al alcance del instrumento, no a una clasificación de competencias importantes y prescindibles para toda la profesión.

Fuente: [[Assyne - Estado de competencias de software]], **tabla 12a, página 10**, contrastada con tabla 12b y discusión de la página 12 del PDF proporcionado. El fundamento de los complementos está en [[Fundamento de las competencias de seguridad de CyberSim]].

## Cómo leer la correspondencia

El artículo declara **49 competencias esenciales agrupadas en 11 temas**. La tabla 12a no asigna 49 identificadores individuales: agrupa expresiones dentro de cada tema. Al separar las expresiones tal como están impresas se obtienen aquí **52 unidades de correspondencia: 19 técnicas, 11 interpersonales y 22 personales**. Ese es un recuento local de expresiones, no una corrección del total de competencias que declaran los autores. Hay formulaciones próximas, como dos expresiones de pensamiento analítico; no se inventan equivalencias ni se borran tres entradas para forzar el número 49.

Las claves A01–A52 solo permiten comprobar cobertura de esta correspondencia; **no son IDs del paper**. Todas las expresiones de sus 11 filas quedan representadas. Se conserva el tema original incluso cuando una expresión pueda parecer más apropiada en otro grupo.

| Decisión | Significado en CyberSim |
| --- | --- |
| Conservar | Evaluar la actuación general que ya describe el catálogo |
| Adaptar | Observar esa actuación en un problema de seguridad, con producto y criterio explícitos |
| Condición previa | Formación o experiencia que caracteriza a la población; no es resultado a enseñar o puntuar durante el intento |
| Fuera de alcance | Requiere responsabilidades, interacción o evidencia que esta prueba no ofrece |
| No puntuar como rasgo | Puede ser importante profesionalmente, pero una entrega aislada no permite inferir ese atributo estable |
| Sin definición suficiente | El término del catálogo no permite construir por sí solo un criterio inequívoco |

## Programación y código

| Clave | Expresión de la tabla 12a | Decisión y correspondencia |
| --- | --- | --- |
| A01 | Writes/automates tests with code | **Conservar → CAP-04.** El estudiante entrega pruebas, explica qué propiedad examinan e interpreta sus resultados; la prueba automática docente se registra aparte |
| A02 | Leverages/reuses code | **Adaptar → CAP-03/06.** Justifica una biblioteca o mecanismo existente, comprueba su uso y evita reutilizar una solución insegura fuera de contexto |
| A03 | Uses code reading | **Conservar → CAP-02.** Ubica el fragmento relevante y explica la relación entre entrada, operación y efecto |
| A04 | Uses structured techniques for communication | **Adaptar → CAP-08.** Informe con hallazgo, evidencia, decisión y límites, con independencia de la herramienta utilizada |

## Análisis de problemas

| Clave | Expresión de la tabla 12a | Decisión y correspondencia |
| --- | --- | --- |
| A05 | Skills/techniques for architecture design | **Adaptar → CAP-01/03.** Representa componentes y propone un control en la frontera adecuada; no diseña toda una arquitectura empresarial |
| A06 | Use of prototypes to assess design | **Adaptar → CAP-03/04.** Un prototipo o cambio ejecutable puede contrastar un control; construir un prototipo no es obligatorio si otro artefacto permite comprobarlo |
| A07 | Possesses unique domain knowledge | **Condición previa.** Se proporciona el contexto del negocio necesario; no se premia conocer de antemano una empresa o sector particular |
| A08 | Obtains necessary training/learning | **Condición previa.** El estudiante llega con formación pertinente; adquirirla mediante CyberSim no es objetivo ni criterio de aprobación |
| A09 | Experience with a similar project | **Condición previa.** Se registra exposición previa cuando afecte la interpretación; no se confunde experiencia declarada con capacidad demostrada |
| A10 | Technical know-how | **Adaptar → CAP-02/03/04.** Se evidencia en explicación, intervención y verificación, en lugar de una autoevaluación genérica |
| A11 | Uses methodical problem solving | **Adaptar → CAP-02.** Explicita hipótesis, selecciona un contraste y revisa su explicación según el resultado |
| A12 | Use of new methods and tools | **Adaptar → CAP-03/04.** Se juzga pertinencia y resultado; la novedad de una herramienta no merece puntos por sí sola |
| A13 | Thinking—strong analytic skills | **Adaptar → CAP-02.** Relaciona evidencia y causa, distingue alternativas y reconoce incertidumbre |
| A14 | Using techniques and tools | **Adaptar → CAP-03/04.** Usa herramientas autorizadas con resultados reproducibles y explica su alcance |
| A15 | Methodological competence | **Adaptar → CAP-02/04.** Procedimiento coherente con el mecanismo; no se exige seguir una secuencia única si otra produce evidencia suficiente |
| A16 | Analytical thinking | **Adaptar → CAP-02.** Mismo constructo operativo que A13; se conserva la expresión original sin contar dos observaciones independientes |

## Gestión de proyectos

| Clave | Expresión de la tabla 12a | Decisión y correspondencia |
| --- | --- | --- |
| A17 | Schedules and estimates well | **Fuera de alcance.** Un caso breve no permite evaluar estimación y seguimiento de un proyecto; una futura tarea de planificación necesitaría evidencia propia |
| A18 | Responds to schedule pressure by sacrificing parts of the design process | **No adoptar como criterio positivo.** Es una conducta reportada por el mapeo, no una recomendación de omitir controles. CAP-08 pide justificar prioridades y riesgos sin recompensar una exposición crítica |
| A19 | Organizational skills | **Fuera de alcance como competencia general.** Una entrega identificable es requisito de evidencia; no demuestra gestión organizativa de proyectos |

## Trabajo en equipo

| Clave | Expresión de la tabla 12a | Decisión y correspondencia |
| --- | --- | --- |
| A20 | Team oriented | **Fuera de alcance.** No hay observación de colaboración sostenida en esta evaluación individual |
| A21 | Interpersonal relationship | **Fuera de alcance.** Hablar con un personaje simulado no equivale a demostrar relaciones profesionales con personas reales |

## Liderazgo

| Clave | Expresión de la tabla 12a | Decisión y correspondencia |
| --- | --- | --- |
| A22 | Proactive role with management | **Fuera de alcance.** Exige relación y responsabilidad de gestión que no se atribuyen al estudiante |
| A23 | Helps others | **Fuera de alcance.** El desempeño individual no permite observar el efecto de su ayuda a compañeros |
| A24 | Information sharing | **Adaptar parcialmente → CAP-08.** Comunica evidencia a quien debe decidir; un informe no acredita liderazgo o colaboración completa |
| A25 | Willingness to confront others | **No puntuar como rasgo.** CAP-08 permite expresar desacuerdo técnico justificado; no se deduce disposición interpersonal estable |
| A26 | Scalability | **Sin definición suficiente.** La palabra aparece en liderazgo sin una definición operativa individual; no se transforma arbitrariamente en escalabilidad técnica de sistemas |

## Comunicación

| Clave | Expresión de la tabla 12a | Decisión y correspondencia |
| --- | --- | --- |
| A27 | Good written communication | **Conservar → CAP-08.** Informe comprensible y verificable, con hechos, evidencia y límites |
| A28 | Good verbal communication | **Conservar si se administra → CAP-08.** Explicación oral breve con los mismos criterios; sin esa oportunidad no se declara evaluada |
| A29 | Reflection | **Adaptar → CAP-02/08.** Explica por qué eligió el control y qué cambiaría si apareciera evidencia contraria; no se exige una confesión personal |

## Orientación al usuario o cliente

| Clave | Expresión de la tabla 12a | Decisión y correspondencia |
| --- | --- | --- |
| A30 | Focus on users or customer needs | **Adaptar → CAP-01/03/08.** Identifica quién necesita la función y conserva ese uso al corregir. Bloquear todo acceso no es una solución suficiente |

## Creatividad

| Clave | Expresión de la tabla 12a | Decisión y correspondencia |
| --- | --- | --- |
| A31 | Creative thinking skills | **Fuera de alcance como rasgo.** CAP-03 admite alternativas correctas sin exigir una solución novedosa |
| A32 | Being innovative | **No puntuar como rasgo.** Aplicar correctamente un control conocido es válido para este perfil; no se exige innovar |
| A33 | Attention to detail | **Adaptar a evidencia del producto → CAP-04.** Comprueba un caso límite relevante; no se diagnostica atención general de la persona |
| A34 | Desire to improve things | **No puntuar como rasgo.** Puede observarse una mejora entregada en CAP-03, no el deseo o motivación que la originó |
| A35 | Design style | **Sin criterio de preferencia personal.** CAP-03 valora seguridad, claridad y función del diseño; no un estilo estético del corrector |

## Autoestima y atributos personales

Se respeta el nombre del grupo del artículo; esta evaluación no diagnostica autoestima.

| Clave | Expresión de la tabla 12a | Decisión y correspondencia |
| --- | --- | --- |
| A36 | Perseverance | **No puntuar como rasgo.** Número de intentos o tiempo invertido no demuestran por sí solos perseverancia ni competencia |
| A37 | The strength of convictions | **No puntuar como rasgo.** Una decisión firme no compensa falta de evidencia; CAP-02 permite rectificar |
| A38 | Proactive/initiator/driver | **No puntuar como rasgo.** Se observa la intervención solicitada, sin inferir iniciativa profesional general |
| A39 | Lack of ego | **No puntuar como rasgo.** Una sesión no permite atribuir humildad o ausencia de ego |
| A40 | Driven by a desire to contribute | **No puntuar como rasgo.** La motivación no se deduce de un artefacto correcto |
| A41 | Desire to do/bias for action | **No puntuar como rasgo.** Actuar rápido puede empeorar el incidente; importa la intervención justificada |
| A42 | Sense of fun | **Fuera de alcance.** Disfrutar el entorno 3D no acredita seguridad de software |
| A43 | Driven by a sense of mission | **No puntuar como rasgo.** No hay evidencia longitudinal sobre la motivación personal |
| A44 | Mixes personal and work goals | **Fuera de alcance.** Los objetivos personales no forman parte de esta evaluación técnica |
| A45 | Thoroughness | **Adaptar a evidencia del producto → CAP-04/08.** Explicita comprobaciones y límites relevantes, sin atribuir minuciosidad estable |
| A46 | Seeks help | **Adaptar como condición registrada.** Documentación, asistencia y pistas se distinguen; pedir ayuda no equivale automáticamente a aprobar o fallar |

## Visión de conjunto y abstracción

| Clave | Expresión de la tabla 12a | Decisión y correspondencia |
| --- | --- | --- |
| A47 | Maintaining a “big picture” view | **Adaptar → CAP-01/08.** Explica consecuencias del cambio sobre datos, usuarios y componentes pertinentes |
| A48 | Breadth of view and influence | **Adaptar parcialmente → CAP-01.** Considera relaciones del sistema; la influencia organizativa queda fuera de alcance |
| A49 | Emphasizes elegant and simple solutions | **Adaptar → CAP-03.** Prefiere una solución comprensible y suficiente cuando cumple los requisitos; la simplicidad no justifica omitir controles |

## Control de calidad

| Clave | Expresión de la tabla 12a | Decisión y correspondencia |
| --- | --- | --- |
| A50 | Quality | **Adaptar → CAP-03/04.** La entrega satisface propiedades explícitas de seguridad y funcionamiento |
| A51 | Pride in quality | **No puntuar como rasgo.** Calidad del producto y orgullo personal son inferencias diferentes |
| A52 | Productivity | **Fuera de alcance como nota de velocidad.** Tiempo y cantidad de cambios pueden registrarse, pero no compensan una corrección insegura |

## Por qué hay complementos que no aparecen literalmente

CAP-05 y CAP-06 especializan análisis, corrección y verificación en mecanismos de secretos, datos, dependencias e integridad. CAP-07 aplica esas capacidades a sistemas con IA cuando forman parte del perfil declarado. La fuente de esos contenidos es la literatura específica que se detalla en [[Fundamento de las competencias de seguridad de CyberSim]] y [[Competencias frente a las familias de ataques]], no una atribución retrospectiva al catálogo de Assyne.

No se crean 52 competencias nuevas ni se suman estas filas como puntos. Son decisiones de correspondencia, y varias alimentan una misma actuación. La definición del nivel y el muestreo se consultan en [[Plan de cobertura del perfil]].
