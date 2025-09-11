# Programación web en entorno cliente
## HTML
### Archivo
Si necesitamos adjuntar un archivo en el formulario utilizamos el siguiente elemento input:


<p>
	<label for="campoCV">Adjunta tu Curriculum:</label>
	<input type="file" name="campoCV" id="campoCV">
</p>

Adjunta tu Curriculum: Ningún archivo seleccionado

De manera nativa no podemos modificar el texto ni la apariencia del botón para adjuntar el archivo. Cualquier modificación en este sentido se realiza con CSS y Javascript.

Podemos restringir el tamaño máximo permitido del archivo, en bites:


<p>
	<label for="campoCV">Adjunta tu Curriculum:</label>
	<input type="file" name="campoCV" id="campoCV" maxlength="100000">
</p>

Y también podemos controlar el tipo de archivo permitidos, mediante el atributo accept y diferentes valores de tipo MIME.:


<p>
	<label for="campoCV">Adjunta tu Curriculum:</label>
	<input type="file" name="campoCV" id="campoCV" accept="image/gif">
</p>

Incluso podemos hablitar la opción de selección múltiple de archivos:


<p>
	<label for="campoCV">Adjunta tu Curriculum:</label>
	<input type="file" name="campoCV" id="campoCV" multiple="multiple">
</p>

Lo más importante a la hora de utilizar este campo es acordarse de utilizar el atributo con el valor correcto enctype="multipart/form-data" en el elemento form, para que se envíe el archivo y no simplemente su nombre.