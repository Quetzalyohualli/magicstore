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
- Precios dobles: escribe `80/145` para "$80 c/u, 2 piezas por $145".

## Agregar una pieza nueva

1. Sube la foto de la pieza a la carpeta `img` del repositorio (por ejemplo `cetro-amatista.jpg`). De preferencia vertical, sin textos encima.
2. En la hoja agrega una fila nueva con:
   - **codigo**: un código que no exista (por ejemplo `CE-01`).
   - **pieza**: tipo y nombre separados por " · " (por ejemplo `Cetro · Cetro de amatista`).
   - **categoria**: el nombre exacto de una categoría (Pulseras, Anillos y dijes, Cuarzos y cristales, Esferas y corazones o Rodados). Si escribes otra, se crea una categoría nueva.
   - **estado** y **precio**, como las demás.
   - **descripcion** (columna F, opcional): una o dos frases sobre la pieza.
   - **imagen** (columna G): el nombre del archivo que subiste, por ejemplo `cetro-amatista.jpg`.
3. La pieza aparece sola en su categoría. Si no pones imagen, se muestra con el sello de la Q mientras tanto.

Las piezas agregadas así se muestran con su foto, nombre, descripción y precio. Si quieres la ficha completa (dos fotos, minerales e intención, como las demás), pídeselo a Claude con la lámina del catálogo.
