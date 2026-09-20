# CardEX v1.10.0 — 30.º aniversario

## Instalar

Este paquete actualiza la versión 1.9.0. Conserva el escáner, el modo holográfico, la identificación japonesa y tus índices actuales.

1. Descomprime el ZIP.
2. Sustituye `index.html` en la raíz de CardEX.
3. Añade los cinco archivos de la carpeta `data` del ZIP a la carpeta `data` del repositorio. NO borres los demás archivos. Los nombres nuevos empiezan por `anniversary-`.
4. Guarda los cambios y espera a que termine correctamente GitHub Pages.
5. Abre https://garciatalavera2003-code.github.io/CardEX/?v=1.10.0 y comprueba la versión y el panel «30.º aniversario».

No subas el ZIP cerrado. No es necesario ejecutar Run workflow: los datos ya están preparados. Este no es un paquete para un repositorio vacío. Si aún tienes la versión 1.8, conserva también los archivos del índice japonés entregados con 1.9.

## Cobertura real de esta entrega — 20 de septiembre de 2026

| Colección | Fichas distintas | Imágenes indexadas EN | Estado |
|---|---:|---:|---|
| 30th Celebration (`30th`) | 158 | 158 | Reconocimiento visual y por texto, con revisión de número/edición |
| 30th Classic Collection (`30th-c`) | 30 | 0 | Fichas consultables; sin identificación visual automática hasta incorporar referencias verificadas |
| Promocionales fuera de esas dos colecciones | No verificado | No añadido | Pendiente de identificar listado y referencias |
| Nuevas versiones japonesas del aniversario | No verificado | No añadido | Pendiente de referencias japonesas verificadas; se conserva el índice japonés anterior |

Hay 188 fichas por idioma (inglés y español); son 188 cartas distintas, no 376 cartas distintas. El índice visual añadido utiliza imágenes inglesas. Se incluyen también descriptores locales de las 158 imágenes para evitar descargar múltiples referencias durante la primera comparación.

**No es correcto afirmar que esta entrega reconoce visualmente todas las cartas del aniversario.** Las 30 clásicas carecen de imagen en el catálogo consultado. No se han usado las imágenes de ediciones antiguas como si fueran nuevas. Tampoco se han inventado imágenes, números impresos ni equivalencias japonesas.

## Cómo usarlo

Escanea frontal y reverso como antes. Las referencias nuevas entran en la búsqueda general automáticamente.

Si estás comprobando exclusivamente esta colección, activa «Buscar solo en el 30.º aniversario» y pulsa «Identificar Pokémon». El filtro se aplica tanto al catálogo como a la búsqueda visual. Desactívalo para volver a comprobar otras colecciones.

En las cartas con reflejos, utiliza «Modo holográfico / reflejos».

Revisa el sello del aniversario y la numeración. Una ilustración coincidente puede pertenecer a otra edición. Para las nuevas candidatas se intenta leer el texto incluso si existe una coincidencia visual fuerte. Una ficha nueva sin número corroborado queda para confirmación; las clásicas sin imagen no se proponen automáticamente como verificadas.

## Cambios técnicos

- Los nuevos vectores se añaden al índice inglés al cargarlo. Se deduplican por ID y no se modifican los archivos ingleses/japoneses existentes.
- Se incorporan fichas y colecciones nuevas aunque el navegador conserve un catálogo anterior en caché.
- Las fichas completas de las dos colecciones se incluyen en el paquete, en EN y ES.
- El panel distingue fichas disponibles de imágenes indexadas. Después de cargar el motor, el contador EN incluye el suplemento; si tu base conserva 19.507 entradas sin estas cartas, pasa a 19.665. Si ya estaban incorporadas, no se cuentan dos veces.
- Si falta el suplemento o está dañado, se muestra un aviso y se conserva la búsqueda anterior.
- Grading y clasificación automática del acabado no se han ampliado en esta actualización.

## Validación realizada

Se comprobaron 188 fichas EN y 188 ES, las 158 imágenes descargadas, los tamaños de los archivos binarios y sus referencias locales. Las 30 ausencias de imagen corresponden explícitamente a Classic Collection.

Se verificó recuperación visual y correspondencia de detalles para Exeggcute 001, Ultra Ball 128, Alolan Exeggutor 129, Mewtwo ex 157 y Mew ex 158 usando imágenes de referencia. También se probaron caché antigua, duplicados, filtro vacío, rechazo de una imagen blanca, protección de fichas clásicas sin imagen y lectura de texto en candidatas del aniversario.

Las pruebas anteriores de captura y reconocimiento japonés siguen pasando. Estas son pruebas de código e imágenes de referencia; no se ha probado esta actualización con tus cartas físicas ni en un iPhone 17 Pro Max.

## Para completar lo que falta

Necesitamos una galería verificable o fotografías nítidas de las 30 clásicas y un listado de las promocionales concretas que quieras comprobar. Las versiones japonesas necesitan sus referencias propias; no basta con traducir una ficha inglesa.

Fuentes de los datos:
- https://api.tcgdex.net/v2/en/sets/30th
- https://api.tcgdex.net/v2/en/sets/30th-c
- https://api.tcgdex.net/v2/es/sets/30th
- https://api.tcgdex.net/v2/es/sets/30th-c

Las fichas y los enlaces de imágenes proceden de TCGdex. Los diseños y marcas pertenecen a sus respectivos titulares.
