---
title: Directrices para paquetes
---

## Nombres de paquetes

Recomendamos nombres cortos y descriptivos en minúsculas. Si tu paquete tiene vinculaciones con servicios comerciales por favor asegúrate de que no viola las leyes de propiedad intelectual, las marcas y patentes. Puedes comprobar si el nombre del paquete está ya utilizado con una búsqueda en CRAN https://cran.r-project.org/web/packages/available_packages_by_name.html y en el listado de paquetes R de GitHub http://rpkg.gepuro.net/

¡También puedes usar el paquete [`available`](https://github.com/ropenscilabs/available) y hacerlo con R!

## Nombres de funciones y sintaxis general


* Recomendamos el uso de `snake_case` en términos generales sobre otros estilos a menos que estés aportando otro paquete que ya est en uso.

* Evita siempre conflictos de nombres entre tus funciones y las de los paquetes de base de R. También evita este conflicto con otros paquetes populares como `ggplot2`, `dplyr`, `magrittr` o `data.table`. Si quieres que tu función se use, es mejor que no se llame igual que otra que ya existe.

* Considera una nomenclatura de `objeto_verbo()` para funciones en tu paquerte que usen tipos de datos similares o interactúen con una API común. Por `objeto` nos refermios a los datos a al API y por `verbo` nos referimos a la acción principal de dicha función. Esto ayuda a evitar conflictos de nombres con paquetes que tengan similares verbos o funciones, haciendo el c digo ms legible y fácil de autocompletar. Por poner un ejemplo, en **stringi**, todas las funciones que empiezan por `stri_` manipulan cadenas de texto (`stri_join()`, `stri_sort()`, o en otyro caso, el paquete **googlesheets** ofrece funciones que comienzan por `gs_` y que son llamadas a la API de Google Sheets (`gs_auth()`, `gs_user()`, `gs_download()`).

* Las funciones que manipulan un objeto o dato concreto y retornan un objeto o dato del mismo tipo recomendamos que lleven como primer argumento dicho dato u objeto. De este modo ganars compatibilidad con el operador tubera (pipe) de magrittr (`%>%`)

* Para más información sobre cómo adaptar estilos de código, funciones y scripts en R, recomendamos la lectura del capítulo dedicado a este tema en el conocido [libro de Hadley Wickam](http://r-pkgs.had.co.nz/r.html).

## Documentación


* Todas las funciones exportadas de un paquete deben sere extensamente documentadas incluyendo ejemplos claros.

* El paquete debe de incluir documentación global que se pueda ver con la llamada a la función `?foobar`, (o `?foobar-paquete` si hay un caso de conflicto de nombres). Opcionalmente podras usar ambos comandos para el fichero del manual, utilizando `?foobar` y `?foobar-paquete` mediante etiquetas roxygen de tipo `@aliases`.

* El paquete debe de contener como mínimo una viñeta que provea una introducción a las funciones principales y casos de uso sencillos.

* Igual que en el caso del archivo README, la documentación de nivel superior o las viñetas deben ser el principal punto de entrada para los usuarios. Si tu paquete conecta a una fuente de datos externa o a un servicio online, o si envuelve otro sdoftware externo, debe de proveer suficiente información al usuario para comprender la naturaleza de el dato, el servicio, el software utilizado, etcétera. Asímismo debe proveer de enlaces a cualquier información relevante.
Por ejemplo, una viñeta no debería solamente decir cosas como: "ofrece acceso al servicio web del ..." sino que también debe de incluir un repositorio de los diferentes servicios que el citado servicio online provee, información general sobre su funcionamiento, la documentación de la estructura de los datos accedidos y sus metadatos, todo ello accesible mediante enlaces visibles.                      

* Recomendamos encarecidamente que todos los paquietes tengan como método de documentación fundamental `roxygen2`.  `roxygen2` es [un paquete R](http://cran.r-project.org/web/packages/roxygen2/index.html) cuya función principal es compilar  los ficheros `.Rd` en el directorio `man` del paquete, con sencillas etiquetas añadidas sobre cada función.

* Puedes encontrar ms información sobre roxygen2 [aquí](http://r-pkgs.had.co.nz/man.html) en el mencionado libroi sobre paquetes R.

* Una de las principales ventajas del uso de `roxygen2`  es que el `NAMESPACE` siempre se genera automáticamente y está siempre actualizado.

* Cuando utilizes `roxygen2`, añade `#' @noRd` a las funciones internas.

## Autoría

TBD

## _Testing_

TBD

## Versionado

TBD

## Dependencias

TBD

## Enlaces recomendados

TBD

---
