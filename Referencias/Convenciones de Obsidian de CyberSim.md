---
type: guide
---
# Convenciones de Obsidian de CyberSim

Se adopta la estructura física de `pii-anonymizer-kb`: Arquitectura, Papers y Referencias; `Estado del arte` orienta la navegación. La guía inicial y el archivo proporcionado `Principios de organización en Obsidian.md` orientan la organización; esta ampliación se trabaja en `C:\Users\stive\Documents\cybersim-kb`, destino indicado por el usuario.

- Las carpetas indican ubicación estable. Los MOCs organizan preguntas, argumentos y rutas de lectura.
- Una publicación tiene una ficha única; puede enlazarse a varias preguntas sin duplicar archivos ni conteos.
- Los nombres son semánticos. Los identificadores P001… se usan como claves de registro, no para ordenar artificialmente los filenames.
- Las fichas de papers usan `type`, `year`, `lectura` y `preguntas`; estas propiedades alimentan consultas reales.
- No se añaden tags que repitan carpetas o estados ya registrados.
- Los enlaces contextuales deben expresar utilidad o dependencia, no llenar el grafo de relaciones arbitrarias.
- El inventario completo vive en CSV y en una Base nativa. Los MOCs mantienen una selección de navegación.
- Los adjuntos originales recuperados se guardan junto a la ficha y se enlazan desde ella. Hay seis PDF conservados. Consultar una fuente web no implica que exista una copia local de su PDF.
- Markdown y enlaces conservan el conocimiento sin plugins. No se reemplaza la configuración `.obsidian` existente del destino.

Los estados de lectura están definidos en [[Protocolo de revisión de CyberSim]]. El año corresponde a la edición citada o primera publicación identificada; diferencias entre online-first y volumen deben anotarse. No deducir el año del DOI ni de la fecha de rastreo del buscador.

## Aplicación en la ampliación de competencias

El fundamento y la correspondencia son notas de decisión dentro del dominio existente Arquitectura; el registro de lecturas permanece en Referencias. Los tres nuevos papers tienen una sola ficha canónica cada uno. Los IDs con huecos son claves de investigación, no una numeración de archivos ni un conteo de publicaciones.

La propiedad `revision_competencias` se utiliza en una vista específica de [[Corpus de CyberSim.base]] para consultar las 50 fichas reexaminadas. La correspondencia A01–A52 vive como contenido de una decisión; no genera 52 notas ni etiquetas. Los MOCs enlazan conceptos y argumentos, y dejan el inventario exhaustivo en la Base, CSV y registro.
