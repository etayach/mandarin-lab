# Mandarin Lab 2.2

Actualización de Mandarin Lab 2.1. Conserva las mejoras de filtros de Flashcards y añade identificación de versión, historial de cambios, respaldo JSON con metadatos y validación, y ayuda contextual para incidencias de audio en iPhone.

## Publicación en GitHub Pages
Sube `index.html`, `sw.js`, `manifest.webmanifest` e `icon.svg` directamente a la raíz del repositorio existente y confirma los cambios. No subas la carpeta contenedora. El nombre de caché del service worker cambió a `mandarin-lab-v2.2.0` para renovar los recursos de la PWA.

## Respaldo
En Ajustes y datos, usa Exportar respaldo JSON antes de actualizar o trasladar tus datos. La importación valida la estructura y solicita confirmación antes de reemplazar los datos locales. El respaldo no incluye el código ni el vocabulario base integrado, que ya forma parte de la aplicación.

## Audio en iPhone
La aplicación usa SpeechSynthesis del navegador. Safari para iPhone puede silenciar la síntesis de voz por el altavoz cuando el interruptor físico está en modo silencio. La web no puede detectar directamente ese interruptor; si no se escucha, comprueba el modo silencio, el volumen y la salida de audio. No se solicita permiso de micrófono para reproducir voz.

## Datos y privacidad
El progreso se almacena localmente en cada navegador y no se sincroniza automáticamente entre dispositivos. Exporta respaldos periódicamente y conserva el archivo en un lugar seguro.
