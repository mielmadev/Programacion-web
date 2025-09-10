# Programación web en entorno cliente

## HTML

### Formulario

#### Elemento Form

Utilizamos los formularios para recoger información que los usuarios introducen en las páginas web. Después la procesaremos para, por último, guardar esa información en una base de datos, mostrar unos resultados de búsqueda, finalizar un proceso, etc.

Para implementar un formulario utilizaremos el elemento `form` y dentro ubicaremos los campos de formulario.

```html
<form>
    <!-- campos del formulario -->
</form>
```

---

#### Configuración

En el formulario, con unos atributos específicos y obligatorios, vamos a indicar unas opciones de configuración:

- **Qué tipo de datos vamos a enviar** (codificación de datos)
- **Cómo se van a enviar** (método de transmisión)
- **A dónde se van a enviar** (la acción)

---

##### Codificación de datos

Con el atributo `enctype` indicamos la codificación de los datos. Tenemos 2 opciones:

- **text/plain**:  
  Se envían los datos como texto plano.

- **multipart/form-data**:  
  Es el adecuado si se van a enviar archivos adjuntos, además de datos. Si no se utiliza esta opción, el formulario sólo envía el nombre del archivo, pero no el archivo en sí mismo.

---

##### Método de transmisión

Con el atributo `method` indicamos el método de transmisión de datos. Tenemos 2 opciones:

- **get**:  
  Los datos se envían a través de la URL, los podemos ver en la barra de dirección (y por lo tanto, podemos manipularlos).

- **post**:  
  Los datos se envían de forma transparente para el usuario, sin que los podamos ver.

> Utilizaremos siempre el valor `post` puesto que a nivel de seguridad es lo mejor. Sólo en el caso de que haya una justificación concreta para usar el valor `get` utilizaremos esta otra opción.

---

##### Acción

Con el atributo `action` indicamos dónde vamos a enviar el formulario. Tenemos varias opciones:

- **A una página**:  
  Puede enviarse sobre sí mismo o bien a otra página.

- **A un e-mail**:  
  Si el usuario tiene instalado un software de gestión de correo electrónico (Outlook, Thunderbird...), al enviarlo, se le abrirá un nuevo mensaje de correo con los datos que ha rellenado del formulario y luego tendrá que enviar dicho e-mail.  
  > Actualmente este sistema no está recomendado porque los usuarios utilizan gestores de correo online y no un software específico, por lo tanto, no funcionaría este envío.

> Si no indicamos un valor en este atributo, el formulario se enviará sobre sí mismo, pero esto provoca vulnerabilidades de seguridad, por lo que siempre es recomendable establecer un valor, y si realmente se quiere enviar el formulario sobre la misma página, poner el nombre del archivo en el atributo.

---

##### Ejemplos

```html
<form action="mailto:info@empresa.com" method="post" enctype="text/plain">
    <!-- campos del formulario -->
</form>

<form action="index.html" method="get" enctype="text/plain">
    <!-- campos del formulario -->
</form>

<form action="envio.html" method="post" enctype="multipart/form-data">
    <!-- campos del formulario con envío de archivo -->
</form>
```

---

#### Otros atributos para el formulario

Tenemos 2 atributos más que, aunque no son obligatorios, sí que son altamente recomendables para el buen funcionamiento del formulario:

- **name**:  
  Es un identificador, muy similar al atributo `id`, que necesitan tanto el navegador como un lenguaje de programación que procese el envío del formulario. También sirve para conocer qué formulario se ha enviado, si en la página existen varios formularios.

- **id**:  
  Es un identificador único para el formulario. Nos va a servir para poder hacer un enlace a este elemento, para seleccionar el elemento mediante Javascript, CSS...

> Generalmente vamos a utilizar el mismo valor para estos 2 atributos (a excepción de un campo de formulario específico que no puede hacerse de esta manera), para no tener que pensar en dos valores diferentes. Podemos tratar estos dos atributos como si `id` fuera nuestro DNI y `name` fuera nuestro Pasaporte.

```html
<form name="formcont" id="formcont" action="index.html" method="get" enctype="text/plain">
    <!-- campos del formulario -->
</form>
```

---

#### Inserción de campos

La mayor parte de los campos de formulario se implementan con el elemento `input`. Para diferenciar unos de otros, utilizaremos el atributo `type` con un valor concreto y de esta manera podremos tener un campo de texto, uno de contraseña... hasta el botón de envío del formulario.

Cada campo de formulario llevará varios atributos (unos opcionales, otros obligatorios) y se tendrá que asociar explícitamente con un texto que nos indique qué dato tenemos que introducir en el campo.

---

##### Campo de texto básico

```html
<input type="text">
```

Para poder utilizar el campo en el formulario, tenemos que añadir inicialmente una serie de atributos y contenido:

- **atributo name**:  
  Es un identificador (muy similar al atributo `id`), a través del cual se recoge el valor que haya introducido el usuario por parte del navegador y lenguaje de programación.

- **Etiqueta / rótulo**:  
  Es un texto que acompaña al campo de formulario para indicar el dato que hay que rellenar en dicho campo.

Ejemplo:

```html
Nombre: <input type="text" name="campoNombre">
```

En este momento el campo sería funcional, pero todavía nos falta añadir un código extra para que esté completo. Tenemos que asociar explícitamente la etiqueta al campo de formulario.

---

##### Asociación explícita con label

Esta asociación explícita se realiza utilizando el elemento `label`, que será el encargado de asociar la etiqueta con su campo de formulario correspondiente.

**Opción 1:**

```html
<label>Nombre:</label>
<input type="text" name="campoNombre">
```

**Opción 2:**

```html
<label>
    Nombre:
    <input type="text" name="campoNombre">
</label>
```

Las dos opciones son válidas, a gusto del desarrollador.

---

Si dejamos el código así, tenemos la asociación a medio hacer, todavía nos falta añadir más código. Para que la asociación sea explícita de verdad, imaginemos que la etiqueta es un enlace que apunta al campo de formulario. Eso es lo que vamos a hacer, pero con los atributos apropiados (no con un enlace).

En el campo de formulario añadiremos un atributo `id` para establecer el identificador. Al igual que hemos hecho con el elemento `form`, vamos a utilizar el mismo valor que hemos puesto en el atributo `name`.

Después, en el elemento `label` vamos a añadir un atributo `for` y el valor será el mismo que el atributo `id`.

---

**Opción 1: Asociación explícita por posicionamiento**

```html
<label for="campoNombre">Nombre:</label>
<input type="text" name="campoNombre" id="campoNombre">
```

**Opción 2: Asociación explícita por englobamiento**

```html
<label for="campoNombre">
    Nombre:
    <input type="text" name="campoNombre" id="campoNombre">
</label>
```

---

Para terminar, podemos dar estructura a cada elemento del formulario, insertándolo dentro de un párrafo, por ejemplo:

**Opción 1: Asociación explícita por posicionamiento**

```html
<p>
    <label for="campoNombre">Nombre:</label>
    <input type="text" name="campoNombre" id="campoNombre">
</p>
```

**Opción 2: Asociación explícita por englobamiento**

```html
<p>
    <label for="campoNombre">
        Nombre:
        <input type="text" name="campoNombre" id="campoNombre">
    </label>
</p>
```



### apuntes de clase

etiqueta para formulario es `form` 

en la url de un sitio donde has rellenado y eniado un formulario lo que aparecen son los datos, manda la info de lo que estas escribiendo mediante la url,, otras veces dse puede mandar de manera invisible, que ees lo general

atributos y valores:
`method` -> metodo de envio post y get(hace que veas los parametros en la url).
buena practica hacerlo con post.

`action`-> si no lo rrelenas se te autoenvia. si no haces programacionen blanco, sino a donde queiras mandarlo.

`enctype` -> tipo codificacin de datos. si no hay archivos  porque es solo texto plano `text/plain`, si hay un archivo el atributo `multipart/form-data`. puedesa cambiar entre estos valores dependiendo de lo que necesites. 

atributo `id`
atributo `name` para saber el nombre de los cambios. name obligatorio para que java, php.... reconozca

inserción de campos: 