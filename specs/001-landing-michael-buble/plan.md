# Plan técnico: landing de Michael Bublé

## Enfoque

Construir una landing informativa de una sola página usando HTML semántico y CSS separado. La plantilla no tiene aún HTML ni CSS; se reutilizará `server.py` para servir la página en el puerto 3000. No se añadirán frameworks, dependencias de interfaz ni JavaScript ejecutable.

## Archivos

- `index.html` — crear en la raíz. Contendrá metadatos, navegación y secciones semánticas `hero`, `about`, `experience` y `events`, además del footer.
- `styles.css` — crear en la raíz y enlazar desde `index.html`. Contendrá diseño Flexbox y reglas responsive.
- `specs/001-landing-michael-buble/spec.md` — consultar como fuente de requisitos y criterios de aceptación; no modificar.
- `AGENTS.md` — seguir las convenciones del proyecto.
- `README.es.md` y `server.py` — consultar para ejecutar la web localmente; no modificar.

## Pasos principales

1. Verificar con fuentes fiables la biografía, discografía, premios y conciertos; incluir enlaces cerca de las afirmaciones correspondientes.
2. Comprobar la licencia o permiso de cada imagen en su fuente original y registrar créditos y procedencia. No usar imágenes sin permiso identificable.
3. Crear `index.html` en español con título y meta descripción, landmarks semánticos, encabezados jerárquicos y navegación interna. Asignar IDs únicos `hero`, `about`, `experience` y `events`.
4. Redactar el contenido en tercera persona y añadir la biografía, la trayectoria, exactamente tres tarjetas de conciertos y un footer. Cada tarjeta incluirá imagen, fecha, lugar y descripción. Si no se hallan fuentes fiables para tres conciertos, marcar los ejemplos restantes visiblemente como «Ejemplo ficticio». Identificar el correo de dominio reservado como ficticio.
5. Incluir JSON-LD válido de Schema.org `Person`, solo con propiedades verificadas que coincidan con el contenido visible. No inventar URLs, perfiles oficiales ni una URL canónica.
6. Crear `styles.css` con una dirección visual elegante, clásica y equilibrada. Usar Flexbox, foco visible, contraste suficiente y alturas mínimas aproximadas al viewport, permitiendo que las secciones crezcan si el contenido lo requiere.
7. Revisar la página en móvil y escritorio con el servidor existente (`python3 server.py`); corregir problemas de navegación, lectura, recortes o desbordamiento antes de finalizar.

## Comprobaciones

- Confirmar carga de `index.html` y `styles.css` en `http://localhost:3000`.
- Revisar landmarks, idioma, jerarquía de encabezados, metadatos, unicidad de IDs y destinos de navegación.
- Confirmar tres tarjetas, fuentes verificables, marcas visibles de contenido ficticio, créditos y textos alternativos apropiados.
- Validar que el JSON-LD sea JSON parseable, de tipo `Person`, y coherente con el contenido visible.
- Probar navegación por teclado, visibilidad del foco, contraste, orden de lectura sin CSS, adaptación móvil y ausencia de desplazamiento horizontal.
- No hay comandos de test o lint configurados; realizar comprobación estática y revisión visual sin añadir herramientas nuevas.
