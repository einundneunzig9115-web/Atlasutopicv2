# Atlas Utòpica v0.43

## Cambios

- Mantiene las firmas de autor específicas y la deduplicación de perfiles provisionales incorporadas en la 0.42.
- Prioriza las recomendaciones con evidencia individual suficiente antes de añadir coincidencias provisionales. Dentro de cada nivel de evidencia, ordena por puntuación y desempata por nombre de forma determinista.
- Aplica el mismo criterio en la recomendación principal por dimensión y calcula la diferencia de afinidad dentro del mismo nivel.
- Utiliza hasta ocho pistas temáticas elegibles como reserva, para completar cinco entradas cuando hay candidatos suficientes, manteniendo sus límites documentales visibles.

## Archivos

- `index.html`: aplicación completa; idéntica byte por byte al HTML individual.
- `README.md`: notas de versión y pruebas.
- `manifest.webmanifest`, `icon-192.png`, `icon-512.png`: recursos del sitio.

## Validación

- Los ocho bloques JavaScript inline superan `node --check`.
- Se ejecutaron ocho perfiles sintéticos de referencia en Chromium para las tres dimensiones (24 rankings). La 0.43 produjo cinco entradas en los 24 casos sin errores JavaScript de ejecución.
- La comparación 0.41 → 0.43 cambió las 24 listas de cinco resultados; la coincidencia media entre listas fue de 3/5 nombres. Esto demuestra que cambió el ranking, no que cada recomendación sea ya correcta.
- Se comprobó el render completo con 5/5/5 resultados, una vista parcial de capítulo con cinco respuestas y el cambio de idioma al castellano.
- Los perfiles sintéticos son pruebas de regresión, no una muestra de usuarios ni una validación psicométrica. Las fichas del catálogo tienen profundidad desigual, y solo una parte de los autores dispone de firmas individuales explícitamente curadas.
- Esta entrega no se ha publicado automáticamente en GitHub Pages. Conserva una copia de seguridad antes de reemplazar archivos remotos.
