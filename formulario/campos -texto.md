Campos de Texto
Campo de texto básico
Es el campo más sencillo que podemos utilizar:


<input type="text">


<p>
	<label for="campoNombre">Nombre:</label>
	<input type="text" name="campoNombre" id="campoNombre">
</p>
Nombre: 

Contraseña
Es un campo de texto, igual que el básico, solo que cuando el usuario escribe en él, en vez de aparecer letras, aparecen asteriscos, puntos...


<input type="password">


<p>
	<label for="campoClave">Contraseña:</label>
	<input type="password" name="campoClave" id="campoClave">
</p>
Contraseña: 

Email
Es un campo de texto, pero destinado a escribir direcciones de e-mail.


<input type="email">


<p>
	<label for="campoEmail">E-mail:</label>
	<input type="email" name="campoEmail" id="campoEmail">
</p>
E-mail: 
 

El campo ofrece una pequeña validación automática y en un dispositivo con teclado virtual, las teclas variables aparecerán con los caracteres necesarios para escribir un e-mail (la arroba, el punto...):

teclado e-mail

URL
Es un campo de texto, pero destinado a escribir direcciones web.


<input type="url">


<p>
	<label for="campoURL">Sitio Web:</label>
	<input type="url" name="campoURL" id="campoURL">
</p>
Sitio Web: 

En un dispositivo con teclado virtual, las teclas variables aparecerán con los caracteres necesarios para escribir una URL (., /, ...):

teclado url

Teléfono
Es un campo de texto, pero destinado a escribir teléfonos.


<input type="tel">


<p>
	<label for="campoTfno">Teléfono:</label>
	<input type="tel" name="campoTfno" id="campoTfno">
</p>
Teléfono: 

En un dispositivo con teclado virtual, las teclas variables aparecerán con los caracteres numéricos:

teclado teléfono

Área de texto
Es un campo de texto multilínea, pensado para que se escriba en él gran cantidad de texto, que tiene una etiqueta propia (no es un input):

Para especificar el ancho del área de texto (medido en caracteres) utilizaremos el atributo cols, y para el número de líneas, rows.


<p>
	<label for="campoComentarios">Escriba sus comentarios:</label><br>
	<textarea name="campoComentarios" id="campoComentarios" cols="60" rows="6">
	</textarea>
</p>
Escriba sus comentarios:
		

Búsqueda
Es un campo de texto, pero destinado al campo del término de búsqueda.


<input type="search">


<p>
	<label for="campoBuscar">Texto a Buscar:</label>
	<input type="search" name="campoBuscar" id="campoBuscar">
</p>
Texto a Buscar: 

Los navegadores deberían de implementar este campo con alguna funcionalidad extra que lo diferencie de un campo de texto básico.

anotaciones

consejo. name poner igual que ide
+ dos formas de hacerlo, posicionamiento label y luego input o englobamiento, input dentro de label, depende de la maquetación. 

+ inserción de campos:
  + etiqueta 'input' , no tiene etiqueta de cierre, todos van a acompañados de un texto llamado etiqueta de campo de formulario, para agregarlo poner delante del input
    + tipos, asi haces una breve validación de los datos
      + `text` para textos, sale un recuadro y puedes escribir, si es largo hace scroll horizontal
        + atributo `name` , para recoger el dato, com osi fuera el pasaporte, sin especias, sin empezar por numero, como un id, usar descriptivos cortos o abreviados
        + `id` etiqueta única, aconseja poner como nombre
        + `label`etiqueta del nombre, hay qeu poner para que campo es.
        + `label` form="id-del-campo"
      + `password` campo de contraseña, es un campo de texto mejorado que no enseña lo que est´´a escribiendo. seguridad tipo password nula, si tiene un  ojo abierto y cerrado, lo único que hace es cambiar en las herramientas de desarrollo cambiar la etiqueta de password, por text
    + `email` obliga a tener un @ porque tiene que ser tipo email. en teclados virtuales hace qeu se asome el arroba por ejemplo. es bueno validar en html , en javascript y luego volver a validar en el servidor que es mas difícil explotarlo
    + `url` no tiene validación. seria para poner un sitio web, en teclado virtual aparecería la barra, el .com, las www,....
    + `tel` para teléfonos, la validación es bestial, por teléfono fijo y teléfono móvil. por ejemplo poner validación de móvil empieza por 6 o es un móvil extranjero, entonces no hay validación, pero el el techado virtual aparecería el modo teclado numérico
+ boton
  + <input type="submit" value="lo que se quiera  mostrar">




despues de rellenar si hemos hecho conget ara saber sihemos hevho bien o mal. depsue sd enevar copiar laurl del navegar. en este caso es: http://127.0.0.1:5500/Ejercicios/html-7-formulario/index.html?nombre-grupo=orion+child&album-grupo=aesthesis&contrase%C3%B1a-grupo=mielmadev&email-grupo=orion%40child.com

analizarla:
http://127.0.0.1:5500/Ejercicios/html-7-formulario/index.html?
nombre-grupo=orion+child
&
album-grupo=aesthesis
&
contrase%C3%B1a-grupo=mielmadev
&
email-grupo=orion%40child.com


+ area de texto: se puede hacer mas grande el bloque de escritura mientas se esta escribiendo lo puedes ampliar con el ratón desde la parte derecha inferior.
máximo de caracteres se hace por js. descripción de redimensionar con js o css.
  +	<label for="comentarios-grupo">
    Comentarios:
  <textarea name="comentarios-grupo" id="comentarios-grupo" rows="4" cols="50">
  </textarea>
  </label>
    + `rows` cantidad de lineas que quieres que tenga
    + `cols` cantidad unidad orientativa que quieres que tenga, teniendo en cuenta que `i` y `w` no tiene la misma anchura.
  + si en cierre de textarea tiene salto delinea o sangria, el texto del area tendra ese salto de linea o sangris.
  + si quiero que salga texto dentro del area de texto predefinido rellenar entre la etiqueta de abrir y cerrar.
+ prerrellenar los campos
  + si ya habias rellenado el formulario y estaba guardado, al intentar coambiar los datos agregar value="nombre que se quiera", pero eso se hacea mano
+ busqueda
  + <input type="search" name="buscar-grupo" id="buscar-grupo" placeholder="Buscar grupo">
    + placeholder: 

    

