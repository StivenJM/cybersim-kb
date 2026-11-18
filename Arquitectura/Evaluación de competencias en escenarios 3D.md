---
type: moc
status: propuesto
---
# Evaluación de competencias en escenarios 3D

**Q1: CyberSim debe evaluar decisiones y productos técnicos situados en el escenario.** La interacción 3D permite representar una oficina, personas con responsabilidades, recursos y consecuencias. La evidencia de competencia proviene de lo que el estudiante investiga, argumenta, modifica y verifica bajo condiciones conocidas.

Pregunta operacional final: **¿Qué evidencias de diagnóstico, decisión, corrección y verificación producidas por estudiantes de ingeniería de software en escenarios virtuales 3D permiten emitir juicios válidos sobre competencias delimitadas de desarrollo seguro?** La población objetivo tiene formación previa en los contenidos evaluados. Esta pregunta guía el diseño y la validación de un instrumento para comprobar qué capacidades puede demostrar cada estudiante.

## Qué se observa

| Dimensión | Actuación que debe provocar la tarea | Evidencia conservada | Insuficiencia que hay que reconocer |
| --- | --- | --- | --- |
| D1 Diagnosticar | Contrastar hipótesis y localizar el mecanismo | Afirmación inicial, artefactos citados y prueba discriminante | Acertar el nombre del CWE o seleccionar la pista obvia |
| D2 Explicar y decidir | Relacionar mecanismo, impacto, alternativas y límites | Explicación situada y decisión con razones | Repetir una definición o un informe genérico |
| D3 Intervenir | Cambiar código, configuración o flujo de recuperación | Revisión entregada y propiedades verificadas | Desactivar el servicio para impedir el ataque o pegar la solución sin entenderla |
| D4 Verificar y delimitar | Elegir contrastes adversarios y legítimos e interpretar resultados | Pruebas elegidas, entradas, salidas, revisión y límites declarados | Que el sistema ejecute una batería oculta y se la atribuya al alumno |

Estas dimensiones organizan observaciones; no se afirma que sean cuatro factores psicométricos independientes. Una misma evidencia puede apoyar dimensiones relacionadas, sin convertirse en varias observaciones independientes.

## Papel concreto del 3D

En AndinaPay, una conversación entrega el aviso; el monitor da acceso al repositorio y al banco criptográfico; otros recursos permiten contrastar custodias o antecedentes. El recorrido tiene sentido si ayuda a decidir quién posee información y qué evidencia falta. Caminar, encontrar un objeto o abrir pantallas no debe otorgar puntos de seguridad por sí mismo.

Cada objeto evaluativo debe llevar a una decisión o artefacto de la tarea. Los documentos esenciales tendrán una vista accesible por teclado y monitor, con la misma información. Antes del intento se permite practicar únicamente los controles y la navegación con contenido ajeno al caso. Esta familiarización no enseña contenidos de seguridad ni revela soluciones. El tiempo de navegación, el mareo, la experiencia con videojuegos o el hardware no deben dominar la interpretación de la competencia en seguridad de aplicaciones.

## Secuencia implementable

1. Presentar situación y condiciones: recursos, tiempo, herramientas, ayudas permitidas y alcance de responsabilidad.
2. Solicitar un diagnóstico con evidencias y conservar su versión inicial. Mantener ocultas las soluciones y aplicar la política de documentación y ayudas permitidas; registrar cualquier exposición que pueda afectar la interpretación del desempeño.
3. Permitir rutas razonables de investigación, correcciones y pruebas, preservando versiones.
4. Confirmar entrega del snapshot exacto y conservar pruebas del alumno separadas de las docentes.
5. Emitir hechos automáticos y una propuesta de revisión; el docente juzga razones, alternativas y límites con anclajes.
6. Entregar un informe del desempeño observado, las evidencias y los límites de la conclusión. Para nuevas evaluaciones, conservar el historial de exposición al caso y utilizar variantes que permitan obtener evidencia adicional.

No exigir una única secuencia historial→clave→descifrado si otra ruta produce evidencia equivalente. Una hipótesis inicial falsa, revisada con rigor, puede ser evidencia de buen diagnóstico. Un acierto final sin rastro suficiente no demuestra por sí solo ese proceso.

## Qué aporta la investigación y qué se descarta

[[NICE-by-design - Diseño trazable de escenarios]] y [[REWIRE - Cursos y certificación por perfil]] ayudan a alinear trabajo y tareas. Los estudios de procesos de respuesta y de rúbricas ofrecen procedimientos de revisión, no una escala universal lista para aplicar. Los trabajos de CTF y VR obligan a distinguir participación, conocimiento declarado y actuación demostrada; véase [[Análisis crítico de los estudios centrales]].

No se adopta puntuación competitiva como medida profesional, ni telemetría exhaustiva, biometría, un tutor LLM o un modelo latente como requisito. La opción inicial más defendible para este código es evidencia explícita más verificadores y revisión docente. Un modelo estadístico podrá añadirse si el diseño y el tamaño efectivo de datos lo sostienen.

## Comprobación que resolverá la incertidumbre local

El piloto comprobará la comprensión de las consignas, la correspondencia entre actuación y evidencia, la dificultad de las tareas, la consistencia entre evaluadores y las barreras de acceso. Participarán estudiantes con la formación previa definida para el perfil. Se revisará si las tareas permiten distinguir niveles de desempeño y si el manejo de la interfaz introduce dificultades ajenas a las competencias de seguridad que se quieren evaluar.

Desarrollo: [[Modelo de evidencia y validación]], [[Revisión del escenario AndinaPay]], [[Ruta de programación de CyberSim]]. Corpus completo de Q1: [[Registro de revisión de CyberSim]] y [[Corpus de CyberSim.base]].
