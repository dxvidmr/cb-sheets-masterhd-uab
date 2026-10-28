---
title: About
layout: about
permalink: /about.html
# true añade al pie de la página el crédito a CollectionBuilder
credits: true
---

<!--
Esta página se escribe en Markdown. Los comentarios como este no se ven en la web:
explican qué va en cada apartado. Sustituid el texto de ejemplo por el vuestro.
-->

<!-- Presentación breve, sin título: qué reúne la colección, quién la ha hecho, en qué contexto
y con qué herramienta. -->

Colección de ejemplo para la práctica sobre digitalización del patrimonio escrito del
Máster en Humanidades y Patrimonio Digitales de la Universitat Autònoma de Barcelona (curso
2026-2027). Reúne nueve portadas de impresos en castellano, entre 1543 y 1642, tomadas de bibliotecas
digitales a través de Europeana, con sus metadatos y una transcripción de cada una hecha con Gemini.
Está construida con [CollectionBuilder-Sheets](https://collectionbuilder.github.io/), una plantilla para
publicaro colecciones digitales utilizando tecnología [Jekyll](https://jekyllrb.com/).

## Criterio de selección

<!-- Qué reúne la colección y por qué estos objetos y no otros. -->

La colección reúne portadas y títulos de cabecera de ediciones antiguas en castellano, es decir digitalizaciones de 
páginas en las que cada edición presenta su título, sea una portada o, cuando no la tiene o el texto forma parte
de un volumen colectivo, el encabezamiento con que empieza.

## Fuentes y derechos

<!-- De dónde proceden los objetos, cómo se localizaron y con qué derechos se reutilizan. -->

Los objetos se localizaron a través [Europeana](https://www.europeana.eu) pero proceden de las bibliotecas
digitales que los publican: Memòria Digital de Catalunya, Biblioteca Digital de Castilla y León,
Patrimonio Digital de Castilla-La Mancha, Biblioteca Virtual del Patrimonio Bibliográfico y Biblioteca
Digital Ciconia. De cada objeto se recogen los derechos que declara la institución de la que se toma
la imagen: dominio público, CC0 o CC BY 4.0. Cuando un mismo ejemplar figuraba con licencias
distintas en dos portales, se ha seguido la del portal de la institución.

## Metadatos

<!-- Criterios propios para rellenar la hoja: vocabulario de materias, forma de los nombres y de
las fechas, qué se pone cuando un dato no consta. -->

Las materias combinan un género literario, uno por objeto, y un tema solo cuando agrupa varios objetos o
precisa el contenido: Poesía, Teatro, Novela, Prosa doctrinal y Crítica literaria como géneros;
Superstición y Góngora como temas. Los nombres de persona siguen la forma autorizada de los
catálogos, con sus fechas. La fuente es la institución que conserva el ejemplar y el identificador,
su signatura, o «No consta» si el registro no la da.

## Digitalización y archivos

<!-- Cómo se obtuvieron las imágenes, qué se conserva como máster y copia de trabajo,
y cuáles se enlazan desde la institución y cuáles se publican desde la colección. -->

Las imágenes se descargaron de cada portal a la mayor resolución disponible y se conservan como
máster en la carpeta `_coleccion/01-master` del repositorio. De cada una se hizo una copia de trabajo
para transcribir; en el *Quijote* y las *Novelas exemplares*, que el portal ofrece como doble página,
la copia de trabajo es la portada recortada. La web enlaza las imágenes desde la institución que las
publica, tres de ellas por IIIF. Solo el Garcilaso de 1604 se publica desde la colección, porque el
portal cambió de dominio y los enlaces que difunde Europeana ya no funcionan.

## Transcripción

<!-- Método: herramienta y modelo, fecha, prompt o prompts empleados (uno por tipo de documento,
si hay varios), qué se revisó y con qué criterios. -->

Las transcripciones se hicieron con Gemini 3.6 Thinking el 28/10/2026, a partir de la copia de
trabajo de cada imagen y con un mismo prompt para todos los objetos. Conservan la grafía, la
puntuación y los saltos de línea del original, con la ſ y el uso de u y v. Entre corchetes van los
elementos que no son texto impreso, como orlas, grabados, escudos y marcas tipográficas, y las
anotaciones manuscritas posteriores (`[añadido: …]`). Las lecturas dudosas se marcan con `[lectura?]`
y los pasajes que no se leen, con `[ilegible]`.

No se han corregido las salidas, es la transcrión literal del LLM.

El prompt empleado:

```
Transcribe el texto visible de esta imagen sin modernizar ni corregir sus grafías. Conserva las abreviaturas, el uso de mayúsculas y los saltos de línea. Marca las lecturas dudosas como [lectura?] y lo que no puedas leer como [ilegible]. Describe entre corchetes los elementos no textuales (grabado, marca tipográfica, orla, escudo) en el lugar donde aparecen. Distingue el texto impreso de los añadidos posteriores, como sellos, signaturas o anotaciones manuscritas, y señala estos últimos como [añadido: texto]. No completes por contexto ni reconstruyas palabras. Devuelve solo la transcripción con esas marcas.
```

## Autoría

<!-- Quiénes han hecho la colección y qué ha hecho cada persona, si se reparte el trabajo. -->

David Merino Recalde.
