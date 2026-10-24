CÍCLICA — primera versión funcional

Contenido:
- index.html: interfaz y lógica de la aplicación
- manifest.json: metadatos de instalación PWA
- sw.js: caché básica para abrirla offline tras la primera carga
- icon.svg: icono de la aplicación

Cómo probar:
1. Extrae el ZIP.
2. Sirve la carpeta mediante un servidor local (por ejemplo, VS Code Live Server) o súbela a un hosting HTTPS.
3. Abre la dirección en Chrome/Edge y elige “Instalar aplicación” o “Añadir a pantalla de inicio”.
4. Los datos se guardan en el almacenamiento local del navegador.

Importante:
- Abrir index.html con file:// permite probar parte de la app, pero service worker e instalación PWA requieren un contexto seguro (HTTPS o localhost).
- Es un prototipo inicial. Antes de usarlo con datos importantes, prueba exportación/importación y conserva copias de seguridad.
- El almacenamiento local no equivale a cifrado; protege también el acceso al dispositivo.
