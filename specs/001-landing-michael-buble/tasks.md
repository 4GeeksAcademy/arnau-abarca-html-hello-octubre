# Tareas: landing de Michael Bublé

## 1. Preparar contenido y recursos

- [ ] Consultar fuentes fiables y registrar datos biográficos verificables.
- [ ] Verificar álbumes destacados, premios y fechas; guardar los enlaces de las fuentes.
- [ ] Buscar tres conciertos pasados con fuentes fiables; identificar como «Ejemplo ficticio» cada tarjeta que deba completarse con datos inventados.
- [ ] Comprobar la licencia o permiso de la fotografía biográfica y de cada imagen de concierto.
- [ ] Registrar procedencia, condiciones de uso y atribuciones requeridas para cada imagen.

## 2. Crear la estructura HTML

- [ ] Crear `index.html` en la raíz con `lang="es"`, título descriptivo y meta descripción.
- [ ] Añadir `header`, navegación, `main` y `footer` usando elementos semánticos.
- [ ] Crear las secciones con los IDs únicos `hero`, `about`, `experience` y `events`.
- [ ] Enlazar la navegación a `about`, `experience` y `events`; enlazar la llamada del hero a `hero`.
- [ ] Redactar la bienvenida y la biografía en tercera persona con datos verificados y fuentes próximas.
- [ ] Añadir la fotografía biográfica con texto alternativo y crédito cuando corresponda.
- [ ] Añadir discos y premios pertinentes con fechas verificadas y enlaces a fuentes fiables.
- [ ] Crear exactamente tres tarjetas de conciertos, cada una con imagen, fecha, lugar y descripción.
- [ ] Marcar de forma visible cada concierto inventado como «Ejemplo ficticio».
- [ ] Añadir al footer un correo de dominio reservado, identificado como ficticio y no oficial.
- [ ] Incluir JSON-LD válido de tipo `Person` con solo propiedades verificadas y coherentes con el contenido visible.
- [ ] Enlazar una hoja de estilos externa `styles.css`; no añadir JavaScript ejecutable ni frameworks.

## 3. Crear estilos adaptables y accesibles

- [ ] Crear `styles.css` con una dirección visual elegante, clásica y equilibrada.
- [ ] Maquetar las secciones y tarjetas con Flexbox.
- [ ] Adaptar la navegación y el contenido a pantallas estrechas sin desbordamiento horizontal.
- [ ] Dar a las secciones una altura mínima aproximada al viewport, permitiendo que crezcan si el contenido lo necesita.
- [ ] Definir foco de teclado visible, contraste suficiente y estilos legibles.

## 4. Revisar y validar

- [ ] Comprobar que todos los IDs son únicos y que cada enlace interno tiene un destino existente.
- [ ] Confirmar el orden semántico, la jerarquía de encabezados y la comprensión del contenido sin CSS.
- [ ] Revisar que haya exactamente tres tarjetas y que las ficticias estén claramente identificadas.
- [ ] Revisar textos alternativos, permisos de uso, procedencia y créditos de todas las imágenes.
- [ ] Validar que el JSON-LD se puede analizar como JSON y coincide con el contenido visible.
- [ ] Probar la navegación con teclado y comprobar el foco y el contraste.
- [ ] Ejecutar `python3 server.py` y revisar la página en `http://localhost:3000`.
- [ ] Revisar en escritorio y móvil que no haya solapamientos, contenido cortado ni desplazamiento horizontal.
