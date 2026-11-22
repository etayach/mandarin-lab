MANDARIN LAB 2.4.3
Publicación: GitHub Pages

Archivos:
- index.html
- manifest.webmanifest
- sw.js
- icon.svg
- README.txt

Cambios 2.4.3:
- Gestión de sesiones de reconocimiento con liberación idempotente.
- No permite solicitudes simultáneas mientras una sesión está activa o cerrándose.
- Espera el evento end antes de iniciar una sesión posterior.
- Watchdogs para recuperar la interfaz si Safari no emite end después de un error o cancelación.
- El botón de reconocimiento refleja los estados de preparación, escucha y disponibilidad.
- Navegación entre palabras espera el cierre de la sesión anterior.
- Se mantiene el diagnóstico técnico oculto por defecto.

Publicación:
Sube los cinco archivos directamente a la raíz del repositorio GitHub Pages y confirma los cambios.
La versión de Service Worker cambia para solicitar los activos nuevos.
