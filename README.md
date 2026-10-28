# Plantilla de colección digital

Plantilla para publicar una colección digital de patrimonio escrito con sus metadatos y sus
transcripciones. Está preparada para la sesión práctica de digitalización del Máster en Humanidades y
Patrimonio Digitales de la UAB y deriva de
[CollectionBuilder-Sheets](https://github.com/CollectionBuilder/collectionbuilder-sheets).

La web se construye con GitHub Pages y lee los metadatos de una hoja de Google Sheets publicada como
CSV: los cambios en la hoja se ven al abrir la web en una ventana nueva, sin tocar el repositorio.
Trae como ejemplo una colección de nueve portadas y encabezamientos de impresos hispánicos.

## Qué se edita

Todo puede editarse desde la web de GitHub, sin instalar nada.

| Qué | Dónde |
| --- | --- |
| Metadatos y transcripciones de los objetos | La hoja de Google Sheets |
| Título, subtítulo, descripción, autoría, enlace a la hoja, imagen de cabecera y aspecto | El primer bloque de `_config.yml` |
| Criterio, fuentes, método de digitalización y de transcripción, autoría | `pages/about.md` |
| Másteres, copias de trabajo y transcripciones | `_coleccion/` (ver su README) |
| Imágenes que se publican desde la colección | `objects/` |

## Estructura

| Carpeta o archivo | Contenido |
| --- | --- |
| `_config.yml` | Datos de la colección y opciones técnicas |
| `pages/` | Páginas de la web; solo `about.md` necesita texto propio |
| `_coleccion/` | Archivos de trabajo de cada objeto; está en el repositorio, pero no se publica |
| `objects/` | Versiones de publicación de las imágenes que no se enlazan desde la institución |
| `docs/` | `metadata-template.csv`, con las columnas de la hoja, y `ejemplo-sheet.csv`, la hoja del ejemplo |
| `assets/ejemplo-metadata.csv` | Copia del ejemplo que la web lee mientras no se enlaza una hoja |
| `_data/`, `_includes/`, `_layouts/`, `_sass/`, `assets/` | Código y configuración de la plantilla; no hace falta tocarlos |

## Columnas propias de esta plantilla

Además de los campos de CollectionBuilder, la hoja tiene tres columnas:

- `record_url`: enlace al registro del objeto digital en el portal de la institución.
- `transcript`: texto de la transcripción, que la página del objeto muestra junto a la imagen.
- `transcript_method`: cómo se hizo la transcripción (herramienta y modelo, fecha, si se revisó).

`identifier` recoge la signatura del ejemplar y `source`, la institución que lo conserva.

## Créditos y licencia

El código procede de CollectionBuilder, un proyecto de la Biblioteca de la Universidad de Idaho, y se
distribuye con licencia [MIT](LICENSE). Las imágenes y los textos de cada objeto tienen los derechos
que indican sus columnas `rights` y `rightsstatement`.
