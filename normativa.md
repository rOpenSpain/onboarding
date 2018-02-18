---
title: Normativa de rOpenSpain
---

## Propuesta de nuevos paquetes

- Para que un paquete sea considerado para su inclusión en rOpenSpain, el
  mantenedor del paquete debe iniciar una _issue_ en el repositorio
  [rOpenSpain/onboarding](https://github.com/rOpenSpain/onboarding).
- Un miembro de rOpenSpain actuará como editor y asignará un revisor para
  continuar con el proceso posterior.
- Los paquetes se revisan para comprobar que su inclusión se adecua a los
  objetivos del proyecto, y para cumplir unos mínimos estándares de calidad,
  claridad y documentación. Consulta las [directrices](directrices) para
  paquetes para más información. Durante el proceso de revisión, que tiene
  lugar íntegramente en la _issue_ antes mencionada, el revisor podrá resolver
  dudas y pedir cambios siguiendo dichas directrices.
- Cuando se hayan resuelto las principales cuestiones y problemas, el editor
  responsable tomará una decisión con respecto a la aceptación o no.

## Objetivos y alcance

rOpenSpain tiene como objetivo apoyar el desarrollo de paquetes que fomentan la investigación reproducible y gestionan el ciclo de vida de los datos para las ciencias. Los paquetes remitidos a rOpenSpain deben entrar dentro de esta categoría, permitir el analisis reproducible, o fometnar el uso de los datos abiertos con especial incidencia en el mundo hispano. Si no estás seguro de si tu paquete encaja en nuestros criterios, por favor abre un issue con el asunto: `petición pre-envío`.

Aunque intentamos mantener un criterio consistente y estable en el tiempo, este es un proyecto vivo, con muchos colaboradores, y por tanto sujeto a cambios. De manera que pueden existir paquetes aceptados en los inicios del proyecto que no cuimplirían la normativa actual. Por ello prometemos estudiar caso por caso y en algunas ocasiones se podrían hacer excepciones si el paquete resulta, a nuestro criterio, de especial interés.

rOpenSpain se esfuerza en promover buenas prácticas de desarrollo, que de lugar a software de calidad. Para asegurarnos de que se cumplen nuestros criterios revisamos todas las peticiones en nuestro proceso de onboarding y aún existiendo aceptación, mantenemos la vigilancia para que las normas de calidad se cumplan, fomentando las mejoras y la correción de errores.

A pesar de nuestros esfuerzos, sin embargo los errores son responsabilidad de los autores, de modo que el software defectuoso o que adolece de un mantenimiento adecuado y estable podrá ser eliminado de nuestro repositorio en cualquier momento si lo consideramos necesario.

## Propiedad de los paquetes

Los autores de los paquetes aceptados mantienen la misma propiedad y rol sobre
los mismos que tenían previa a su inclusión en rOpenSpain. Los mantenedores
serán incluidos como miembros de rOpenSpain y seguirán teniendo permisos de
escritura en su repositorio. Si se requiere que otros colaboradores tengan
también permisos de escritura, hay que solicitar su inclusión como miembro a un
administrador de rOpenSpain.

## Paquetes eliminados

En caso de que por alguna razón alguno de los contribuyentes retirase uno de sus paquetes, mantenemos el derecho de poseer una copia del mismo por motivos de archivo.

## Responsabilidades de los mantenedores

Los mantenedores son responsables de sus repositorios, debiendo de atender a las normas dictadas desde rOpenSpain y seguir en todo momento las instrucciones de los miembros del equipo rector de rOpenSpain.

Deben así mismo responder en tiempo y forma a las peticiones de resolución de errores desde CRAN o desde rOpenSpain, existiendo un plazo de aproximadamente 3 meses para solucionar los fallos detectados. Los miembros del equipo rector de rOpenSpain se dirigirán al mantenedor al menos en tres ocasiones para recordarle su responsabilidad, y si tras dicho periodo o tras los avisos, el problema sigue sin resolver, rOpenSpain se reserva las medidas a tomar en tal caso.

Este periodo de tres meses es orientativo, dado que no siempre todos los colaboradores tienen el mismo número de compromisos o tiempo para dedicar al proyecto, y en cualquier caso se puede acortar o alargar en función de la gravedad del error. La definición del nivel de la gravedad del un error puede ser algo subjetivo, por lo que aportamos unos ejemplos:

- Errores que deben corregirse de manera inmediata:
    - El paquete es una dependencia de otros paquetes (1 o varios) en CRAN, de modo que el fallo está provocando errores en los paquetes que dependen de él.
    - El paquete puede que no tenga otros dependientes de él en CRAN, pero es ampliamente usado, y por tanto es necesario que sea corregido con celeridad.

- Casos en que podemos esperar un poco más:
    - El paquiete no está en CRAN, o estando en CRAN no es dependencia para ningún otro.
    - El paquete necesita algunas correcciones, el mantenedor ha respondido pero está muy atareado en un nuevo trabajo, o por otras reazones de índole personal, pero se ha comprometido a corregirlo pronto.

Requerimos a todos los mantenedores que se aseguren de recibir las notificaciones de GitHub así como comprobar que los mensajes de los miembros del equipo rector de rOpenSpain no están terminando en la carpeta de spam. Además, tenemos la opción del canal Slack de rOpenSpain para mantener el contacto entre los miembros de la comunidad.

En caso de que un autor abandone el mantenimiento de su paquete, nos reservamos el derecho de solicitar a CRAN que rOpenSpain aparezca como mantenedor del mismo.

## Código de Conducta

* Estamos comprometidos con proveer de un ambiente amistoso, seguro y abierto para todos los desarrolladores sin importarnos su procedencioa, género, orientación sexual, ideología o cualquier otra característica personal. No son temas de nuestra incumbencia, pero no toleraremos que se usen como argumentos en contra de nadie.

* Debe evitarse el uso de nombres o avatares con contenido sexual explícito, o que incumplan las normas de educación, el sentido común, o que vayan contra el mantenimiento de este ambiente amistoso y agradable que todos pretendemos.

* Por favor, sé amable y educado. Todos tenemos un mal día pero en ese caso siempre es mejor que todos nos traten con amabilidad. No es necesario ser maleducado.

* Respeta que los demás tengan diferencias de opinión al respecto del software y que cada decisión sobre el mismo conlleva que todos deben de ceder en algún momento. Raramente hay respuestas corectas a todas las preguntas.

* Por favor, mantengamos las críticas no constructivas al mínimo. Al final, si crees que las cosas se pueden hacer mejor, puedes hacer un _fork_ y demostrarlo.

* Te expulsaremos si insultas, humillas o acosas a alguien. No aceptamos este tipo de conductas. Somos una comunidad que trata de fomentar la calidad del software, no un foro de discusión donde todo está permitido. En especial estaremos atentos a las conductas misóginas o contra colectivos desfavorecidos o minoritarios.

* Si consideras que has sido acosado, humillado o insultado por un miembro de la comunidad, ponte en contacto con nosotros en hola@ropenspain.es enviando una captura de pantalla si es posible. Estamos comprometidos con un ambiente amistoso y agradable para trabajar donde podamos recibir la ayuda que no siempre encontramos en otros sitios.

* De la misma manera, no se permite la publicidad no solicitada, las discusiones estériles o incendiarias, acaparar la atención con temas que estén muy lejos del objetivo fundamental de la comunidad rOpenSpain, o cualesquiera otras manifestaciones que no contribuyan a los objetivos generales de la comunidad rOpenSpain.

* Si consideras que este código de conducta debe incluir alguna otra recomendación, haznoslo saber en nuestro formulario de contacto o a través del correo electrónico.

---













