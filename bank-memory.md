# Memoria del proyecto

## Objetivo y reglas

Landing informativa e independiente sobre Michael Bublé, en español y tercera persona. Debe usar HTML semántico y CSS separado, Flexbox y diseño responsive; sin JavaScript ejecutable, frameworks ni dependencias de interfaz. Seguir [AGENTS.md](AGENTS.md).

## Implementación

- [index.html](index.html): landmarks `header`, `nav`, `main`, `footer`; secciones `hero`, `about`, `experience` y `events`; metadatos SEO, fuentes, créditos, alt y JSON-LD `Person` mínimo.
- [styles.css](styles.css): paleta clásica, tipografía de sistema, Flexbox, breakpoint móvil en `44rem`, foco visible y secciones con `min-height: 100svh` para permitir crecimiento sin recortes.
- [spec.md](specs/001-landing-michael-buble/spec.md), [plan.md](specs/001-landing-michael-buble/plan.md) y [tasks.md](specs/001-landing-michael-buble/tasks.md): requisitos, pasos y seguimiento.
- [research.md](specs/001-landing-michael-buble/research.md): hechos contrastados, conciertos de ejemplo y procedencia/licencias de imágenes.

## Decisiones de contenido y permisos

La biografía oficial sustenta los datos del artista, álbumes y recuentos de premios; no se inventan fechas individuales de premios. Al no verificarse tres conciertos, los tres ejemplos se identifican visiblemente como ficticios. Las imágenes usan licencias abiertas con atribución; no se usa una foto cuya licencia en el origen discrepaba de Commons. El correo `contacto@example.com` se presenta como ficticio y no oficial.

## Ejecución y verificación

Arrancar con `python3 server.py`; abre en `http://localhost:3000`. Flask se instaló en el entorno, no como dependencia del repo. HTML, CSS e imágenes respondieron correctamente; se comprobaron IDs, JSON-LD, contraste y reglas responsive estáticas. La prueba interactiva y la inspección visual móvil/escritorio siguen pendientes: Chromium no arranca por bibliotecas de sistema ausentes y el usuario del contenedor no tiene privilegios para instalarlas.
