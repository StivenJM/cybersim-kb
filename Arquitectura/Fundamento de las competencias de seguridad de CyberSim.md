---
type: decision
status: fundamentado
---
# Fundamento de las competencias de seguridad de CyberSim

**CyberSim evaluará capacidades de desarrollo seguro que el estudiante ya adquirió. La selección tiene una base bibliográfica identificable: un modelo publicado de competencias de aseguramiento de software, el catálogo general de Assyne y estudios que evalúan tareas concretas de estudiantes.** Las ocho etiquetas CAP organizan esa selección; los papers no publicaron conjuntamente una escala de ocho factores con esos nombres.

La ampliación documental del 15–16 de noviembre de 2026 examinó **abstract y cierre de 50 publicaciones distintas**, incluyendo 47 ya registradas y tres incorporaciones. El registro distingue fundamentos directos, apoyo metodológico, contexto y trabajos que no se adoptan. Véase [[Revisión focalizada de competencias de seguridad]].

## Perfil y responsabilidad que se evalúan

El destinatario es un estudiante próximo a terminar ingeniería de software, con formación previa en programación, bases de datos, aplicaciones web, control de versiones y los mecanismos de seguridad del caso. Resuelve un problema delimitado de una aplicación o integración: identifica el riesgo, explica su causa, modifica o propone un control y comprueba que protege sin impedir el uso autorizado. Puede consultar documentación y debe declarar ayudas.

Esta delimitación no exige desempeñarse como jefe de seguridad, investigador de vulnerabilidades inéditas o responsable de toda una organización. La selección cubre trabajo individual observable; colaboración y liderazgo requerirían otras tareas. La seguridad de sistemas con IA se evalúa como **extensión explícita**, con formación previa correspondiente. No se presupone que cualquier estudiante de software domina entrenamiento de modelos.

## Un paper que vincula seguridad de software y nivel de pregrado

[[Mead y Shoemaker - Competencias de aseguramiento de software]] presenta el *Software Assurance Competency Model*. Su sección 2.1 distingue niveles profesionales; la sección 2.4 vincula expresamente resultados de pregrado con L1–L2. Por eso aporta una referencia de población más directa que adoptar íntegramente un perfil de especialista de ciberseguridad.

Aquí, **aseguramiento de software** significa reunir y comprobar evidencia que permita confiar en que el software cumple las propiedades esperadas, incluidas las de seguridad. No basta con que una función produzca el resultado habitual: también debe examinarse qué ocurre ante usos adversarios y fallos relevantes.

Se toman como dominios de referencia evaluación del aseguramiento, seguridad de sistemas, funcionalidad, operación, riesgos y comunicación. **No se declara que aprobar CyberSim certifique L2**, ni se convierten sus niveles en D1–D4.

Hay una precaución concreta: la tabla detallada del informe técnico asociado sitúa algunas contramedidas en L3. Por tanto, no puede afirmarse que toda corrección autónoma de cualquier sistema sea una exigencia literal de L2. CyberSim acota las correcciones a código y configuraciones conocidos, con un mecanismo identificable; los estudios de [[Lam - Diagnóstico y corrección de código inseguro]] y [[Almansoori - Componentes del razonamiento seguro]] aportan ejemplos de evaluación de estas actuaciones en estudiantes. Ampliar a auditoría integral, arquitectura organizativa o mitigaciones nuevas exigiría justificar otro perfil.

El artículo y el informe técnico describen **el mismo modelo**: no son dos validaciones independientes. El respaldo bibliográfico del modelo y su revisión profesional tampoco equivalen a validar un instrumento de puntuación de CyberSim.

## Qué aporta cada fuente seleccionada

| Fuente | Aporte utilizado | Alcance que se respeta |
| --- | --- | --- |
| Mead y Shoemaker, 2013, §§2.1–2.4; informe SEI, tabla 3 | Competencias de aseguramiento de software y referencia de nivel de entrada | Modelo de referencia; no prueba local ni equivalencia automática de cada CAP con L2 |
| Assyne, Ghanbari y Pulkkinen, 2022, tabla 12a y discusión | Lectura y escritura de código, pruebas, análisis, comunicación, atención al usuario y calidad | Catálogo general; no se eliminan competencias por su antigüedad ni se copian rasgos personales como notas |
| Lam y colaboradores, 2022, método y figura 1; Almansoori y colaboradores, 2023, §§3–5 y suplemento | Identificar código inseguro, explicar el mecanismo, corregir y usar documentación críticamente | Muestra pequeña y tareas en C; ambos artículos utilizan las mismas 21 entrevistas |
| Joshi y colaboradores, 2024, método y apéndice A | Evaluación de activos, actores, flujos, límites de confianza, amenazas y mitigaciones en ingeniería de software | Rúbricas aplicadas a proyectos de equipos; requieren adaptación para atribución individual |
| Ghosh y Francia, 2021, §§4–9 | Vincular escenario, tareas, preguntas, productos y rúbrica | Su estudio no acredita por sí solo validez de la evaluación ni superioridad del 3D |
| Estudios de secretos, revisión de código e integraciones | Contenidos y fallos concretos que debe representar una tarea de seguridad | Evidencia técnica o profesional; no una escala validada de estudiantes |
| SecureAI y trabajos técnicos de ataques a IA | Diferenciar seguridad de IA, uso de IA para seguridad y etapas del sistema | Extensión del alcance del proyecto; no requisito universal de todo egresado |

## De las fuentes a las ocho capacidades

En esta tabla, **adaptación** significa que el contenido tiene antecedente publicado, pero la redacción y delimitación son de CyberSim. **Especialización** añade un mecanismo técnico a una capacidad general. Ninguna fila atribuye al paper los identificadores CAP.

| Capacidad que se evaluará | Sustento concreto | Decisión y evidencia exigida |
| --- | --- | --- |
| **CAP-01 Analizar contexto y confianza** | P023: modelado del sistema y rúbricas de amenazas; P139: riesgo y seguridad del sistema; P001: arquitectura y visión de conjunto | Adaptación: representar activos, actores, flujos y permisos del caso y explicar dónde puede cruzarse una frontera sin autorización |
| **CAP-02 Diagnosticar causalmente** | P135/P022: reconocer código inseguro y explicar su efecto; P001: análisis y solución metódica de problemas | Adaptación: ubicar evidencia, formular una explicación y contrastarla con una prueba que permita descartar otra hipótesis plausible |
| **CAP-03 Corregir o diseñar un control** | P135/P022: modificar código inseguro; P023: proponer mitigaciones; P001: construcción y reutilización de código | Adaptación acotada: entregar código, configuración o diseño que actúe sobre la causa y conserve el uso autorizado. Proponer un control no acredita haberlo implementado |
| **CAP-04 Verificar e interpretar** | P001: escribir/automatizar pruebas; P135: entradas que evidencian fallos; P139: evaluación y funcionalidad; P038: límites de detectores | Adaptación: elegir contrastes de seguridad y de uso legítimo, interpretar resultados y reconocer lo que las pruebas no cubren |
| **CAP-05 Proteger secretos y datos** | P036/P037: prácticas y dificultades del ciclo de vida de secretos; P038/P039: detección; antecedentes de pruebas y análisis de P001 | Especialización: localizar exposición, limitar acceso, cambiar credenciales y gestionar datos afectados según el caso. Quitar una clave del archivo no elimina copias históricas |
| **CAP-06 Comprobar integridad y procedencia** | P139/informe SEI: aseguramiento de componentes adquiridos; P137: revisión de dependencias e interacciones; estudios técnicos de Q2 | Especialización: verificar origen, integridad y autorización antes de que un dato o artefacto produzca efectos. Una firma válida no convierte por sí sola un contenido en seguro |
| **CAP-07 Evaluar seguridad de una integración con IA** | P079: dominios de seguridad de IA; P042/P044: tareas y mecanismos diferenciados de agentes y contaminación | Extensión condicionada al perfil: distinguir entrenamiento, inferencia, datos e instrucciones y permisos de herramientas. Se requiere una tarea para cada mecanismo que se quiera acreditar |
| **CAP-08 Comunicar y justificar una respuesta responsable** | P001: comunicación, reflexión y necesidades del usuario; P139: riesgo y comunicación; P023: justificación de decisiones | Adaptación: informar hechos, impacto, prioridad, alternativas y riesgo residual con evidencia. Se evalúa la decisión observable, sin diagnosticar personalidad |

P005, P061 y P108 respaldan precauciones sobre puntuación, procesos de respuesta y verificación de artefactos; **no se usan para inventar el contenido de las ocho competencias**. NICE y ECSF ayudan a describir responsabilidades, pero el fundamento no depende exclusivamente de esos catálogos institucionales.

## Qué ocurrió con la lista de Assyne

Se conservan y especializan lectura y construcción de código, pruebas, arquitectura, análisis, resolución de problemas, comunicación, necesidades del usuario y calidad del producto. La correspondencia completa está en [[Correspondencia de competencias de Assyne con CyberSim]], con una decisión para cada expresión de la tabla 12a.

Las competencias de dirección y trabajo en equipo quedan fuera de **esta prueba individual** porque sus tareas no permiten observarlas suficientemente. Experiencia previa y formación son condiciones de entrada. Motivación, autoestima, diversión o orgullo no se califican desde acciones aisladas. Atención al detalle y calidad se traducen en comprobaciones del producto, sin inferir un rasgo estable. La frase sobre sacrificar diseño bajo presión no se adopta como conducta que merezca recompensa.

La ausencia de competencias de mantenimiento/configuración en la tabla 12b del mapeo no prueba que sean irrelevantes: los propios autores señalan esa laguna. Esto justifica complementar el catálogo, no eliminar seguridad de operación o dependencias.

## Alternativas examinadas y razón de la selección

| Alternativa | Decisión razonada |
| --- | --- |
| Copiar todo Assyne | Conserva un antecedente, pero mezcla responsabilidades, condiciones de experiencia y atributos personales; no representa por sí solo tareas actuales de seguridad |
| Adoptar solo SECAT o UComGSP | Son pertinentes para evaluación/contextualización de software. El acceso recuperado fue parcial; no se les atribuye una lista operativa ni una validación no examinada |
| Adoptar íntegramente NICE/ECSF o un perfil SOC | Confunde el alcance del estudiante de desarrollo con responsabilidades de otros puestos; se toman solo tareas pertinentes |
| Usar una síntesis reciente de DevSecOps o buenas prácticas como única escala | Aporta contenidos, pero una síntesis conceptual no demuestra que sus categorías sean factores medibles de estudiantes |
| Usar un inventario genérico de competencias digitales o de personalidad | Mide otro dominio o constructo; no sustituye una actuación de desarrollo seguro |
| Modelo de aseguramiento + catálogo de software + tareas evaluadas + mecanismos técnicos | Selección adoptada: cada componente resuelve una necesidad distinta y deja visible qué es adaptación local |

No se concluye que estas sean las únicas competencias posibles o que la búsqueda encontró el mejor instrumento universal. Sí se dispone de una selección justificable para el perfil y las familias de ataques declarados, sin posponer su fundamento a un futuro panel.

## Qué queda resuelto y qué debe comprobarse

**Queda resuelto documentalmente qué evaluar y por qué.** Las tareas se construyen con criterios técnicos verificables: impedir el efecto no autorizado, conservar el autorizado, actuar sobre el mecanismo y justificar el alcance. El [[Plan de cobertura del perfil]] especifica productos y contraejemplos; una guía de corrección debe mostrar ejemplos de esos productos.

Una comisión de especialistas no es condición para que exista esta selección fundamentada. La revisión del contenido puede contrastarse con docentes de las asignaturas, fuentes publicadas y corrección de tareas de muestra. Los verificadores y ejemplos reducen la dependencia de interpretaciones tácitas. Las respuestas no previstas o ambiguas sí requieren revisión humana competente en el mecanismo.

**Sigue pendiente comprobar el instrumento y el uso del resultado:** si los estudiantes interpretan las consignas, si distintos correctores coinciden, si las tareas representan la capacidad y si una conclusión se sostiene en otros casos. No se promete automatizar íntegramente ese juicio. Si se quiere una aprobación global con consecuencias, habrá que justificar el estándar y su precisión; citar un paper no proporciona ese corte. Para un estudio de evaluación por capacidades puede informarse el desempeño observado y sus límites sin certificar todo un perfil profesional.

La justificación bibliográfica está completada; el pilotaje no se presenta como una ganancia de aprendizaje causada por CyberSim. Véanse [[Modelo de evidencia y validación]] y [[Del desempeño a la competencia del perfil]].

## Aplicación documentada

[[Guía para evaluar las competencias de seguridad]] transforma el fundamento en productos, criterios y ejemplos de corrección. La lectura completa adicional de P135 permite precisar las condiciones de consulta y ayuda. El catálogo conserva sus fuentes; la guía es una adaptación explícita que deberá contrastarse con entregas de muestra y el piloto.
