# Tareas: landing de Michael Bublé

## 1. Preparar contenido y recursos

- [x] Consultar fuentes fiables y registrar datos biográficos verificables en `research.md`.
- [x] Verificar álbumes destacados, premios y fechas; guardar los enlaces de las fuentes en `research.md`.
- [x] Buscar tres conciertos pasados con fuentes fiables; al no encontrar registros suficientes, definir tres ejemplos ficticios y rotularlos como tales en `research.md`.
- [x] Comprobar la licencia o permiso de la fotografía biográfica y de cada imagen de concierto.
- [x] Registrar procedencia, condiciones de uso y atribuciones requeridas para cada imagen en `research.md`.

## 2. Crear la estructura HTML

- [x] Crear `index.html` en la raíz con `lang="es"`, título descriptivo y meta descripción.
- [x] Añadir `header`, navegación, `main` y `footer` usando elementos semánticos.
- [x] Crear las secciones con los IDs únicos `hero`, `about`, `experience` y `events`.
- [x] Enlazar la navegación a `about`, `experience` y `events`; enlazar la marca de cabecera a `hero`.
- [x] Redactar la bienvenida y la biografía en tercera persona con datos verificados y fuentes próximas.
- [x] Añadir la fotografía biográfica con texto alternativo y crédito cuando corresponda.
- [x] Añadir discos y premios pertinentes con fechas verificadas y enlaces a fuentes fiables.
- [x] Crear exactamente tres tarjetas de conciertos, cada una con imagen, fecha, lugar y descripción.
- [x] Marcar de forma visible cada concierto inventado como «Ejemplo ficticio».
- [x] Añadir al footer un correo de dominio reservado, identificado como ficticio y no oficial.
- [x] Incluir JSON-LD válido de tipo `Person` con solo propiedades verificadas y coherentes con el contenido visible.
- [x] Enlazar una hoja de estilos externa `styles.css`; no añadir JavaScript ejecutable ni frameworks.

## 3. Crear estilos adaptables y accesibles

- [x] Crear `styles.css` con una dirección visual elegante, clásica y equilibrada.
- [x] Maquetar las secciones y tarjetas con Flexbox.
- [x] Adaptar la navegación y el contenido a pantallas estrechas sin desbordamiento horizontal.
- [x] Dar a las secciones una altura mínima aproximada al viewport, permitiendo que crezcan si el contenido lo necesita.
- [x] Definir foco de teclado visible, contraste suficiente y estilos legibles.

## 4. Revisar y validar

- [x] Comprobar que todos los IDs son únicos y que cada enlace interno tiene un destino existente.
- [x] Confirmar el orden semántico, la jerarquía de encabezados y la comprensión del contenido sin CSS.
- [x] Revisar que haya exactamente tres tarjetas y que las ficticias estén claramente identificadas.
- [x] Revisar textos alternativos, permisos de uso, procedencia y créditos de todas las imágenes.
- [x] Validar que el JSON-LD se puede analizar como JSON y coincide con el contenido visible.
- [ ] Probar la navegación con teclado y comprobar el foco y el contraste.
- [x] Ejecutar `python3 server.py` y revisar la página en `http://localhost:3000`.
- [ ] Revisar en escritorio y móvil que no haya solapamientos, contenido cortado ni desplazamiento horizontal.

> Pendiente de prueba interactiva de teclado e inspección visual móvil/escritorio: el servidor responde y los recursos cargan, pero Chromium no arranca porque faltan bibliotecas de sistema y este contenedor no tiene permisos para instalarlas. Las reglas responsive se comprobaron estáticamente; eso no confirma visualmente la ausencia de solapamientos.
