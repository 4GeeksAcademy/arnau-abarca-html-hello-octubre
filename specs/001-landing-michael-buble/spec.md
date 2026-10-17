# Especificación: landing de Michael Bublé

## Objetivo

Definir una landing page en español dedicada a presentar la biografía y trayectoria musical de Michael Bublé, junto con una selección de conciertos. El resultado debe ser elegante, clásico, equilibrado, accesible y adaptable a distintos tamaños de pantalla.

La página es informativa e independiente. No debe dar a entender que está afiliada, aprobada o gestionada por Michael Bublé. El contenido se redactará en tercera persona, aunque el enlace de navegación conserve la etiqueta solicitada «Sobre mí».

## Alcance

- Una sola landing page.
- HTML semántico y CSS en archivos separados.
- Maquetación con Flexbox y diseño responsive.
- Sin JavaScript ejecutable, frameworks, bibliotecas ni dependencias externas de interfaz.
- Datos estructurados Schema.org `Person` en JSON-LD.

## Estructura y contenido

1. **Header:** navegación interna hacia «Sobre mí», «Trayectoria» y «Conciertos».
2. **Hero (`id="hero"`):** bienvenida, presentación clara del artista y enlace para explorar el contenido.
3. **Sobre mí (`id="about"`):** biografía breve y útil, acompañada de una fotografía autorizada.
4. **Trayectoria (`id="experience"`):** discos destacados y premios o reconocimientos pertinentes.
5. **Conciertos (`id="events"`):** tres tarjetas de conciertos pasados; cada una incluye imagen, fecha, lugar y descripción.
6. **Footer:** correo ficticio de contacto, identificado expresamente como demostración y no como contacto oficial.

Los cuatro IDs indicados deben aparecer una sola vez y coincidir exactamente con los enlaces internos correspondientes.

## Requisitos de contenido y fuentes

- Redactar contenido completo, coherente y natural en español; no dejar texto de relleno ni secciones vacías.
- Priorizar fuentes primarias y fiables, como el sitio y los canales oficiales del artista, así como fuentes institucionales o discográficas reconocidas.
- Verificar fechas, álbumes, premios y datos biográficos. Enlazar las fuentes relevantes cerca de las afirmaciones que respaldan.
- Si no se encuentran fuentes fiables para tres conciertos, completar las tarjetas restantes con ejemplos inventados y marcar cada uno de forma visible e inequívoca como **«Ejemplo ficticio»**. No describirlos como actuaciones reales de Michael Bublé.
- No inventar citas, premios ni datos biográficos; las invenciones permitidas se limitan a los ejemplos de conciertos de reserva y al correo ficticio.
- Utilizar `contacto@example.com` o una dirección equivalente de dominio reservado para ejemplos, y presentarla como ficticia.

## Imágenes y permisos

- Utilizar imágenes de Internet únicamente si la licencia o permiso en su fuente original permite claramente el uso previsto.
- Comprobar y registrar procedencia, licencia, atribuciones y requisitos de enlace o modificación antes de incorporar cada imagen.
- No considerar que una imagen es reutilizable solo porque aparezca en buscadores, redes sociales o una página oficial.
- Añadir texto alternativo descriptivo a imágenes informativas; usar `alt=""` en imágenes decorativas. Incluir pies y créditos cuando correspondan.

## Diseño y accesibilidad

- Mantener una dirección visual elegante, clásica y balanceada, con jerarquía tipográfica clara, buen contraste y espacios equilibrados.
- Cada sección principal debe aproximarse a la altura del viewport cuando el contenido lo permita. Usar altura mínima, no fija: las secciones pueden crecer para evitar contenido cortado, especialmente en móvil y en la sección de conciertos.
- La composición debe reorganizarse para pantallas estrechas sin desbordamiento horizontal. La navegación y las tarjetas deben seguir siendo legibles y utilizables.
- Usar landmarks semánticos, jerarquía lógica de encabezados y enlaces descriptivos. Declarar el idioma del documento como español.
- Proporcionar foco de teclado visible, navegación completa por teclado y contraste suficiente. La información no debe depender solo del color o las imágenes.
- No usar autoplay ni ocultar contenido esencial. El orden de lectura debe tener sentido con CSS desactivado.

## SEO, GEO y datos estructurados

- Incluir título único y descriptivo, meta descripción pertinente y encabezados que reflejen el contenido real.
- Organizar nombres, fechas y temas de forma explícita y consistente. Proporcionar contexto y fuentes verificables para facilitar la comprensión por personas, buscadores y sistemas generativos; evitar repetición artificial de palabras clave.
- Incluir JSON-LD válido con `@type: "Person"` y el nombre de Michael Bublé. Añadir solo propiedades cuyos valores sean correctos, estén verificados y sean coherentes con el contenido visible.
- No inventar URL canónica, dominio, perfiles oficiales ni valores de Schema.org. Omitir las propiedades que no puedan verificarse.
- El bloque `application/ld+json` es datos estructurados, no JavaScript ejecutable; no añadir scripts ejecutables.

## Criterios de aceptación

1. La página está en español y contiene un título descriptivo y una meta descripción pertinente.
2. La página contiene `header`, `nav`, `main` y `footer` semánticos, además de las cuatro secciones con IDs exactos `hero`, `about`, `experience` y `events`, cada ID único.
3. Los enlaces del header llevan a las secciones `about`, `experience` y `events`; el enlace de bienvenida lleva a `hero`. Todos los destinos existen y son navegables con teclado.
4. El hero presenta a Michael Bublé y ofrece una bienvenida. La sección biográfica incluye información verificada y una foto con permisos comprobados.
5. La trayectoria contiene discos y reconocimientos pertinentes, con fechas verificadas y enlaces a fuentes fiables.
6. Se muestran exactamente tres tarjetas de conciertos pasados. Cada una contiene imagen, fecha, lugar y descripción. Los conciertos sin fuente fiable se identifican claramente como ejemplos ficticios y no se presentan como hechos reales.
7. Las imágenes cumplen sus permisos de uso, créditos y texto alternativo; los elementos decorativos tienen `alt=""`.
8. El footer muestra un correo de dominio reservado identificado como ficticio, no como contacto oficial.
9. El documento contiene JSON-LD parseable de tipo `Person`; sus datos coinciden con contenido visible y verificado, y no se añaden URLs o perfiles sin confirmar.
10. Las secciones se aproximan a la altura del viewport sin usar una altura fija que recorte contenido. En móvil y escritorio no hay solapamientos ni desplazamiento horizontal.
11. Se puede recorrer el contenido con teclado, el foco es visible, el contraste es suficiente y el contenido sigue teniendo un orden comprensible sin CSS.
12. La implementación usa HTML y CSS separados, Flexbox para la maquetación y no contiene JavaScript ejecutable, frameworks ni dependencias externas de interfaz.

## Fuera de alcance

- Implementación de HTML, CSS o JavaScript.
- Funciones interactivas que requieran JavaScript, reproductores con autoplay o formularios funcionales.
- Afirmaciones de afiliación oficial o contacto directo con el artista.