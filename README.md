# Atlas Utòpica v0.40 · copia de trabajo

Esta entrega contiene la versión de trabajo 0.40. El archivo `index.html` de este paquete es **idéntico byte por byte** al archivo independiente `Atlas_Utopic_v040.html` entregado junto al ZIP.

## Contenido
- `index.html`: entrada principal para GitHub Pages.
- `README.md`: estas instrucciones y notas de validación.
- `manifest.webmanifest`: metadatos de instalación web.
- `icon-192.png` y `icon-512.png`: iconos referenciados por el manifiesto.

## Cambios principales incluidos en 0.40
- Ajustes a la selección y presentación de recomendaciones para mostrar cinco autores por dimensión cuando el estado del test permite emitir resultados.
- Unificación del orden de los perfiles con puntuación entre dimensiones.
- Actualización de identificadores de versión del motor y de los datos exportados.

## Estado de validación
- Los seis bloques JavaScript incrustados pasan una comprobación sintáctica con `node --check`.
- **La validación funcional completa en navegador sigue pendiente.** La prueba automatizada en Chromium no pudo finalizar correctamente en el entorno de auditoría.
- Por tanto, esta es una copia de trabajo para revisión, no una garantía de que todos los flujos de la aplicación estén validados ni de que esté desplegada en GitHub Pages.
- El paquete no confirma ni modifica el contenido actual del repositorio remoto.

## Publicación en GitHub Pages
Para probar esta copia en un repositorio, conserva los nombres y sube los cinco archivos a la raíz. Hazlo solo después de guardar una copia de seguridad de la versión publicada. No se ha realizado ningún despliegue remoto.

## Nota sobre los iconos
Los iconos incluidos se recrearon para mantener funcional el manifiesto; no se ha podido confirmar que sean idénticos a los iconos originales del repositorio de GitHub.
