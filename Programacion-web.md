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

#### Extensiones recomendadas
- **Web Developer**: Añade un conjunto de herramientas útiles para desarrolladores web ([Chrome Web Store](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm?hl=es)).
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

**Recomendación:** Mantén coherencia en el estilo de autocierre que elijas para todo tu proyecto.

**Incorrecto:** No inventes etiquetas de cierre para etiquetas autoconclusivas.

```html
<!-- Esto es incorrecto -->
<etiquetaautocierre>
</etiquetaautocierre>
```

#### Semántica y variedad de etiquetas

HTML ofrece muchas etiquetas para describir el significado del contenido. Utiliza la etiqueta adecuada para cada tipo de información. La presentación visual se gestiona con CSS, no con HTML.

#### Comentarios en HTML

Para documentar o desactivar partes del código, utiliza comentarios:

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

- PNG, JPG (JPEG), GIF, SVG, WEBP.

Elige el formato según el tipo de imagen, transparencia, calidad y peso.

#### Bancos de imágenes y recursos de iconos

- [Lorem Picsum (imágenes aleatorias)](https://picsum.photos/)
- [Unsplash (fotos de alta calidad)](http://unsplash.com/)
- [Pexels (fotos gratuitas)](https://www.pexels.com/)
- [Iconfinder (iconos)](https://www.iconfinder.com/)

#### Mapas de imágenes

Un mapa de imágenes define áreas activas (hotspots) sobre una imagen que actúan como enlaces. Actualmente su uso es poco frecuente y, si se utilizan, deben ser accesibles y adaptables (responsive).

> **Recomendación:** Prioriza siempre la accesibilidad y la optimización de imágenes para mejorar la experiencia de usuario y el rendimiento del sitio web.

### Títulos

### Listas

### Tablas

### Otros elementos