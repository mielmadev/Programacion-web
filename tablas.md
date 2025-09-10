
# Programación web en entorno cliente
## HTML

### 9. Guía de tablas en HTML

Las tablas en HTML sirven para presentar información tabulada, como calendarios, resultados, listados o resúmenes. Es importante usarlas solo para datos tabulares, no para maquetar el diseño de la web.



- `<thead>`: Cabecera de la tabla.
- `<tbody>`: Cuerpo de la tabla.
- `<tfoot>`: Pie de la tabla (opcional).
- `<tr>`: Fila de la tabla.
- `<th>`: Celda de cabecera.
- `<td>`: Celda de datos.


| Nombre        | Departamento | Extensión |
| ------------- | ------------ | --------- |
| Michael Scott | Gerencia     | 233       |
| ...           | ...          | ...       |

> **¿Cuándo usar `<caption>`?**
>
> - Siempre que la tabla sea relevante o necesite un título descriptivo.
> - Si quieres que el resumen de la página incluya esa tabla.
> - Por regla general, debe haber un párrafo explicativo antes de la tabla para dar contexto adicional, especialmente si la tabla es compleja o su propósito no es evidente solo con el título.

**Ejemplo de uso de `<caption>` y párrafo explicativo:**


```html
<p>La siguiente tabla muestra el personal y su extensión telefónica en la oficina:</p>
<table>
	<caption>Personal de Dunder Mifflin</caption>
	<thead>
		<tr>
			<th>Nombre</th>
			<th>Departamento</th>
			<th>Extensión</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Michael Scott</td>
			<td>Gerencia</td>
			<td>233</td>
		</tr>
		<!-- ... -->
	</tbody>
</table>
```

| Nombre        | Departamento | Extensión |
| ------------- | ------------ | --------- |
| Michael Scott | Gerencia     | 233       |



## 2. Ejemplo básico y visualización


# Programación web en entorno cliente
## HTML

## Guía de tablas en HTML

### 1. Introducción

Las tablas en HTML sirven para presentar información tabulada, como calendarios, resultados, listados o resúmenes. Es importante usarlas solo para datos tabulares, no para maquetar el diseño de la web.

### 2. Estructura básica de una tabla

- `<table>`: Define la tabla.
- `<thead>`: Cabecera de la tabla.
- `<tbody>`: Cuerpo de la tabla.
- `<tfoot>`: Pie de la tabla (opcional).
- `<tr>`: Fila de la tabla.
- `<th>`: Celda de cabecera.
- `<td>`: Celda de datos.

**Ejemplo básico:**

```html
<table>
	<caption>Personal de Dunder Mifflin</caption>
	<thead>
		<tr>
			<th>Nombre</th>
			<th>Departamento</th>
			<th>Extensión</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Michael Scott</td>
			<td>Gerencia</td>
			<td>233</td>
		</tr>
		<tr>
			<td>Dwight Schrute</td>
			<td>Ventas</td>
			<td>255</td>
		</tr>
		<tr>
			<td>Jim Halpert</td>
			<td>Ventas</td>
			<td>256</td>
		</tr>
		<tr>
			<td>Pam Beesly</td>
			<td>Atención al cliente</td>
			<td>211</td>
		</tr>
	</tbody>
</table>
```

### 3. Elementos principales: `<thead>`, `<tbody>`, `<tfoot>`

Estructura recomendada para tablas grandes o complejas:

```html
<table>
	<thead>
		<tr>
			<th>Cabecera 1</th>
			<th>Cabecera 2</th>
			<th>Cabecera 3</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Columna 1</td>
			<td>Columna 2</td>
			<td>Columna 3</td>
		</tr>
		<tr>
			<td>Columna 1</td>
			<td>Columna 2</td>
			<td>Columna 3</td>
		</tr>
	</tbody>
	<tfoot>
		<tr>
			<td colspan="3">Total o resumen</td>
		</tr>
	</tfoot>
</table>
```

### 4. Accesibilidad y descripción de tablas

Describir correctamente una tabla es fundamental para la accesibilidad y la comprensión del contenido, especialmente para personas que utilizan lectores de pantalla.

- Usa `<caption>` para describir la tabla.
- Usa `<th>` para celdas de cabecera y añade el atributo `scope` (`col` o `row`).
- Si la tabla es compleja, usa `id` en `<th>` y el atributo `headers` en `<td>` para asociar celdas de datos con sus cabeceras.
- Utiliza atributos de accesibilidad como `aria-describedby` para asociar la tabla con una descripción más extensa si es necesario.
- Evita el uso del atributo `summary`, ya que está obsoleto.

**¿Cuándo usar `<caption>`?**
- Siempre que la tabla sea relevante o necesite un título descriptivo.
- Si quieres que el resumen de la página incluya esa tabla.
- Por regla general, debe haber un párrafo explicativo antes de la tabla para dar contexto adicional, especialmente si la tabla es compleja o su propósito no es evidente solo con el título.

**Ejemplo de uso de `<caption>` y párrafo explicativo:**

```html
<p>La siguiente tabla muestra el personal y su extensión telefónica en la oficina:</p>
<table>
	<caption>Personal de Dunder Mifflin</caption>
	<thead>
		<tr>
			<th>Nombre</th>
			<th>Departamento</th>
			<th>Extensión</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Michael Scott</td>
			<td>Gerencia</td>
			<td>233</td>
		</tr>
		<!-- ... -->
	</tbody>
</table>
```

**Ejemplo de tabla con descripción accesible:**
```html
<p id="desc-ventas">Esta tabla muestra el resumen de ventas por departamento en 2025.</p>
<table aria-describedby="desc-ventas">
	<caption>Ventas por departamento</caption>
	<tr><th>Departamento</th><th>Ventas</th></tr>
	<tr><td>Electrónica</td><td>1200</td></tr>
	<tr><td>Ropa</td><td>950</td></tr>
</table>
```

#### El atributo `scope` en `<th>`

El atributo `scope` mejora la accesibilidad de las tablas, indicando a los lectores de pantalla si una celda de cabecera (`<th>`) se aplica a una columna (`scope="col"`), a una fila (`scope="row"`), a un grupo de columnas (`scope="colgroup"`) o a un grupo de filas (`scope="rowgroup"`).

**Valores más comunes:**
- `scope="col"`: la cabecera aplica a toda la columna.
- `scope="row"`: la cabecera aplica a toda la fila.

**Ejemplo:**
```html
<table>
	<caption>Ejemplo con scope</caption>
	<thead>
		<tr>
			<th scope="col">Nombre</th>
			<th scope="col">Departamento</th>
			<th scope="col">Extensión</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<th scope="row">Michael Scott</th>
			<td>Gerencia</td>
			<td>233</td>
		</tr>
		<tr>
			<th scope="row">Dwight Schrute</th>
			<td>Ventas</td>
			<td>255</td>
		</tr>
	</tbody>
</table>
```
Esto ayuda a que los usuarios de tecnologías de asistencia comprendan mejor la relación entre los encabezados y los datos de la tabla.

> El atributo `summary` está obsoleto. Si necesitas un resumen, usa `<caption>` o un texto alternativo fuera de la tabla.

### 5. Fusión de celdas y filas (`colspan`, `rowspan`)

A veces una celda debe ocupar varias columnas o filas. Para ello se usan los atributos:

- **`colspan`**: Permite que una celda ocupe el espacio de varias columnas. Se usa cuando quieres que una celda se extienda horizontalmente.
- **`rowspan`**: Permite que una celda ocupe el espacio de varias filas. Se usa cuando quieres que una celda se extienda verticalmente.

Ambos atributos pueden aplicarse tanto a `<td>` como a `<th>`.

**Ejemplo:**
```html
<table>
	<caption>Novedades en el Videoclub</caption>
	<tr>
		<th>Título</th>
		<th colspan="2">Géneros</th>
	</tr>
	<tr>
		<td>Sin City</td>
		<td>Acción</td>
		<td>Comic</td>
	</tr>
	<tr>
		<td>Charlie y la fábrica de chocolate</td>
		<td>Infantil</td>
		<td>Musical</td>
	</tr>
	<tr>
		<td>La madre del novio</td>
		<td rowspan="2">Comedia</td>
		<td rowspan="2">Romántica</td>
	</tr>
	<tr>
		<td>Embrujada</td>
	</tr>
</table>
```

### 6. Tablas anidadas

Es posible insertar una tabla dentro de una celda de otra tabla en HTML. Esto se llama tabla anidada. Sin embargo, solo debe hacerse cuando la estructura de los datos realmente lo requiera, ya que puede dificultar la accesibilidad y el mantenimiento del código.

**Buenas prácticas:**
- Usa tablas anidadas solo si no hay otra forma clara de representar la información.
- Mantén la estructura lo más simple posible.
- Añade comentarios en el código para facilitar la comprensión.
- Considera alternativas como dividir la información en varias tablas independientes si es posible.

**Ejemplo de tabla anidada:**
```html
<table border="1">
	<caption>Tabla principal</caption>
	<tr>
		<th>Nombre</th>
		<th>Detalles</th>
	</tr>
	<tr>
		<td>Producto 1</td>
		<td>
			<table border="1">
				<caption>Características</caption>
				<tr><th>Peso</th><th>Color</th></tr>
				<tr><td>2kg</td><td>Rojo</td></tr>
			</table>
		</td>
	</tr>
</table>
```

### 7. Buenas prácticas

- Usa tablas solo para datos tabulares, no para maquetar el diseño.
- Usa `<thead>`, `<tbody>` y `<tfoot>` para estructurar tablas grandes.
- Añade atributos de accesibilidad en tablas complejas.

### 8. Generadores automáticos de tablas HTML

En ocasiones, para ahorrar tiempo o evitar errores de sintaxis, puedes utilizar generadores automáticos de tablas HTML. Estas herramientas permiten crear tablas visualmente y obtener el código listo para copiar y pegar en tu proyecto.

**¿Cuándo usarlos?**
- Cuando necesitas crear tablas grandes o complejas rápidamente.
- Para prototipos, ejemplos o documentación.
- Si no dominas la sintaxis de tablas HTML y quieres aprender visualmente.

**Algunas herramientas recomendadas:**
- [Accessify Table Builder (accesibilidad)](https://www.accessify.com/tools-and-wizards/accessibility-tools/table-builder/)

Recuerda revisar y adaptar el código generado para cumplir con las buenas prácticas de accesibilidad y semántica.

### 9. Recursos y documentación

- [Tablas en HTML Living Standard (WHATWG)](https://html.spec.whatwg.org/multipage/tables.html)
- [MDN Web Docs: Tablas HTML](https://developer.mozilla.org/es/docs/Web/HTML/Element/table)


**Algunas herramientas recomendadas:**

