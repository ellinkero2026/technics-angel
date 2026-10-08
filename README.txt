TECHNICS ANGEL — versión PWA para Android

NO NECESITÁS ANDROID STUDIO.

QUÉ INCLUYE
- index.html: tu página adaptada como aplicación web instalable.
- manifest.json: configuración de la app Android/PWA.
- sw.js: caché básica para funcionamiento offline de la interfaz.
- icon-192.png / icon-512.png: iconos de la app.
- Se corrigió además el problema de restauración del ecualizador (gains).

CÓMO INSTALARLA EN ANDROID
1. Subí TODOS estos archivos a un hosting que use HTTPS.
2. Abrí la dirección desde Chrome en tu teléfono Android.
3. Elegí "Instalar aplicación" o "Agregar a pantalla de inicio".
4. La app aparecerá con su propio icono y se abrirá en modo independiente.

IMPORTANTE
- No sirve abrir index.html directamente desde "Archivos" del teléfono (file://), porque
  los Service Workers y la instalación PWA necesitan un sitio web servido por HTTP/HTTPS.
- Los MP3 que agregues desde la propia app siguen usando IndexedDB, como en tu página original.
- El funcionamiento offline de la interfaz depende de haber abierto la app al menos una vez
  con conexión para que el navegador guarde los recursos.

Si querés un APK instalable directamente, esta misma base se puede envolver como APK mediante
un servicio de compilación/cloud build; no hace falta instalar Android Studio en tu PC.
