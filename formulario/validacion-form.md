# Programación web en entorno cliente
## HTML
### Formulario
#### Validación Formulario
Resumen de los principales atributos y patrones para validar formularios en HTML.

---

##### Desactivar validación nativa
Permite desactivar la validación automática de un formulario o campo usando el atributo `novalidate`:

```html
<form ... novalidate>
	...
</form>
```

---

##### Campo obligatorio
El atributo `required` obliga a completar un campo antes de enviar el formulario:

```html
<input type="text" name="nombre" required>
```

---

##### Validación por patrón
El atributo `pattern` define una expresión regular para validar el formato del campo. Se recomienda usar también `title` para guiar al usuario:

```html
<input type="text" name="codIdioma" pattern="[A-z]{2}" title="2 letras">
<input type="text" name="usuario" pattern="[A-Za-z0-9]{6,10}" title="6-10 letras o números">
<input type="tel" name="tel" pattern="([0-9]{1}(-[0-9]{3})(-[0-9]{3})(-[0-9]{4}))" title="1-234-567-8910">
```

---

##### Patrones RegExp comunes

| Patrón | Significado                | Ejemplo o uso        |
| ------ | -------------------------- | -------------------- |
| .      | Cualquier carácter         | `a.b` → "acb", "a9b" |
| [0-9]  | Un dígito                  | `\d`                 |
| [A-Z]  | Letra mayúscula            |                      |
| [^A-Z] | No mayúscula               |                      |
| *      | 0 o más repeticiones       | `[0-9]*`             |
| +      | 1 o más repeticiones       | `[0-9]+`             |
| {n}    | Exactamente n repeticiones | `[0-9]{3}`           |
| {n,m}  | Entre n y m repeticiones   | `[0-9]{2,4}`         |
| ?      | Opcional                   | `b?`                 |
| \\     | Escape                     | `\.` → punto literal |

---

##### Patrones RegExp avanzados

| Patrón   | Significado                             | Ejemplo o uso                            |
| -------- | --------------------------------------- | ---------------------------------------- |
| ^        | Inicio de línea                         | `^abc` → empieza por "abc"               |
| $        | Fin de línea                            | `abc$` → termina en "abc"                |
| [a-zA-Z] | Cualquier letra (mayúscula o minúscula) |                                          |
| \s       | Espacio en blanco (incluye tab y salto) | `\s+` → uno o más espacios               |
| \S       | No espacio en blanco                    |                                          |
| \w       | Carácter alfanumérico o guion bajo      | `\w+` → palabra                          |
| \W       | No alfanumérico                         |                                          |
| (a       | b)                                      | Alternancia (a o b)                      | `rojo | azul` |
| (?:...)  | Agrupación sin captura                  | `(?:abc){2}` → "abcba"                  |
| (?=...)  | Lookahead positivo (lo que sigue)       | `\d(?=€)` → dígito seguido de €          |
| (?<=...) | Lookbehind positivo (lo que precede)    | `(?<=#)\w+` → palabra tras #             |
| (?!)     | Lookahead negativo (lo que NO sigue)    | `foo(?!bar)` → "foo" no seguido de "bar" |
| (?<!...) | Lookbehind negativo (lo que NO precede) | `(?<!@)gmail` → "gmail" no tras @        |

> Nota: No todos los navegadores soportan lookahead/lookbehind en HTML5, pero sí en la mayoría de lenguajes modernos.

#### referencias
[Expresiones regulares](https://support.google.com/a/answer/1346938)
[Tutorial de patrones](https://input-pattern.com/en/tutorial.php)
[Librería expresiones regulares](https://www.regexlib.com/Default.aspx)