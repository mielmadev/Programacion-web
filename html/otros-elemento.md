# Programación web en entorno cliente
## HTML


### Otros elementos HTML

Dentro de la especificación HTML existen más elementos para proporcionar valor semántico al contenido. A continuación se describen algunos de los más relevantes:

---


#### Iframe

El elemento `<iframe>` se utiliza para insertar contenido de otra página web dentro de una página existente, por ejemplo, un video de YouTube, un mapa de Google Maps.

Por lo general, no crearemos este elemento manualmente. Cuando vayamos a insertar este contenido, la página donde se encuentra ese contenido a insertar nos facilitará el código para copiar y pegar, que no podremos modificar.

El contenido dentro del iframe es completamente independiente del contenido de nuestra página, por lo que nuestros estilos CSS y funciones Javascript no se aplicarán al contenido dentro del iframe.

**Ejemplo de video de YouTube:**
```html
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/pxUSYa3u7rs?si=mC4gi8Z2YPkzV2Ad" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
```

**Ejemplo de mapa de Google Maps:**
```html
<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d10902.285379700763!2d-2.9266834000090793!3d43.371624242320614!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xd4e4361a5f31b31%3A0x96d1894e7b4b6d9!2sCastillo%20de%20Butr%C3%B3n%2C%20Bo.%20Butron%2C%2012%2C%2048110%20Gatica%2C%20Vizcaya!5e0!3m2!1ses!2ses!4v1710369254055!5m2!1ses!2ses" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
```

---


#### Dirección (`address`)

El elemento `<address>` se utiliza para marcar la información de contacto del autor/responsable de la página (dirección postal, teléfono, e-mail...). Solo debe incluir esta información específica. Generalmente se utiliza en el pie de página.

```html
<address>
	<p>Empresa ACME<br>
	C/ Gran Vía nº 1<br>
	48000 Bilbao (Vizcaya)<br>
	Teléfono: 94 444 444 444
	</p>
</address>
```

No debe utilizarse para representar direcciones arbitrarias (por ejemplo, en un directorio de empresas, solo en el pie de página).

---


#### Superíndice y Subíndice (`sup`, `sub`)

El elemento `<sup>` se aplica a un texto que se tiene que mostrar como superíndice (más alto y más pequeño que el texto principal, como en notaciones científicas o matemáticas).

El elemento `<sub>` se aplica a un texto que se tiene que mostrar como subíndice (más bajo y pequeño).

```html
<p>La parcela mide 20m<sup>2</sup></p>
<p>La fórmula química del agua es: H<sub>2</sub>O</p>
```
Superíndice: 2<sup>3</sup>

Subíndice: H<sub>2</sub>O

Estas etiquetas no deben usarse solo para lograr un efecto visual, para eso se debe usar CSS.

---


#### Elemento `b` mejor usar `strong`

El elemento `<b>` representa un fragmento de texto que se resalta por ser importante en relación al contenido: palabras clave, nombres de productos, etc.

```html
<h2>Opiniones sobre Caracoles Lentos</h2>
<p>
	Los <b class="nom-product">Caracoles Lentos</b>
	son un nuevo producto de la empresa alimenticia....
</p>
```
Los **Caracoles Lentos** son un nuevo producto de la empresa alimenticia....

---


#### Elemento `i` mejor usar `em`

El elemento `<i>` representa un fragmento de texto en voz alternativa o contenido que se presenta en cursiva: palabras en otro idioma (usando `lang`), términos técnicos, notación musical, pensamientos, etc.

Es recomendable utilizar clases (`class`) para indicar el significado que se le quiere dar al elemento `i` en cada caso.

```html
<p>
	Los <i lang="ca">escargots</i>, o caracoles,
	son de la familia de los <i class="taxonomy">Helix aspersa</i>.
</p>
```
Los *escargots*, o caracoles, son de la familia de los *Helix aspersa*.

---


#### Tecla (`kbd`)

El elemento `<kbd>` se utiliza para indicar que el texto mostrado pertenece a una tecla o combinación de teclas que debemos introducir con el teclado.

```html
<p>Pulsa <kbd>F5</kbd> para refrescar la página.</p>
```
---


#### Insertado y borrado (`ins`, `del`)

A veces, cuando modificamos un dato de una página web (por ejemplo, una fecha o precio), nos interesa dejar constancia de esa modificación. Para ello se usan los elementos `<ins>` (insertado) y `<del>` (borrado).

```html
<p>El sorteo se realizará el 2 de abril a las <del>11</del> <ins>12</ins> de la mañana.</p>
```
~~tachado del~~ <ins>agregado ins</ins>

#### Preformateo y código (`pre`, `code`)

El elemento `<pre>` representa texto preformateado, es decir, se respetan los espacios, saltos de línea y tabulaciones tal y como están escritos.

```html
<pre>
	function saludar() {
		console.log('¡Hola, clase!');
	}
</pre>
```
visual:

	function saludar() {
		console.log('¡Hola, clase!');
	}


El elemento `<code>` sirve para indicar que el texto pertenece a un código informático y normalmente se usa junto con `<pre>`.

```html
<code>
	class HelloWorld {
		public static void main(String[] args) {
			System.out.println("Hello World!");
		}
	}
</code>
```
visual:
```
	class HelloWorld {
		public static void main(String[] args) {
			System.out.println("Hello World!");
		}
	}
```

---


#### Orden de tabulador (`tabindex`)

El atributo `tabindex` permite modificar el orden de navegación mediante el tabulador. El valor de este atributo será numérico, indicando el orden en caso de haber más de uno. Si la información de la página está bien estructurada, rara vez se necesita este atributo.

**Ejemplo de mal uso de tabindex:**

```html
<table>
	<tr>
		<td>Nombre:<br /><input type="text" name="nom" tabindex="1" /></td>
		<td>Población:<br /><input type="text" name="pob" tabindex="4" /></td>
	</tr>
	<tr>
		<td>Apellidos:<br /><input type="text" name="apel" tabindex="2" /></td>
		<td>CP:<br /><input type="text" name="cp" tabindex="5" /></td>
	</tr>
	<tr>
		<td>Dirección:<br /><input type="text" name="dir" tabindex="3" /></td>
		<td>Teléfono:<br /><input type="text" name="tfn" tabindex="6" /></td>
	</tr>
</table>
```

> Nota: este código de formulario es incorrecto en muchos sentidos (semántico, accesible) y solo se utiliza para ilustrar un mal uso del atributo tabindex.

---


#### Acceso directo (`accesskey`)

El atributo `accesskey` permite implementar atajos de teclado para los enlaces más utilizados en nuestra web (como los atajos de teclado en un programa software).

```html
<a href="index.html" accesskey="1">Página de inicio</a>
```

La combinación de teclas varía según el navegador y sistema operativo:

| Navegador/SO | Windows             | Linux                 | Mac                      |
| ------------ | ------------------- | --------------------- | ------------------------ |
| Firefox      | Alt + Shift + tecla | Control + Alt + tecla | Control + Option + tecla |
| MS Edge      | Alt + tecla         | Control + Alt + tecla | Control + Option + tecla |
| Chrome       | Alt + tecla         | Control + Alt + tecla | Control + Option + tecla |
| Safari       | n/a                 | n/a                   | Control + Option + tecla |
| Opera        | Alt + tecla         | Control + Alt + tecla | Control + Alt + tecla    |

Se recomienda utilizar solo números para evitar interferencias con letras reservadas y usar el número "1" para la página de inicio.

> Chrome suele ignorar estos accesos directos.

#### Ejemplo interactivo

Puedes ver un ejemplo interactivo en CodePen:

[https://codepen.io/antxoa/pen/zYXKGWz](https://codepen.io/antxoa/pen/zYXKGWz)

