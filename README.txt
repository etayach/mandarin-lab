# Mandarin Lab 2.0

## Incluye
- Aplicación web responsive (escritorio y móvil).
- 28 entradas transcritas de las fotografías compartidas: lecciones 9 y 10 de *El Nuevo Libro de Chino Práctico 1, 3.ª edición*.
- 20 entradas de muestra HSK 3.0, identificadas expresamente como muestra y no como lista completa.
- Flashcards con repetición espaciada tipo SM-2.
- Dictado, síntesis de voz, práctica oral con reconocimiento del navegador cuando esté disponible, escritura por teclado y examen.
- Biblioteca con filtro por fuente/lección e importación CSV.
- Estadísticas y respaldo/restauración JSON.

## Abrir en Mac
1. Descomprime el ZIP.
2. Abre `index.html` con Safari o Chrome.

## Importante sobre PWA
La aplicación funciona como página local. La instalación PWA, el service worker y la sincronización entre dispositivos requieren alojamiento HTTPS. No se puede instalar una PWA completa abriendo `file://`.

## CSV para importar vocabulario
Encabezados mínimos: `hanzi,pinyin,meaning`
Opcionales: `level,lesson,pos`

Ejemplo:
`汉字,hànzì,carácter chino,3,Lección 1,sustantivo`

Usa UTF-8. Las palabras importadas quedan etiquetadas como vocabulario personal.

## Fuentes y precisión
- Las 28 entradas del libro se transcribieron de las dos fotografías proporcionadas en la conversación. La aplicación conserva las lecciones 9 y 10 visibles en esas imágenes.
- La muestra HSK 3.0 se basa en las primeras entradas visibles del listado de nivel 3 de MandarinBean. No debe confundirse con el listado oficial completo.
- El estándar HSK 3.0 tiene un programa nuevo. La fuente oficial de referencia es Chinese Test Service: https://www.chinesetest.cn/HSK
- Para completar la biblioteca con exactitud, importar el listado oficial del syllabus HSK 3.0 y verificar cada campo de pinyin y significado.

## Instalación PWA (cuando se publique en HTTPS)
El paquete ya incluye `manifest.webmanifest`, `sw.js` e `icon.svg`.
1. Publica los cuatro archivos juntos en un hosting HTTPS (por ejemplo, GitHub Pages, Netlify o Vercel).
2. Abre la URL HTTPS desde Safari en iPhone.
3. Usa Compartir → Añadir a pantalla de inicio.
4. En Mac, usa el menú Archivo → Añadir al Dock (Safari compatible).
El service worker cachea la interfaz para abrirla offline tras la primera visita.
