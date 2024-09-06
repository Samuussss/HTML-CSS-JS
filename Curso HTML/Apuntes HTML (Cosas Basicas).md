# Apuntes HTML by Samuussss

## ¿como se compone una pagina web?

```html
<!DOCTYPE html>  <!-- Define el tipo de documento -->
<html>           <!-- Elemento raíz de la página HTML -->
<head>           <!-- Contiene metadatos sobre el documento -->
  <title>        <!-- Título de la página, mostrado en la pestaña del navegador -->
</head>
<body>           <!-- Contiene el contenido visible de la página -->
  <h1>           <!-- Encabezado principal (nivel 1), el más importante -->
  <h2>           <!-- Encabezado secundario (nivel 2) -->
  <h3>           <!-- Encabezado terciario (nivel 3) -->
  <p>            <!-- Párrafo de texto -->
  <a href="#">   <!-- Enlace, el atributo href especifica el destino del enlace -->
  <img src="#" alt="Descripción"> <!-- Imagen, el atributo src especifica la fuente y alt proporciona una descripción alternativa -->
  <ul>           <!-- Lista desordenada -->
    <li>        <!-- Elemento de lista -->
  </ul>
  <ol>           <!-- Lista ordenada -->
    <li>        <!-- Elemento de lista -->
  </ol>
  <table>        <!-- Tabla -->
    <tr>        <!-- Fila de la tabla -->
      <td>      <!-- Celda de datos -->
      <th>      <!-- Celda de encabezado -->
    </tr>
  </table>
  <form>         <!-- Formulario para enviar datos -->
    <input type="text">  <!-- Campo de entrada de texto -->
    <button>        <!-- Botón para enviar el formulario -->
  </form>
  <div>          <!-- Contenedor genérico para agrupar elementos -->
  <span>         <!-- Contenedor en línea para agrupar elementos -->
</body>
</html>
```

`------------------------------------`

#### Etiquetas Generales (algunas)

```html
<h1> TITULO IMPORTANTE </h1>

<h2> SUBTITULOS IMPORTANTES </h2>
```

"**h**" es lo mas importante de la pagina y **el h1** es al que **google le da mas importancia**,la importancia baja segun **Cuantos h1** usemos, y puede recivir una **penalizacion** la pagina **si usamos muchos**(si esto pasa **solo podremos usar un h1**), estos **llegan hasta el h6**. 

#### Se Escriben asi:
"
`<h1>Contenido</h1>`
`<h2>Contenido</h2>`
`<h3>Contenido</h3>`
`<h4>Contenido</h4>`
`<h5>Contenido</h5>`
`<h6>Contenido</h6>`
"

#### Y se ven asi:

<h1>Contenido</h1>
<h2>Contenido</h2>
<h3>Contenido</h3>
<h4>Contenido</h4>
<h5>Contenido</h5>
<h6>Contenido</h6>

`------------------------------------`

## listas:

list item: - `<li> item </li>` - es la forma en la que **el navegador reconoce el contenido de las listas**.

orderer list: - `<ol> lista ordenada </ol>` - es la forma en la que **el navegador reconoce** que **SI** es una **lista ordenada**.

unorderer list: - `<ul> lista desordenada </ul>` - es la forma en la que **el navegador reconoce** que **NO** es una **lista ordenada**.

#### Ordenadas:

```html
<ol>
    <li>Elemento 1</<li>
    <li>Elemento 2</<li>
    <li>Elemento 3</<li>
    <li>Elemento 4</<li>
</ol>
```

cuando el **orden importa** se usa este tipo de listas, ya que **enumera la lista**, Como a continuacion:

```html
 1.Elemento1
 2.Elemento2
 3.Elemento3
```

#### Desordenadas:

cuando el **orden no importa** se usa este tipo de listas, ya que **pone puntos**, como a continuacion:

"
 * Elemento1
 * Elemento2
 * Elemento3

"
#### y se escriben asi:

```html
<ul>
    <li>Elemento 1</<li>
    <li>Elemento 2</<li>
    <li>Elemento 3</<li>
    <li>Elemento 4</<li>
</ul>
```

`------------------------------------`
## Enlaces

pueden ser llamados tambien "hiper vinculos" la etiqueta para los enlaces es `<a> </a>` para que la etiqueta sea funcional y nos reediriga a una pagina debemos darle un atributo, como **"href"** para que funcione debe tener:
 **" //youtu... "** pero se recomienda **" https://youtu... "** por seguridad, **posicionamiento**, etc.
 la estructura seria de la siguiente forma:
```html
<!DOCTYPE html>
<html>
<head>
    <title>Enlaces</title>
</head>
<body>
    <a href= "https://github.com/sami-heart">Esto Se ve en lugar del enlace</a>
</body>
</html>
```
el resultado del codigo seria:

"<!DOCTYPE html>
<html>
<head>
    <title>Enlaces</title>
</head>
<body>
    <a href= "https://github.com/samuussss">Esto Se ve en lugar del enlace</a>
</body>
</html>

"

`------------------------------------`
## Atributos y Propiedades
### Atributos
Un **atributo** es lo que está dentro de las etiquetas (`"<"` y "`>"`). Define características adicionales sobre los elementos HTML.

Ejemplo:
```html
<p title="Esto es un título">Este es un párrafo</p>
```

En este caso, `title` es un atributo del elemento `p`.

Otro ejemplo común es el atributo `href` en un enlace:

```html
<a href="https://www.example.com">Visitar ejemplo</a>
```

### Propiedades (CSS y JavaScript)
Las propiedades se manejan fuera de las etiquetas `HTML`, ya sea mediante `JavaScript` o `CSS`. Son dinámicas y se pueden modificar en tiempo de ejecución o mediante estilos.

### Propiedades CSS:
Son parte de la presentación visual de los elementos. Definen cómo se ve un elemento en la página.

##### Ejemplo de propiedades CSS:

```css
p {
  color: red;
  font-size: 16px;
}
```

En este caso, `color` y `font-size` son propiedades `CSS` que afectan el estilo del párrafo.

### Propiedades en JavaScript:
Son parte del `DOM (Document Object Model)` y representan el estado actual de los elementos. Estas propiedades se pueden acceder y modificar a través de scripts.

##### Ejemplo de propiedades JavaScript:

```js
const link = document.querySelector('a');
console.log(link.href); // Muestra la URL del enlace
link.href = "https://www.nuevaurl.com"; // Cambia la propiedad href del enlace
```

Aquí, `href` es una propiedad en el contexto de `JavaScript`, y su valor puede cambiar dinámicamente.

