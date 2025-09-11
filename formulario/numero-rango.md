# Programación web en entorno cliente
## HTML
### Número
Es un campo que sólo permite la inserción de números. Se puede indicar un número máximo `max` y mínimo `min`, así como el incremento/decremento entre pasos `step`:
`step` puede ser decimales, recordar que `html` usa punto para decimal, `0.5`


<p>
	<label for="campoEdad">Edad:</label>
	<input type="number" name="campoEdad" id="campoEdad" min="18" max="75" step="1">
<p>


Edad: 

### Rango
Es un campo numérico, pero el usuario no inserta el número, sino que lo elige orientativamente entre un rango:
indicar un número máximo `max` y mínimo `min`, así como el incremento/decremento entre pasos `step`



<p>
	<label for="campoVal">¿Puntuación de la película?:</label>
	<input type="range" name="campoVal" id="campoVal" min="0" max="100" step="10">
<p>

¿Puntuación de la película?: 


Si queremos que en este elemento también se vea el valor que se está eligiendo, tenemos que implementar la funcionalidad mediante Javascript:
[rango con numeros](https://codepen.io/antxoa/pen/OOLMMb)


