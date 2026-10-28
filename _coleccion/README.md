# Archivos de trabajo de la colección

Esta carpeta está en el repositorio, pero no se publica en la web: Jekyll omite las carpetas que
empiezan por `_`. Cada archivo lleva como nombre el `objectid` de su fila en la hoja de metadatos.

- `01-master/`: la imagen tal como se descarga de la institución o se captura. No se edita.
- `02-trabajo/`: una copia del máster para recortar, girar o ajustar, y la que se usa para transcribir.
- `03-transcripciones/`: un archivo de texto por objeto con la transcripción revisada. Su contenido se
  pega en la columna `transcript` de la hoja.

La imagen que se ve en la web sale de la columna `filename`:

- Si la institución ofrece una URL estable de la imagen, por `https`, se pone esa URL. Es la opción
  preferente: cita la fuente original y evita publicar copias de copias.
- Si la imagen no puede enlazarse, se prepara una versión de publicación a partir de la copia de
  trabajo, de unos 1600 px de lado largo, se sube a la carpeta `objects/` de la raíz y en `filename`
  se escribe solo el nombre del archivo.

En la colección de ejemplo, el *Quijote* y las *Novelas exemplares* tienen como máster la doble página
que ofrece el portal y como copia de trabajo la portada recortada. El Garcilaso de 1604 es el único
objeto que se publica desde `objects/`.
