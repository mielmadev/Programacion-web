# Programación web en entorno cliente

## Intro

### Sistemas Operativos

#### Mostrar extensiones de archivo y archivos ocultos

Para trabajar correctamente en programación web, es importante poder ver las extensiones de los archivos y los archivos ocultos en tu sistema operativo. A continuación, se detallan los pasos recomendados para cada sistema:

---

#### Windows

**Mostrar extensiones de archivo:**
1. Abre el **Explorador de archivos** (tecla Windows + E o desde la barra de tareas).
2. Haz clic en la pestaña **Vista** en la parte superior.
3. En el grupo **Mostrar u ocultar**, marca la casilla **Extensiones de nombre de archivo**.
	- Si no está marcada, haz clic para activarla.
4. Ahora verás las extensiones junto a los nombres de archivo.

**Mostrar archivos ocultos:**
1. En la misma pestaña **Vista**, marca la casilla **Elementos ocultos**.
2. Los archivos y carpetas ocultos serán visibles en el explorador.

> **Nota:** Estas opciones ayudan a evitar errores al trabajar con archivos de código y configuración.

---

#### Linux (Ubuntu)

**Extensiones visibles:**
- En Ubuntu, las extensiones de archivo suelen ser visibles por defecto.

**Mostrar archivos ocultos:**
1. Abre el **administrador de archivos** (Nautilus).
2. Haz clic en el menú **Ver**.
3. Activa la opción **Ver archivos ocultos**.
	- Alternativamente, puedes presionar `Ctrl + H` para mostrar/ocultar archivos ocultos rápidamente.

---


#### Mac OS

**Mostrar extensiones de archivo:**
- Consulta la documentación oficial de Apple: [Mostrar extensiones](https://support.apple.com/es-es/guide/mac-help/mchlp1031/mac)
- También puedes seguir esta guía específica: [Cómo mostrar u ocultar extensiones de archivos en Mac](https://support.apple.com/es-es/guide/mac-help/mchlp2304/mac)



> **Recomendación:** Mantén siempre visibles las extensiones y archivos ocultos durante el desarrollo web para evitar confusiones y facilitar la gestión de archivos de configuración.

### Editores de Código

Para trabajar en programación web es fundamental utilizar un editor de código fuente adecuado. Existen muchas opciones y la mejor será aquella con la que te sientas más cómodo y productivo, ya que pasarás muchas horas utilizándola.

#### Recomendaciones generales
- Elige un editor que se adapte a tus necesidades y preferencias personales.
- Considera la facilidad de uso, la personalización, la disponibilidad de extensiones y la compatibilidad con tu sistema operativo.
- En entornos profesionales, puede que se requiera un editor específico, pero lo importante es saber programar, no dominar un programa concreto.

#### Editores recomendados

- **Notepad++**: Interfaz sencilla y amigable, ideal para principiantes.
- **Sublime Text**: Muy popular entre diseñadores. Dispone de versión gratuita y de pago.
- **Visual Studio Code**: Uno de los más utilizados actualmente, muy completo y con gran cantidad de extensiones.

> Cualquier editor que permita trabajar con texto plano es válido, incluso el Bloc de notas, aunque se recomienda usar uno especializado para mejorar la productividad.

#### Otros aspectos importantes

##### Modo oscuro
El modo oscuro es recomendable por varias razones:
- **Reducción de la fatiga visual:** Utiliza colores oscuros de fondo y claros para el texto, lo que ayuda a reducir el cansancio ocular, especialmente en sesiones largas o en ambientes con poca luz.
- **Mejor legibilidad:** El contraste entre texto claro y fondo oscuro puede facilitar la lectura del código.
- **Menor consumo de energía:** En pantallas OLED/AMOLED, el modo oscuro puede ahorrar batería.
- **Personalización:** Permite adaptar la interfaz a tus preferencias y crear un entorno cómodo.

> La preferencia por el modo oscuro es subjetiva. Usa la configuración que mejor se adapte a tus necesidades.

##### Tipografías
Utiliza una tipografía monoespaciada y clara para mejorar la legibilidad del código. Es importante que caracteres similares (como I, l, 1, 0, O) se distingan fácilmente.

Algunas sugerencias:
- **Dejavu Sans Mono**
- **JetBrains Mono**

Puedes explorar y comparar diferentes tipografías para programar en: [programmingfonts.org](https://www.programmingfonts.org/)

> Evita tipografías donde caracteres como la i mayúscula (I) y la ele minúscula (l) sean idénticos, ya que dificulta la lectura y comprensión del código.

### Navegadores

Para navegar por internet como usuario, se puede utilizar cualquier navegador moderno. Sin embargo, para el desarrollo web es recomendable limitarse a dos navegadores principales debido a las funcionalidades y soporte que ofrecen para pruebas y depuración:

#### Navegadores recomendados para desarrollo

- **Mozilla Firefox**
- **Google Chrome**

Otros navegadores como Edge, Safari, Opera, Vivaldi, Brave, etc., pueden ser útiles en ciertos contextos, pero no siempre permiten realizar todas las pruebas y depuración de la forma más eficiente.

> Los dos navegadores recomendados, junto con extensiones específicas, permiten un desarrollo y depuración más ágil y preciso.

#### Buenas prácticas
- Mantén ambos navegadores actualizados para asegurar compatibilidad y seguridad.
- Utiliza las herramientas de desarrollo integradas (DevTools) para inspeccionar, depurar y optimizar tu código.
- Realiza pruebas cruzadas en ambos navegadores para garantizar el correcto funcionamiento de tus aplicaciones web.

> Aunque Chrome y Firefox cubren la mayoría de necesidades, es recomendable probar en otros navegadores antes de publicar un proyecto para asegurar la máxima compatibilidad.
### Extensiones, complementos y add-ons

Para mejorar las prestaciones de los navegadores durante el desarrollo web, es recomendable instalar algunas extensiones específicas. Estas herramientas facilitan tareas de inspección, depuración y diseño.

- **Web Developer**: Extensión para navegadores que añade una barra de herramientas con utilidades para inspeccionar, depurar y modificar páginas web en tiempo real. Permite deshabilitar scripts, ver estructuras de HTML y CSS, validar código, analizar imágenes y mucho más. Es ideal para mejorar la productividad y la calidad del desarrollo front-end. [Chrome Web Store](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm?hl=es)
- **ColorZilla**: Permite obtener colores de cualquier parte de la página y gestionar paletas de colores ([Chrome Web Store](https://chrome.google.com/webstore/detail/colorzilla/bhlhnicpbhignbdhedgjhgdocnmhomnp)).

#### Herramientas propias de los navegadores
Además de las extensiones, los navegadores incluyen herramientas integradas muy útiles:
- **Vista de código fuente**: `Ctrl + U` (permite ver el HTML generado de la página).
- **Consola de desarrollo**: `Ctrl + Shift + I` (abre las DevTools para inspeccionar, depurar y modificar el código en tiempo real).

> Mantén tus extensiones actualizadas y revisa los permisos que solicitan para garantizar la seguridad y el buen funcionamiento del navegador.

### Servicios Web

Para probar ejemplos, realizar ejercicios y compartir proyectos de desarrollo web de manera sencilla, existen servicios web gratuitos como **CodePen**.

#### ¿Qué es CodePen?
CodePen es una plataforma online que permite crear, compartir y colaborar en proyectos de desarrollo web. Ofrece herramientas para escribir código HTML, CSS y JavaScript en tiempo real, mostrando los resultados de inmediato en una vista previa en vivo.

#### Características principales
- **Editor de código en tiempo real:** Permite escribir y editar HTML, CSS y JavaScript, mostrando los resultados instantáneamente.
- **Preprocesadores y bibliotecas:** Soporta preprocesadores como Sass y Less, y bibliotecas populares como Bootstrap, jQuery y React.
- **Vista previa en vivo:** Los cambios en el código se reflejan al instante en la vista previa.
- **Proyectos colaborativos:** Permite compartir proyectos públicos y colaborar con otros desarrolladores.
- **Comunidad activa:** Cuenta con una comunidad de desarrolladores y diseñadores que comparten recursos, ideas y proyectos.

> Para utilizar CodePen es necesario crear una cuenta gratuita en [codepen.io](https://codepen.io/). Existen planes de pago con funcionalidades avanzadas, pero la versión gratuita es suficiente para la mayoría de prácticas y pruebas.


## HTML

### Introducción a HTML

**HTML** (HyperText Markup Language) es el lenguaje de marcado estándar para la creación de páginas web. Permite estructurar el contenido mediante el uso de etiquetas, definiendo la jerarquía y el significado de cada elemento en la página.

> **Nota:** HTML no es un lenguaje de programación, sino un lenguaje de marcado utilizado para definir la estructura y el contenido de los documentos web.

#### Estándares y organización

HTML es gestionado y estandarizado por el **World Wide Web Consortium (W3C)**, organismo encargado de definir las tecnologías fundamentales de la web. El cumplimiento de los estándares garantiza la compatibilidad y el correcto funcionamiento de las páginas en todos los navegadores modernos.

#### Historia y contexto

El desarrollo de HTML fue liderado por **Sir Tim Berners-Lee**, quien también creó el protocolo HTTP y el sistema de localización de recursos URL. Estas tecnologías sentaron las bases para la World Wide Web y su expansión global.

#### Filosofía de trabajo

- **HTML** se utiliza para definir la estructura y semántica del contenido.
- **CSS** se encarga de la presentación visual y el diseño.
- **JavaScript** añade interactividad y comportamiento dinámico.

Esta separación de responsabilidades facilita el mantenimiento, la accesibilidad y la escalabilidad de los proyectos web.

#### Referencias

- [World Wide Web Consortium (W3C)](https://www.w3.org/)
- [Especificación HTML Living Standard (WHATWG)](https://html.spec.whatwg.org/multipage/)
- [Tim Berners-Lee - W3C](https://www.w3.org/People/Berners-Lee/)


### Normas generales de HTML

#### Archivos y nombres

- El archivo principal de cada sitio web debe llamarse `index.html`.
- Utiliza la extensión `.html` (no `.htm`).
- Los nombres de archivos deben estar en minúsculas, sin tildes ni caracteres especiales (ejemplo: `á`, `ñ`, `ç`, etc.).
- No uses símbolos (¿? ¡! () {} [] ; : % & ...) ni espacios. Si necesitas separar palabras, utiliza guiones medios (`-`).

#### Estructura de elementos y etiquetas

El código HTML se compone de elementos representados por etiquetas. La mayoría de los elementos tienen una etiqueta de apertura y otra de cierre:

```html
<etiqueta>
	<!-- contenido -->
</etiqueta>
```

Algunas etiquetas son autoconclusivas (no requieren cierre). Puedes escribirlas de dos formas válidas:

```html
<etiquetaautocierre>
<etiquetaautocierre />
```

### Documentación oficial sobre encabezados y outlines en HTML

#### Enlaces oficiales

- [Elementos h1, h2, h3, h4, h5 y h6 (WHATWG HTML)](https://html.spec.whatwg.org/multipage/sections.html#the-h1,-h2,-h3,-h4,-h5,-and-h6-elements)
- [Encabezados y outlines (WHATWG HTML)](https://html.spec.whatwg.org/multipage/sections.html#headings-and-outlines-2)

#### Recomendaciones

**Recomendación:** Mantén coherencia en el estilo de autocierre que elijas para todo tu proyecto.

#### Ejemplo incorrecto de autocierre

No inventes etiquetas de cierre para etiquetas autoconclusivas.

```html
<!-- Esto es incorrecto -->
<etiquetaautocierre>
#### Semántica y variedad de etiquetas

HTML ofrece muchas etiquetas para describir el significado del contenido. Utiliza la etiqueta adecuada para cada tipo de información. La presentación visual se gestiona con CSS, no con HTML.

#### Comentarios en HTML
```html
<!-- Esto es un comentario -->
```

No es posible anidar comentarios en HTML. El cierre del primer comentario cerrará todos los comentarios abiertos.

#### Atributos

Las etiquetas pueden tener atributos para especificar características adicionales. Los atributos se colocan en la etiqueta de apertura y su valor va entre comillas:

```html
<etiqueta atributo="valor">
</etiqueta>
```

Puedes usar varios atributos separados por espacios, pero no repitas el mismo atributo en una etiqueta:

```html
<etiqueta atributo1="valor1" atributo2="valor2">
</etiqueta>

<!-- Incorrecto -->
<etiqueta atributo="valor1" atributo="valor2">
</etiqueta>
```


### Esquema básico de un documento HTML

Un documento HTML debe seguir una estructura estándar para garantizar compatibilidad, accesibilidad y correcto funcionamiento en todos los navegadores. A continuación se describe el esquema básico recomendado:

#### 1. Declaración del tipo de documento

La primera línea debe ser la declaración `<!DOCTYPE html>`, que indica al navegador que el documento sigue el estándar HTML5.

```html
<!DOCTYPE html>
```

#### 2. Elemento raíz `<html>` y atributo `lang`

El elemento principal es `<html>`, que engloba todo el contenido de la página. Es recomendable añadir el atributo `lang` para especificar el idioma principal del documento, usando el código ISO 639-1 (por ejemplo, `es` para español, `en` para inglés):

```html
<html lang="es">
	...
</html>
```

Puedes especificar también la región, por ejemplo `es-ES` para español de España o `en-US` para inglés de Estados Unidos.

#### 3. Estructura interna: `<head>` y `<body>`

El elemento `<html>` debe contener dos elementos hijos principales:

- `<head>`: Contiene metadatos y configuraciones técnicas (no visibles en la página).
- `<body>`: Contiene el contenido visible de la página.

```html
<!DOCTYPE html>
<html lang="es">
	<head>
		...
	</head>
	<body>
		...
	</body>
</html>
```

#### 4. Contenido mínimo recomendado en `<head>`

Incluye siempre la codificación de caracteres y el título de la página:

```html
<head>
	<meta charset="utf-8">
	<title>Mi primera página</title>
</head>
```

- `<meta charset="utf-8">` define la codificación de caracteres recomendada para la mayoría de idiomas.
- `<title>` define el texto que aparece en la pestaña del navegador y en los marcadores.

> **Nota:** La etiqueta `<meta charset="utf-8">` debe ir antes de `<title>` para evitar problemas con caracteres especiales.

#### 5. Ejemplo completo de documento HTML básico

```html
<!DOCTYPE html>
<html lang="es">
	<head>
		<meta charset="utf-8">
		<title>Mi primera página</title>
	</head>
	<body>
		<!-- Contenido visible de la página -->
	</body>
</html>
```

#### Buenas prácticas

- Utiliza siempre la declaración `<!DOCTYPE html>`.
- Especifica el idioma con el atributo `lang` en `<html>`.
- Incluye la codificación de caracteres y el título en `<head>`.
- No inventes etiquetas de cierre para etiquetas autoconclusivas como `<meta>`.
- Mantén la indentación y la estructura clara para facilitar la lectura y el mantenimiento.


### Validación de código HTML

Validar el código HTML es fundamental para asegurar que las páginas web cumplen con los estándares y funcionan correctamente en todos los navegadores. El uso de un validador ayuda a detectar errores de sintaxis, etiquetas mal cerradas o atributos incorrectos.

#### ¿Por qué validar?

Así como revisamos la ortografía en un documento de texto, debemos revisar la sintaxis y estructura de nuestro código HTML para evitar errores y mejorar la accesibilidad, compatibilidad y mantenimiento.

#### Herramienta recomendada

El **W3C Markup Validation Service** es la herramienta oficial y gratuita para validar documentos HTML:

- [Validador HTML del W3C](https://validator.w3.org/#validate_by_upload)

#### Formas de validar tu código

Puedes validar tu código HTML de tres maneras principales:

1. **Indicando la URL** de una página web pública.
2. **Subiendo el archivo HTML** desde tu equipo.
3. **Pegando el código fuente** directamente en el formulario del validador.

> **Recomendación:** Valida tu código frecuentemente, especialmente si algo no funciona como esperas o antes de publicar tu sitio web.


### Texto en HTML

HTML proporciona diferentes elementos para estructurar y dar significado al texto en una página web. Utiliza siempre elementos semánticos para mejorar la accesibilidad y el SEO.

#### Párrafos

El elemento `<p>` se utiliza para agrupar y separar párrafos de texto:

```html
<p>Este es un párrafo.</p>
<p>Este es otro párrafo.</p>
```

#### Saltos de línea

Para insertar un salto de línea dentro de un párrafo, utiliza el elemento autoconclusivo `<br>`:

```html
<p>
	Imagine there’s no heaven<br>
	It’s easy if you try
</p>
```

> **No uses varios `<br>` seguidos para simular separación entre párrafos. Utiliza siempre `<p>` para separar bloques de texto y CSS para controlar el espaciado.

#### Énfasis y relevancia

Para resaltar o enfatizar partes del texto, utiliza los elementos semánticos:

- `<strong>`: Indica importancia (por defecto, negrita).
- `<em>`: Indica énfasis (por defecto, cursiva).

```html
<p>
	<strong>Aviso:</strong> No olvide utilizar un <em>DNI válido</em>.
</p>
```

> **Evita usar `<b>` y `<i>` solo para dar formato visual. Prefiere `<strong>` y `<em>` por su significado semántico.

#### Citas

**Bloques de cita:**
Utiliza `<blockquote>` para citas textuales extensas. Puedes incluir varios párrafos dentro:

```html
<blockquote>
	<p>En un lugar de la Mancha, de cuyo nombre no quiero acordarme...</p>
	<p>Una olla de algo más vaca que carnero...</p>
</blockquote>
```

> No uses `<blockquote>` solo para obtener sangría visual.

**Citas en línea:**
Para citas cortas dentro de un texto, utiliza `<q>`. Para el autor, usa `<cite>`:

```html
<p>Como dijo <cite>Hamlet</cite>: <q>ser o no ser, esa es la cuestión</q>.</p>
```

#### Abreviaturas

El elemento `<abbr>` marca abreviaturas, siglas o acrónimos. Usa el atributo `title` para indicar el significado completo:

```html
<abbr title="Unión Europea">UE</abbr>
```

El atributo `title` puede usarse en la mayoría de elementos HTML para proporcionar información adicional. No lo confundas con la etiqueta `<title>` del `<head>`.


#### Recursos útiles

- [Generador de texto aleatorio (Lorem Ipsum)](https://es.lipsum.com/)
- [Choose your Ipsum (varios generadores)](https://idsgn.dropmark.com/107)
- [Ejemplo de cita: Wikipedia American Idol](https://es.wikipedia.org/wiki/American_Idol)

> Utiliza siempre elementos semánticos para mejorar la accesibilidad, el SEO y la mantenibilidad del código.


### Enlaces en HTML

Los enlaces (o hipervínculos) son fundamentales en la web, permitiendo la navegación entre páginas y recursos.

#### Estructura básica

El elemento `<a>` se utiliza para crear enlaces. El atributo `href` indica la ruta o URL de destino y el contenido entre las etiquetas es el texto visible del enlace:

```html
<a href="ruta">Texto del enlace</a>
```

Ejemplos de rutas:

- Mismo directorio: `<a href="mipagina.html">Página personal</a>`
- Subdirectorio: `<a href="personal/mipagina.html">Mi página</a>`
- Nivel superior: `<a href="../mipagina.html">Mi página</a>`
- Varias subidas/bajadas: `<a href="personal/io/mio/mipagina.html">Mi página</a>`

#### Enlaces externos

Para enlaces a sitios externos, utiliza URLs completas que comiencen con `http://` o `https://`:

```html
<a href="https://www.google.es">Google</a>
<a href="https://play.google.com/">Google Play</a>
```

> **Incorrecto:** No omitas el protocolo ni uses rutas incompletas.

```html
<!-- Incorrecto -->
<a href="google.es">Google</a>
<a href="www.google.es">Google</a>
<a href="http:www.google.es">Google</a>
```

#### Atributo `title` para enlaces

El atributo `title` proporciona información adicional sobre el destino del enlace. Úsalo solo si aporta valor real y no repite el texto del enlace:

```html
<a href="https://www.yahoo.com" title="Yahoo: noticias, e-mail, fotos, grupos, etc.">Yahoo</a>
```

> **No uses** el atributo `title` si su contenido es idéntico o muy similar al texto del enlace.

#### Enlaces internos (anclas)

Para enlazar a una sección dentro de la misma página, utiliza el atributo `id` en el destino y una almohadilla `#` en el enlace:

```html
<a href="#cancion2">Canción 2</a>
...
<p id="cancion2">Esta es la Canción 2</p>
```

Reglas para el atributo `id`:
- Debe ser único en la página.
- No debe empezar con un número.
- No debe contener espacios ni caracteres especiales.

También puedes enlazar a una sección específica de otra página:

```html
<a href="noticias.html#referencia1">Referencia</a>
```

#### Idioma de destino (`hreflang`)

Si el enlace apunta a una página en otro idioma, utiliza el atributo `hreflang` para especificarlo:

```html
<a href="https://www.nasa.gov" hreflang="en">NASA</a>
<a href="https://www.paris.fr" hreflang="fr">Ayuntamiento de París</a>
```

#### Abrir enlaces en nueva pestaña

El atributo `target="_blank"` abre el enlace en una nueva pestaña. Si lo usas, añade también `rel="noopener noreferrer"` para mejorar la seguridad:

```html
<a href="https://www.ejemplo.com" target="_blank" rel="noopener noreferrer">Sitio externo</a>
```

> **Nota:** El uso de `target="_blank"` debe ser justificado y no abusivo, ya que puede afectar la experiencia del usuario.

#### Buenas prácticas

- Usa rutas relativas para enlaces internos y URLs absolutas para externos.
- Utiliza atributos semánticos (`title`, `hreflang`) solo cuando aporten valor.
- Mantén los `id` únicos y descriptivos.
- No uses enlaces vacíos (`href="#"`) salvo para casos muy específicos y controlados por JavaScript.


### Imágenes en HTML

Las imágenes se insertan en HTML mediante el elemento autoconclusivo `<img>`. Es fundamental utilizar correctamente los atributos obligatorios para garantizar accesibilidad y compatibilidad.

#### Sintaxis básica

```html
<img src="ruta" alt="texto alternativo">
<img src="ruta" alt="texto alternativo" />
```

> **Nota:** La etiqueta `<img>` es autoconclusiva y no necesita etiqueta de cierre. En HTML5 puedes escribirla como `<img ...>` o `<img ... />`; la barra `/` al final es opcional y proviene de la sintaxis XHTML.

Ejemplos:

```html
<img src="logo.jpg" alt="ACME">
<img src="logo.jpg" alt="ACME" />
```

> **Incorrecto:**
```html
<img>
<img src="logo.jpg">
<img alt="ACME">
```

La ruta del archivo de imagen sigue las mismas reglas que los enlaces (`href`).

#### Atributo `alt` (texto alternativo)

El atributo `alt` es obligatorio y debe describir el contenido o función de la imagen. Es esencial para la accesibilidad (lectores de pantalla) y para casos en que la imagen no se carga.

Recomendaciones para el texto alternativo:
- Si la imagen está dentro de un enlace, el texto alternativo debe describir el destino del enlace.
- Si la imagen aporta información, el texto alternativo debe transmitir esa información.
- Si la imagen es decorativa, deja el atributo `alt` vacío (`alt=""`).

Ejemplos:
```html
<img src="lavado-mano.jpg" alt="Lavado a mano">
<img src="personas.jpg" alt="">
<a href="https://www.google.es">
	<img src="logo-google.jpg" alt="Google">
</a>
```

#### Diferencia entre `alt` y `title`

El atributo `alt` es para accesibilidad y SEO. El atributo `title` muestra un texto emergente al pasar el ratón, pero rara vez es necesario en imágenes. No los dupliques ni los uses con el mismo valor salvo justificación clara.

#### Imágenes como enlaces

Puedes usar una imagen como enlace envolviéndola en un elemento `<a>`:

```html
<a href="index.html">
	<img src="mapa.gif" alt="mapa web">
</a>
```

#### Formatos de imagen recomendados

- **PNG**: Formato sin pérdida, ideal para imágenes con transparencias y gráficos con pocos colores (iconos, logotipos, ilustraciones).
- **JPG (JPEG)**: Compresión con pérdida, adecuado para fotografías y gráficos con muchos colores. No soporta transparencias.
- **GIF**: Soporta animaciones y transparencias simples (un solo color transparente). Útil para imágenes animadas de baja resolución.
- **SVG**: Formato vectorial, escalable sin pérdida de calidad. Perfecto para iconos, logotipos y gráficos que deben adaptarse a cualquier tamaño.
- **WEBP**: Formato moderno con alta compresión y buena calidad, soporta transparencias y animaciones. Recomendado para optimizar el peso de imágenes en la web.
- **AVIF**: Formato de última generación, ofrece mayor compresión y calidad que WEBP y JPG. Soporta transparencias y animaciones. Ideal para máxima optimización.

Elige el formato según el tipo de imagen, necesidad de transparencia, calidad y peso.



#### Bancos de imágenes y recursos de iconos

- **[Lorem Picsum](https://picsum.photos/):** Servicio gratuito para obtener imágenes aleatorias de prueba, ideal para prototipos y maquetación. Permite especificar el tamaño y otras opciones en la URL.
	- Ejemplo de uso:
		```html
		<img src="https://picsum.photos/300/200" alt="Imagen aleatoria de Lorem Picsum">
		```
- **[Unsplash](http://unsplash.com/):** Banco de imágenes de alta calidad y libres de derechos para uso personal y comercial. Permite buscar y descargar fotografías profesionales en diferentes resoluciones.
	- Ejemplo de uso (descarga manual):
		1. Busca una imagen en Unsplash y descargarla.
		2. Sube la imagen a tu proyecto y usa:
		```html
		<img src="ruta/a/mi-imagen.jpg" alt="Descripción de la imagen de Unsplash">
		```
- **[Pexels](https://www.pexels.com/):** Plataforma de fotografías y videos gratuitos para uso personal y comercial. Permite buscar, descargar y utilizar imágenes de alta calidad sin necesidad de atribución (aunque se recomienda).
	- Ejemplo de uso (descarga manual):
		1. Busca una imagen en Pexels y descargarla.
		2. Sube la imagen a tu proyecto y usa:
		```html
		<img src="ruta/a/mi-imagen.jpg" alt="Descripción de la imagen de Pexels">
		```
- **[Iconfinder](https://www.iconfinder.com/):** Plataforma para buscar, descargar y comprar iconos en diferentes formatos (SVG, PNG, etc.), tanto gratuitos como de pago. Permite filtrar por licencia y estilo, ideal para proyectos web y aplicaciones.
	- Ejemplo de uso (descarga manual):
		1. Busca un icono en Iconfinder y descárgalo en el formato deseado (por ejemplo, SVG).
		2. Sube el icono a tu proyecto y usa:
		```html
		<img src="ruta/a/mi-icono.svg" alt="Descripción del icono">
		```

- **[Font Awesome](https://fontawesome.com/):** Biblioteca de iconos vectoriales y sociales ampliamente utilizada en desarrollo web. Permite integrar iconos mediante CDN, descarga o npm, y usarlos como fuentes o SVG en HTML y CSS.
	- Ejemplo de uso (CDN):
		1. Añade el siguiente enlace en la sección `<head>` de tu HTML:
		```html
		<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
		```
		2. Usa un icono en tu HTML:
		```html
		<i class="fa-solid fa-camera"></i>
		```


#### Mapas de imágenes

Un mapa de imágenes permite definir áreas activas (hotspots) sobre una imagen, que actúan como enlaces a diferentes recursos. Aunque su uso es poco frecuente hoy en día, pueden ser útiles en casos específicos. Si se utilizan, deben ser accesibles y, preferentemente, adaptables (responsive).

##### Ejemplo básico de mapa de imagen (no responsive)

```html
<img src="https://assets.codepen.io/513929/logos-mapa-imagen.jpg" usemap="#image-map" alt="Mapa de logos">

<map name="image-map">
	<area alt="HTML" title="HTML" href="https://es.wikipedia.org/wiki/HTML" coords="2,2,117,149" shape="rect">
	<area alt="CSS" title="CSS" href="https://es.wikipedia.org/wiki/CSS" coords="185,62,57" shape="circle">
	<area alt="Javascript" title="Javascript" href="https://es.wikipedia.org/wiki/JavaScript" coords="117,166,152,187,194,222,195,222,183,261,177,315,136,331,108,328,67,310,52,206,92,191,103,177" shape="poly">
</map>
```

**Explicación de atributos y formas:**

- `usemap="#image-map"`: Asocia la imagen con el mapa de áreas definido por `<map name="image-map">`.
- `<area shape="rect" coords="x1,y1,x2,y2">`: Área rectangular, define dos esquinas opuestas.
- `<area shape="circle" coords="x,y,r">`: Área circular, define el centro y el radio.
- `<area shape="poly" coords="x1,y1,x2,y2,...">`: Área poligonal, define múltiples vértices.
- `alt`: Texto alternativo para accesibilidad.
- `title`: Texto emergente al pasar el ratón (opcional).
- `href`: URL de destino.

> **Nota:** Las coordenadas se expresan en píxeles relativos a la imagen original. Cada área debe tener un texto alternativo (`alt`) descriptivo.

##### Recursos y generadores

- [HTML - Ejemplo Mapa de Imagen en CodePen](https://codepen.io/antxoa/pen/jORqjEw)
- [Generador de mapas de imagen (no RWD)](http://www.image-map.net/)
- [Generador de mapas de imagen responsive (SVG)](https://imagemapper.pageballoon.com/)

> **Recomendación:** Prioriza siempre la accesibilidad y la optimización de imágenes para mejorar la experiencia de usuario y el rendimiento del sitio web. Considera usar SVG para mapas de imagen responsive.


### Títulos (Encabezados) en HTML

Los títulos o encabezados (`<h1>` a `<h6>`) permiten estructurar la información de la página en diferentes niveles jerárquicos, facilitando la comprensión, accesibilidad y SEO del contenido.

#### ¿Se puede tener un título que no se vea?

Sí, es posible incluir un título (por ejemplo, un `<h1>`) que no sea visible para los usuarios, pero que esté presente en el código HTML. Esto se suele hacer usando técnicas de CSS para ocultarlo visualmente. Esta práctica puede ser útil para mejorar la accesibilidad (por ejemplo, para lectores de pantalla) o para SEO, permitiendo que los motores de búsqueda y tecnologías asistivas detecten información importante aunque no se muestre en pantalla.

**¿Es buena práctica?**

Solo se recomienda ocultar títulos si existe una razón justificada, como necesidades de accesibilidad o estructura semántica para SEO, pero el diseño visual no permite mostrar el título. No debe usarse para ocultar información relevante a los usuarios con fines engañosos. Si se usa correctamente, es una técnica aceptada y útil en desarrollo web profesional.

#### Jerarquía y uso correcto

- Existen 6 niveles de encabezado: `<h1>`, `<h2>`, `<h3>`, `<h4>`, `<h5>`, `<h6>`, siendo `<h1>` el más importante.
- Cada encabezado debe tener su etiqueta de apertura y cierre.
- Se recomienda utilizar un solo `<h1>` por página, representando el tema principal.
- Los encabezados deben seguir un orden jerárquico: no uses un `<h2>` sin haber usado antes un `<h1>`, ni saltes niveles (por ejemplo, de `<h2>` a `<h4>` sin un `<h3>` intermedio).

#### Ejemplo correcto

```html
<h1>Servicios</h1>
<p>Empresa ACME le proporciona los siguientes servicios:</p>

<h2>Catering</h2>
<p>Por un módico precio, puede disfrutar de la mejor y más variada comida del mundo…</p>

<h2>Preparación oposiciones</h2>
<p>Nuestro personal estará encantado en ayudarle a preparar las siguientes oposiciones:</p>

<h3>Ayudante de Chef</h3>
<p>bla, bla, bla</p>

<h3>Ayudante de cocina</h3>
<p>bla, bla, bla</p>

<h2>Formación privada</h2>
<p>Si lo desea, podemos enseñarle a preparar usted mismo los exquisitos platos...</p>
```

#### Ejemplo incorrecto

```html
<h2>Servicios</h2>
<p>Empresa ACME le proporciona los siguientes servicios:</p>

<h1>Catering</h1>
<p>Por un módico precio, puede disfrutar de la mejor y más variada comida del mundo…</p>

<h2>Preparación oposiciones</h2>
<p>Nuestro personal estará encantado en ayudarle a preparar las siguientes oposiciones:</p>

<h3>Ayudante de Chef</h3>
<p>bla, bla, bla</p>

<h3>Ayudante de cocina</h3>
<p>bla, bla, bla</p>

<h4>Formación privada</h4>
<p>Si lo desea, podemos enseñarle a preparar usted mismo los exquisitos platos...</p>
```

#### Buenas prácticas

- Utiliza los encabezados para reflejar la estructura lógica del contenido, no solo para dar formato visual.
- No utilices los encabezados para cambiar el tamaño del texto; usa CSS para estilos visuales.
- Mantén la jerarquía y evita saltos de nivel.
- Un solo `<h1>` por página es lo recomendado para accesibilidad y SEO.

> **También puedes incluir imágenes dentro de los encabezados** (por ejemplo, logotipos o iconos), pero siempre acompañadas de texto para mantener la accesibilidad y el SEO. Ejemplo:
> ```html
> <h1><img src="logo.png" alt="Logo"> Título principal</h1>
> ```
> La imagen no debe ser el único contenido del encabezado.

#### Especificación oficial y ejemplos

- [Especificación oficial de encabezados HTML](https://html.spec.whatwg.org/multipage/sections.html#the-h1,-h2,-h3,-h4,-h5,-and-h6-elements): Explica el propósito, uso y reglas de los elementos de encabezado.
- [Ejemplos de estructura y jerarquía de títulos](https://html.spec.whatwg.org/multipage/sections.html#headings-and-outlines-2): Muestra cómo los encabezados definen la estructura y el esquema de la página.

### listas

- **Listas desordenadas** (`<ul>`): Elementos sin orden específico, con viñetas.
- **Listas ordenadas** (`<ol>`): Elementos con orden, numerados automáticamente.
- **Listas de definición** (`<dl>`): Pares de término y definición.

### 1. Etiquetas principales y ejemplos

- `<ul>` (**Unordered List**): Contenedor de lista desordenada.
		```html
		<ul>
			<li>Elemento 1</li>
			<li>Elemento 2</li>
		</ul>
		```
- `<ol>` (**Ordered List**): Contenedor de lista ordenada.
		```html
		<ol>
			<li>Paso 1</li>
			<li>Paso 2</li>
		</ol>
		```
- `<li>` (**List Item**): Elemento de lista, hijo de `<ul>` o `<ol>`. Puedes tener tantos como necesites.
		```html
		<ul>
			<li>Elemento A</li>
			<li>Elemento B</li>
		</ul>
		```
- `<dl>` (**Description List**): Contenedor de lista de definiciones.
		```html
		<dl>
			<dt>Término</dt>
			<dd>Definición</dd>
		</dl>
		```
- `<dt>` (**Definition Term**): Término a definir en `<dl>`.
		```html
		<dl>
			<dt>HTML</dt>
			<dd>Lenguaje de marcado</dd>
		</dl>
		```
- `<dd>` (**Definition Description**): Definición del término anterior en `<dl>`.
		```html
		<dl>
			<dt>CSS</dt>
			<dd>Lenguaje de estilos</dd>
		</dl>
		```

### 2. Contenido permitido en `<li>`

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

### 3. Listas anidadas

Puedes anidar listas para crear jerarquías. **Una lista (`<ul>` o `<ol>`) solo puede estar dentro de un `<li>`, nunca directamente dentro de `<ul>` o `<ol>`.** Puedes anidar tantas sublistas como desees, pero se recomienda no abusar para mantener la legibilidad y accesibilidad.

Ejemplo correcto:
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
Ejemplo incorrecto:
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

### 4. Listas de definición avanzadas

Las listas de definición (`<dl>`) pueden tener varios `<dd>` para un mismo `<dt>`.

```html
<dl>
	<dt>Plataformas</dt>
	<dd>Linux</dd>
	<dd>Mac</dd>
	<dd>Windows</dd>
</dl>
```


### 5. Personalización visual

Si se desea, es posible cambiar el tipo de viñeta o numeración de las listas mediante CSS. No es necesario saber CSS en este momento, solo conocer que existe esa posibilidad.

### 6. Sangría y espaciado

Los navegadores aplican sangría por defecto. Puedes modificarla con CSS:
```css
ul, ol { margin-left: 2em; padding-left: 40px; }
ul, ol { margin-left: 0; padding-left: 0; } /* Para eliminar sangría */
```
Recomendación: Ajusta solo si el diseño lo requiere, pero mantén la semántica.

### 7. Mejores prácticas

- Usa el tipo de lista adecuado según el contenido.
- Las sublistas siempre dentro de `<li>`.
- Personaliza solo con CSS, no cambies la semántica.
- No uses listas solo para sangrar texto o maquetar.
- Mantén la accesibilidad y la estructura clara.

### 8. Documentación oficial

- [Listas en HTML Living Standard (WHATWG)](https://html.spec.whatwg.org/multipage/grouping-content.html#the-ul-element)
- [MDN Web Docs: Listas HTML](https://developer.mozilla.org/es/docs/Web/HTML/Element/ul)

### Ejemplo de lista desordenada

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

### Ejemplo de lista ordenada

```html
<h2>Preparación</h2>
<ol>
	<li>Triturar en la batidora los pimientos y los tomates partidos por la mitad, los pepinos pelados, los ajos, el pan, y el aceite, con un chorrito de vinagre, un poco de agua y sal.</li>
	<li>Batir muy bien</li>
	<li>Verter todo en la fuente en la que vaya a ser servido y agregar agua hasta que adquiera la consistencia de una crema ligera.</li>
	<li>Servir muy frío.</li>
</ol>
```


### Listas anidadas

Las listas pueden anidarse para crear jerarquías. **Una lista (`<ul>` o `<ol>`) solo puede estar dentro de un elemento `<li>`, nunca directamente dentro de `<ul>` o `<ol>`.** Esto asegura la estructura semántica y la validez del HTML.

Puedes anidar tantas sublistas como desees, creando varios niveles de profundidad, siempre que cada sublista esté dentro de un `<li>`. No hay un límite técnico, pero se recomienda no abusar para mantener la legibilidad y accesibilidad del contenido.

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

**Incorrecto:**

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

### Listas de definición

Las listas de definición (`<dl>`) agrupan términos (`<dt>`) y sus definiciones (`<dd>`). Un término puede tener varias definiciones.

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

### Mejores prácticas

- Utiliza el tipo de lista adecuado según el contenido (ordenada, desordenada o de definición).
- Las sublistas deben estar siempre dentro de un `<li>`.
- Usa CSS para personalizar la apariencia, nunca cambies la semántica de la lista solo por motivos visuales.
- No utilices listas solo para sangrar texto o maquetar, deben tener sentido semántico.


### Sangría de las listas

### Personalización de viñetas y numeración con CSS

Puedes cambiar el tipo de viñeta de las listas desordenadas (`<ul>`) y el tipo de numeración de las listas ordenadas (`<ol>`) usando la propiedad CSS `list-style-type`.

Consulta la documentación de CSS para más opciones: [MDN list-style-type](https://developer.mozilla.org/es/docs/Web/CSS/list-style-type)

Por defecto, los navegadores aplican una sangría (indentación) a las listas (`<ul>`, `<ol>`, `<dl>`) para diferenciarlas del resto del contenido. Esta sangría puede variar según el navegador y el sistema operativo.

**Controlar la sangría con CSS:**

Puedes modificar o eliminar la sangría de las listas usando las propiedades CSS `margin` y `padding`. Por 
**Recomendación:** Ajusta la sangría solo si el diseño lo requiere, pero mantén la estructura semántica de la lista. No uses listas únicamente para crear sangrías visuales; utiliza listas solo cuando el contenido lo justifique.

### Documentación oficial

- [Listas en HTML Living Standard (WHATWG)](https://html.spec.whatwg.org/multipage/grouping-content.html#the-ul-element)
- [MDN Web Docs: Listas HTML](https://developer.mozilla.org/es/docs/Web/HTML/Element/ul)

### Tablas

### Otros elementos
