 # Historia de BEAM ecosystem
 
## Erlang
 es un lenguaje de programación funcional, Dinamico, que corre sobre una maquina virtual (BEAM), diseñado especialmente concurrencia y la alta disponibilidad .
 inventado incialmente para manejar sistemas de telecomunicaciones.   inventado en 1986 por Ericsson.

 ![erlang comic](resources/images/PPerlang.png)
 
 Una de las filosofias con las que se diseño el lenguaje es "let it crash", es decir, los sistemas eventualmente
 fallarán,es casí que imposible manejar todos los errores, entonces lo que hago es isolar el error en un proceso (no confundir con el concepto de proceso del Sistema Operativo),  "matarlo" y 
 volver a comenzar en un estado conocido.

 se han preguntado muchas veces como simplemente apagando y encediendo la computadora se arregla el problema?
 bueno es algo similar.

 ## Elixir
 es un lenguaje de programación funcional inventado en el 2011,que corre sobre la misma maquina virtual de erlang.
 el creador de Elixir, se preocupaba por que no habian casi buenos lenguajes para manejar de manera eficiente y efectiva la concurrencia, por lo que decidio crear Elixir, Es parecido a Erlang, pero con una sintaxis mas amigable y moderna. El creador era core contributor de Ruby on Rails, por lo que Elixir se asemeja en cierta forma a Ruby en cuanto a la sintaxis.

![elixir comic](resources/images/elixir.png)

## Otros lenguajes en BEAM
- Gleam (2016) soporte nativo de tipos y compilación a JavaScript
- LFE (2008) Lisp

# Modelo de actores
- Los actores son la unidad basica de de computación.
![actores 1](resources/images/actores_1.png)

- Los actores se comunican entre si enviandose mensajes
![actores 2](resources/images/actores_2.png)
	- los mensajes son una construccion **LIVIANA** enviar mensajes entre actores
	es casi primitivo.

- Se puede generar algo en el otro actor si le respondemos, enviamos algun mensaje.  (no responder puede ser una respuesta)
![actores 3](resources/images/actores_3.png)	
![actores 4](resources/images/actores_4.png)	

- introducir nuevos actores es muy barato en terminos computacionales (a diferencia de en la vida real)
![actores 5](resources/images/actores_5.png)


- todos se pueden enviar mensajes entre todos, al fin y al cabo cada actor es un proceso.
![actores 5](resources/images/actores_6.png)

## De eso tan bueno no dan tanto....
- No es una bala de plata
- puede ser muy bueno para manejar un servidor de videojuegos mas no para escribir un videojuego [servidor de wow en elixir ](https://pikdum.dev/posts/thistle-tea/)
- hacer paralelismo o concurrencia sobre cualquier problema, no lo va a solucionar mas rapido necesariamente, incluso lo podria hacer mas lento
- escoge la herramienta adecuada para el trabajo adecuado, o incluso combina varias herramientas para lograr el mejor resultado posible
- han creado una herramienta de modelo 3d 🤯  [wings 3d](https://www.wings3d.com)
- No es particularmente bueno en procesamiento de señales (audio o imagenes), escribir drivers de sistema operativos, en general cosas que requieran muy bajo nivel, y operaciones de alto rendimiento en el espacio numerico, aunque se esta haciendo un esfuerzo para cambiar esto, en especial en el mundo de machine learning.

	

# Casos de uso




# Recursos interactivos

[curso completo self paced de programacion funcional en Elixir](https://www.kth.se/social/course/ID1019/)

[excercism.io](https://exercism.io/tracks/elixir)
# Recursos
[Learn You Some Erlang for Great Good!](https://learnyousomeerlang.com/introduction#what-is-erlang)
[let it crash philosophy](https://www.youtube.com/watch?v=sz3tMPkl5hI)
[elixir documentary](https://www.youtube.com/watch?v=lxYFOM3UJzo)
[programs as people](https://leftoversalad.com/c/015_programmingpeople/)



