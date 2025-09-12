# Programación web en entorno cliente
## HTML
### Formulario
#### Atributos Extra

#### placeholder
Permite incluir un texto a modo de ayuda para rellenar un campo de formulario:

```html
<p>
    <label for="campoNombre">Nombre:</label>
    <input type="text" name="campoNombre" id="campoNombre" placeholder="tu nombre...">
</p>
```

El atributo `placeholder` no debe usarse como alternativa al elemento `label` cada uno tiene una misión diferente. Si no se quiere visualizar por pantalla el elemento , simplemente habrá que ocultarlo por CSS, pero no se debe eliminar del código.

`label` obligatorio `placeholder` opcional

#### size
Permite indicar el ancho del campo en función del nº de caracteres y su tamaño base (al igual que ocurría con el atributo cols en el elemento textarea):

<p>
    <label for="campoNombre2">Nombre:</label>
    <input type="text" name="campoNombre2" id="campoNombre2" size="5">
</p>

Generalmente este atributo no se utiliza demasiado puesto que la tendencia suele ser igual en anchura todos los campos de formulario, y eso se logrará mediante CSS.

#### maxlength
Permite restringir el nº máximo de caracteres que se pueden escribir en un campo:

<p>
    <label for="campoNombre3">Nombre:</>
    <input type="text" name="campoNombre3" id="campoNombre3" maxlength="10">
</p>


#### disabled
Permite deshabilitar un campo de formulario o botón:

<p>
    <label for="campoEmail">Email:</>
    <input type="email" name="campoEmail" id="campoEmail" disabled>
</p>

Podemos usar también disabled="disabled"

Si un campo de formulario tiene este atributo `disabled`, el valor que tenga no se enviará con el formulario.


#### readonly
Permite establecer un campo de formulario como sólo lectura (se puede copiar el contenido pero no editarlo):

<p>
    <label for="campoEmail2">Email:</>
    <input type="email" name="campoEmail2" id="campoEmail2" value="jane@doe.es" readonly>
</p>

Podemos usar también readonly="readonly"

Si un campo de formulario tiene este atributo `readonly`, el valor que tenga sí se enviará con el formulario.

#### autocomplete
Se utiliza para activar o desactivar el `autocomplete` de un formulario o de un campo concreto:

<form autocomplete="off">
<input type="text" name="nombre" autocomplete="off">

#### spellcheck
Activa o desactiva la propiedad de revisión ortográfica en un contenido editable:

<input type="text" spellcheck="false">
<textarea spellcheck="true">

#### autofocus
Permite forzar al navegador a que sitúe el foco en un campo de formulario determinado, de manera nativa (sin necesidad de utilizar javascript):

<input type="text" autofocus>
