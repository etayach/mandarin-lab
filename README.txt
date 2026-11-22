# Mandarin Lab 2.4

Actualización de Mandarin Lab 2.2. Conserva los filtros de Flashcards, el almacenamiento local, la importación/exportación de respaldos y el motor de síntesis de voz.

## Novedades de 2.4
- Diagnóstico detallado de SpeechRecognition en Safari.
- Captura de códigos de error reales (`not-allowed`, `audio-capture`, `network`, `no-speech`, `service-not-allowed`, entre otros).
- Gestión de eventos de inicio, captura de audio, voz, resultados, errores y finalización.
- Captura de excepciones al iniciar el reconocimiento.
- Prevención de sesiones simultáneas.
- Panel para copiar el diagnóstico técnico y compartirlo.
- Alternativa de autoevaluación si el navegador no ofrece reconocimiento.

## Publicación en GitHub Pages
Sube `index.html`, `sw.js`, `manifest.webmanifest` e `icon.svg` directamente a la raíz del repositorio existente y confirma los cambios. No subas la carpeta contenedora. El nombre de caché del Service Worker cambió a `mandarin-lab-v2.4.0`.

## Respaldo y datos
Antes de actualizar, exporta un respaldo JSON desde Ajustes y datos. La versión 2.4 conserva el mismo esquema de respaldo de 2.2 y mantiene el progreso en el almacenamiento local del navegador. No hay sincronización automática entre dispositivos.

## Limitación importante
La versión 2.4 mejora el diagnóstico y el manejo de errores, pero no puede corregir por sí sola un fallo del servicio de reconocimiento de voz de Safari/WebKit. Si el servicio del sistema falla, la aplicación mostrará el código de error real para orientar el siguiente paso. El reconocimiento de voz puede requerir conexión a internet según la implementación de Safari.
