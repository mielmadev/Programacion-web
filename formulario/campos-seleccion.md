# Programación web en entorno cliente
## HTML
### formulario
### campos selección

Estos campos nos van a permitir seleccionar entre uno o varios valores ya definidos.

#### Checkbox
+ gráficamente como un cuadrado que el usuario puede activar y desactivar.
+ En este campo, el usuario no tiene que introducir ningún dato, simplemente elegir entre los datos que se le ofrecen.
+ Podrá seleccionar, una, varias, todas o ninguna de las opciones.
+ Estableceremos nosotros el dato/valor de cada campo checkbox, utilizando el atributo value.
+ En este campo, primero se inserta el campo y después su etiqueta:
+ Si queremos que una o varias opciones estén ya marcadas al entrar en la pagina, basta con añadir el atributo checked="checked" o simplemente checked en el checkbox correspondiente.


```html
<p>
  que música te gusta más?
	<input type="checkbox" name="music" id="music" value="si" checked="checked">
  <label for="metal">Metal</label>

	<input type="checkbox" name="music" id="music" value="si" checked="checked">
  <label for="rock">Rock</label>

	<input type="checkbox" name="music" id="music" value="si" checked="checked">
  <label for="pop">Pop</label>

	<input type="checkbox" name="music" id="music" value="si" checked="checked">
  <label for="opera">Opera</label>

</p>
```


#### Radiobutton
+ gráficamente por botones redondos.
+ Se utilizan normalmente cuando ofrecemos al usuario una lista de opciones de la que sólo puede seleccionar una de ellas, de forma exclusiva.
+ Este elemento es el más especial que tenemos dentro de todos los elementos input.
+ Es la única excepción donde no podremos utilizar el mismo valor para los atributos id y name. Si fueran iguales, entonces se podrían elegir varias opciones (como si fueran checkboxes)
+ Si queremos que una o varias opciones estén ya marcadas al entrar en la pagina, basta con añadir el atributo checked="checked" o simplemente checked en el radiobutton correspondiente.

Imaginemos que en un cuestionario queremos preguntar si la tortilla se prefiere con cebolla o sin cebolla. Tenemos 2 opciones y el usuario únicamente puede elegir una de ellas:


<p>
	¿Cómo te gusta la tortilla?:<br>
	<input type="radio" name="tortilla" id="tortillaCon" value="con cebolla">
	<label for="tortillaCon">Con Cebolla</label><br>
	<input type="radio" name="tortilla" id="tortillaSin" value="sin cebolla">
	<label for="tortillaSin">Sin Cebolla</label>
</p>
¿Cómo te gusta la tortilla?:
 Con Cebolla
 Sin Cebolla

#### Select
Las listas de selección tienen una función similar a la de los radiobuttons. Presentamos al usuario múltiples opciones en las que, a priori, solo puede seleccionar una de ellas. La ventaja que tienen las listas desplegables es que apenas ocupan espacio, y son muy útiles cuando tenemos muchas opciones.
+ es uan especie de lista
  + en vez de ul/ol, select
  + en vez de li, option
+ solo elegir uno
  + defecto primera opción aparece
  


##### Selección básica
La estructura nos puede recordar a la de una lista.


<p>
	<label for="campoColor">Elige un color favorito:</label>
	<select name="campoColor" id="campoColor">
		<option>negro</option>
		<option>rojo</option>
		<option>blanco</option>
		<option>verde</option>
		<option>azul</option>
	</select>
</p>
Elige un color favorito: 
negro

Si queremos que una opción esté ya marcada al entrar en la página, basta con añadir el atributo selected="selected" o simplemente selected en la opción correspondiente.

##### Selección con valor alternativo
Si queremos que, al elegir una opción, el dato que se envíe no sea el texto de la opción, sino otro valor, entonces tenemos que utilizar el atributo value dentro de cada opción:


<p>
	<label for="campoProvincia">Elige tu provincia:</label>
	<select name="campoProvincia" id="campoProvincia">
		<option value="01">Araba/Álava</option>
		<option value="48">Bizkaia</option>
		<option value="20">Gipuzkoa</option>
	</select>
</p>
Elige tu provincia: 
Araba/Álava

##### Selección multiple
buscar info qeu falta este apartado. por regla general no se usa por complicación a al ahora de usarlo

##### Selección categorizada
Si tenemos un listado de opciones que queremos categorizar, podemos hacerlo de la siguiente manera:


<p>
	<label for="campoProducto">Seleccione un producto:</label>
	<select name="campoProducto" id="campoProducto">
		<optgroup label="software">
			<option value="1">Ubuntu</option>
			<option value="2">Gimp</option>
			<option value="3">Open Office</option>
		</optgroup>
			<optgroup label="hardware">
			<option value="4">Grabador DVD</option>
			<option value="5">Tarjeta Gráfica</option>
		</optgroup>
		<optgroup label="material">
			<option value="7">Torre 10 CDs</option>
			<option value="8">Alfombrilla</option>
			<option value="9">WebCam</option>
		</optgroup>
	</select>
</p>
Seleccione un producto: 
Ubuntu

Técnicamente es posible dar la opción de seleccionar varias opciones a la vez, pero requiere de una combinación de teclado y ratón, por lo que no se puede utilizar en muchos dispositivos, ni tampoco por personas que no dispongan los dos métodos de entrada.

##### Valor vacío inicialmente
+ la primera opción de este elemento aparece de forma visible y seleccionada. Si no queremos que aparezca nada como seleccionado, tenemos la opción de crear una primera opción vacía. Pero esto hace que el usuario pueda seleccionar esa opción que, en realidad, no es una opción.

Para evitar todos estos problemas, basta con añadir unos atributos adicionales a la no-opción problemática:

```html
	<p>
		<label for="campoProvincia">Elige tu provincia:</label>
		<select name="campoProvincia" id="campoProvincia">
			<option value="" disabled hidden selected></option>
			<option value="01">Araba/Álava</option>
			<option value="48">Bizkaia</option>
			<option value="20">Gipuzkoa</option>
		</select>
	</p>
```
	
Agregar categorías no seleccionables
```html
 <optgroup label="categoría">
```

se puede hacer el icono que esta en el desplegable, con cuidado porque hay iconos que ya tiene un valor sugerido