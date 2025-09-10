# Programación web en entorno cliente
## HTML

### 8. Guía de Listas en HTML
Una lista en HTML permite organizar información en elementos agrupados, facilitando la lectura y la estructura del contenido. Usar listas mejora la semántica y la accesibilidad de las páginas web, por lo que es una buena práctica emplearlas siempre que se presenten conjuntos de elementos relacionados.

#### Tipos de listas

- **Listas desordenadas** (`<ul>`): Elementos sin orden específico, con viñetas.
- **Listas ordenadas** (`<ol>`): Elementos con orden, numerados automáticamente.
- **Listas de definición** (`<dl>`): Pares de término y definición.



#### 1. Etiquetas principales y ejemplos

**Lista desordenada (`<ul>`)**
```html
<ul>
	<li>Elemento 1</li>
	<li>Elemento 2</li>
</ul>
```
Ejemplo práctico:
```html
<h2>Ingredientes</h2>
<ul>
	<li>8 tomates rojos</li>
	<li>2 pepinos pequeños</li>
	<li>1 rebanada de pan</li>
	<li>2 dientes de ajo</li>
	<li>2 pimientos</li>
	<li>cuarto litro de aceite</li>
	<li>vinagre</li>
	<li>sal</li>
	<li>agua</li>
</ul>
```

**Lista ordenada (`<ol>`)**
```html
<ol>
	<li>Paso 1</li>
	<li>Paso 2</li>
</ol>
```
Ejemplo práctico:
```html
<h2>Preparación</h2>
<ol>
	<li>Triturar en la batidora los pimientos y los tomates partidos por la mitad, los pepinos pelados, los ajos, el pan, y el aceite, con un chorrito de vinagre, un poco de agua y sal.</li>
	<li>Batir muy bien</li>
	<li>Verter todo en la fuente en la que vaya a ser servido y agregar agua hasta que adquiera la consistencia de una crema ligera.</li>
	<li>Servir muy frío.</li>
</ol>
```

**Elemento de lista (`<li>`)**
```html
<ul>
	<li>Elemento A</li>
	<li>Elemento B</li>
</ul>
```

**Lista de definición (`<dl>`, `<dt>`, `<dd>`)**
```html
<dl>
	<dt>Término</dt>
	<dd>Definición</dd>
</dl>
```
Ejemplo práctico:
```html
<h2>Ficha técnica</h2>
<dl>
	<dt>Nombre:</dt>
	<dd>Open open</dd>
	<dt>Versión:</dt>
	<dd>2.0</dd>
	<dt>Plataformas:</dt>
	<dd>Linux</dd>
	<dd>Mac</dd>
	<dd>Windows</dd>
</dl>
```


---

#### 2. Contenido permitido en `<li>`

Dentro de `<li>` puedes incluir texto, enlaces, imágenes, listas anidadas y cualquier otro elemento HTML válido.

```html
<ul>
	<li>Texto simple</li>
	<li><a href="#">Enlace</a></li>
	<li><img src="logo.png" alt="Logo"></li>
	<li>
		<a href="#"><img src="icono.png" alt="Icono"> Enlace con imagen</a>
	</li>
	<li>Con <strong>formato</strong> y <a href="#">enlace contextual</a></li>
</ul>
```


---

#### 3. Listas anidadas

Puedes anidar listas para crear jerarquías. **Una lista (`<ul>` o `<ol>`) solo puede estar dentro de un `<li>`, nunca directamente dentro de `<ul>` o `<ol>`.**

**Ejemplo correcto:**
```html
<ul>
	<li>
		Trilogía de El señor de los anillos
		<ol>
			<li>La comunidad del anillo</li>
			<li>Las dos torres</li>
			<li>El retorno del rey</li>
		</ol>
	</li>
	<li>El Silmarillión</li>
	<li>El Hobbit</li>
</ul>
```

**Ejemplo incorrecto:**
```html
<ul>
	<li>Trilogía de El señor de los anillos</li>
<ol>
	<li>La comunidad del anillo</li>
	<li>Las dos torres</li>
	<li>El retorno del rey</li>
</ol>
	<li>El Silmarillión</li>
	<li>El Hobbit</li>
</ul>
```


---



#### 4. Listas de definición avanzadas

Las listas de definición (`<dl>`) se utilizan para mostrar pares de términos y sus definiciones. Dentro de una lista de definición:

- `<dl>` es el contenedor principal de la lista.
- `<dt>` (Definition Term) define el término o concepto.
- `<dd>` (Definition Description) proporciona la descripción o definición del término anterior.

Puedes tener varios `<dt>` y `<dd>` dentro de un mismo `<dl>`, e incluso varios `<dd>` para un solo `<dt>`, lo que permite asociar múltiples definiciones a un mismo término.

**Ejemplo básico:**
```html
<dl>
	<dt>HTML</dt>
	<dd>Lenguaje de marcado para la web</dd>
	<dt>CSS</dt>
	<dd>Lenguaje de estilos para la web</dd>
</dl>
```

**Ejemplo con varios `<dd>` para un `<dt>`:**
```html
<dl>
	<dt>API</dt>
	<dd>Interfaz de programación de aplicaciones.</dd>
	<dd>Conjunto de funciones y procedimientos para acceder a servicios.</dd>
</dl>
<dl>
	<dt>Plataformas</dt>
	<dd>Linux</dd>
	<dd>Mac</dd>
	<dd>Windows</dd>
</dl>
```



---

#### 5. Personalización visual y sangría

Puedes cambiar el tipo de viñeta o numeración de las listas mediante CSS. Los navegadores aplican sangría por defecto:

```css
ul, ol { margin-left: 2em; padding-left: 40px; }
ul, ol { margin-left: 0; padding-left: 0; } /* Para eliminar sangría */
```

Recomendación: Ajusta solo si el diseño lo requiere, pero mantén la semántica.


---

#### 6. Mejores prácticas

- Usa el tipo de lista adecuado según el contenido.
- Las sublistas siempre dentro de `<li>`.
- Personaliza solo con CSS, no cambies la semántica.
- No uses listas solo para sangrar texto o maquetar.
- Mantén la accesibilidad y la estructura clara.


---

#### 7. Documentación oficial

- [Listas en HTML Living Standard (WHATWG)](https://html.spec.whatwg.org/multipage/grouping-content.html#the-ul-element)
- [MDN Web Docs: Listas HTML](https://developer.mozilla.org/es/docs/Web/HTML/Element/ul)


---


<!-- Los ejemplos prácticos ahora están integrados tras cada explicación -->

---

#### 9. Personalización de viñetas y numeración con CSS

Puedes cambiar el tipo de viñeta de las listas desordenadas (`<ul>`) y el tipo de numeración de las listas ordenadas (`<ol>`) usando la propiedad CSS `list-style-type`.

Consulta la documentación de CSS para más opciones: [MDN list-style-type](https://developer.mozilla.org/es/docs/Web/CSS/list-style-type)

Por defecto, los navegadores aplican una sangría (indentación) a las listas (`<ul>`, `<ol>`, `<dl>`) para diferenciarlas del resto del contenido. Esta sangría puede variar según el navegador y el sistema operativo.

**Controlar la sangría con CSS:**

Puedes modificar o eliminar la sangría de las listas usando las propiedades CSS `margin` y `padding`.

**Recomendación:** Ajusta la sangría solo si el diseño lo requiere, pero mantén la estructura semántica de la lista. No uses listas únicamente para crear sangrías visuales; utiliza listas solo cuando el contenido lo justifique.
