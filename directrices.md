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

* Las funciones que manipulan un objeto o dato concreto y retornan un objeto o dato del mismo tripo recomendamos que lleven como primer argumento dicho dato u objeto. De este modo ganars compatibilidad con el operador tubera (pipe) de magrittr (`%>%`)

* Para más información sobre cómo adaptar estilos de código, funciones y scripts en R, recomendamos la lectura del capítulo dedicado a este tema en el conocido [libro de Hadley Wickam](http://r-pkgs.had.co.nz/r.html).

## Documentación

TBD

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
