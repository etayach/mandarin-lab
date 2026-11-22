# Mandarin Lab 2.4.1

Actualización correctiva de Mandarin Lab 2.4 centrada en el ciclo de vida de SpeechRecognition en Safari iOS.

## Cambios de 2.4.1
- Cierre de reconocimiento mediante abort() y espera del evento end antes de liberar la sesión.
- No se desconectan los manejadores de eventos antes de que Safari complete el cierre.
- Bloqueo de pulsaciones repetidas mientras existe una sesión activa o una solicitud de inicio/cierre.
- No se inicia una nueva sesión hasta que la anterior haya terminado o venza un tiempo de seguridad.
- Cierre preventivo al salir de Pronunciación, ocultar la página, abandonar Safari o congelar la página.
- Diagnóstico técnico sigue oculto por defecto y puede habilitarse desde Ajustes y datos.

## Publicación en GitHub Pages
Sube los cinco archivos directamente a la raíz del repositorio existente y confirma los cambios. No subas la carpeta contenedora. El Service Worker utiliza la caché `mandarin-lab-v2.4.1`.

## Datos y limitaciones
Se conserva el esquema de respaldo y el almacenamiento local del progreso. La corrección gestiona de forma más segura las sesiones desde la aplicación, pero el comportamiento final de liberación del micrófono debe validarse en Safari del iPhone; una página web no puede garantizar el comportamiento interno de iOS.
