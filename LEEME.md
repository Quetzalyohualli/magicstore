# Quetzalyohualli · Página web

## Qué hay en esta carpeta

- `index.html`: la página.
- `img/`: todas las fotos.
- `inventario.csv`: copia de respaldo del inventario.

La página ya está **conectada a la hoja "Inventario Quetzalyohualli"** de Google Sheets, que está en la carpeta Quetzalyohualli de Google Drive. Las existencias se cambian ahí, no en este archivo.

## Subir la página a GitHub Pages

1. En tu repositorio de GitHub usa "Add file → Upload files" y arrastra **el contenido** de esta carpeta: `index.html`, `inventario.csv` y la carpeta `img`. Si ya existían, se reemplazan.
2. Toca "Commit changes".
3. En **Settings → Pages**, la rama debe ser `main` y la carpeta `/ (root)`.
4. En uno o dos minutos la página queda en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPOSITORIO/`.

## Actualizar existencias

Abre la hoja **Inventario Quetzalyohualli** (también funciona desde la app de Google Sheets en el celular) y cambia la columna **estado**:

- `Disponible`: la pieza se ve normal, con su botón "Apartar".
- `Agotada` (también sirve `Vendida` o `Apartada`): aparece el sello "Agotada", la pieza pasa al final de su categoría y el botón cambia a "Pedir una similar".
- `Oculta`: la pieza desaparece de la página sin borrarla.

La columna **precio** es opcional: si escribes un número, por ejemplo `850`, la página muestra "$850 MXN". Si la dejas vacía, no se muestra precio.

La página revisa el inventario cada vez que alguien la abre. Google tarda unos **5 minutos** en actualizar la versión publicada de la hoja.

## Reglas para no romper nada

- No cambies los códigos ni los títulos de las columnas (codigo, pieza, categoria, estado, precio).
- La primera fila de la hoja siempre debe ser la de títulos: no agregues notas encima.
- No despubliques la hoja (Archivo → Compartir → Publicar en la web). Si se despublica, la página muestra todo como disponible.
- Una pieza nueva necesita sus fotos y textos dentro de la página; agregar una fila a la hoja no basta.
