# aprenda-los-colores-de-css-construyendo-un-conjunto-de-marcadores-de-colores

Página web creada en el curso "Aprenda los colores de CSS construyendo un
conjunto de marcadores de colores", perteneciente a la certificación "Diseño Web
Responsivo" de freeCodeCamp.

---

[Enlace a la web](https://colored-markers-bde.netlify.app/)

---

- Primero creamos una estructura HTML para crear la página web.
- Creamos un archivo "styles.css" y agregamos el link al archivo html.
- Tras haber creado el titulo de la página (h1), creamos un `<div>` y le
  añadimos una clase con el nombre `container` .

- Creamos otro `<div>` anidado, dentro del `<div>` anterior. Le damos la clase
  `marker`.

- En el .css seleccionamos a la clase `marker` y le damos un `background-color`
  con un valor `red` .

- El color de fondo en `marker` se ha aplicado, pero como el elemento `<div>`
  `marker` no tiene contenido, este no tiene altura de forma predeterminada. Es
por esto que no podemos ver los cambios en la página. Para ver los cambios le
daremos a la clase `marker` una _propiedad-valor_ `height: 25px;` y otra
_propiedad-valor_ `width: 200px;` .

- Con la _propiedad-valor_ `margin: auto;` hacemos que todos los valores de margen
(top, bottom, left y right) se establezcan de manera conjunta y de forma
automática, con valores basados en la posición del elemento en la pagina.

- Anadimos dos elementos `<div>` mas dentro de `container`

- Se veran los tres `<div>` como un solo bloque. Para separarlos, modificamos el
  atributo `margin` de la clase `marker` a `margin: 10px auto;` . El primer
valor (10px) aplica el valor a `margin-top` y `margin-bottom` , mientras que el
segundo (auto) se aplica a `margin-left` y `margin-right` .

- Para que cada marcador (div) tenga un color diferente, hay que añadir una clase
única para cada uno de ellos. Podemos añadir múltiples clases dentro de un mismo
elemento _html_ listándolas juntas y separadas por un espacio:

    `<div class="marker uno">`

    Esto sin embargo, puede generar problemas, ya que los valores que se le den
a la primera clase, serán sobre-escritos por el valor de la clase que le
precede.

- Para solucionar el problema descrito anteriormente, llamamos a la clase que
queremos estilizar directamente por su nombre único; es decir que si queremos
estilizar el `<div>` `marker uno` , lo llamamos nombrando directamente la clase
`uno` :
    `.uno {}`

- Se aplico el color de fondo, pero como el elemento marcador `<div>` no tiene
  contenido, este no tiene altura de forma predeterminada.

- Hay dos modelos principales de colores:
    - Aditivo: RGB (Red Green Blue), aplicado a dispositivos electrónicos.
    - Sustractivo: CMYK (Cyan Magenta Yellow Black), aplicado a la impresión en
      papel.

- En RGB, los colores comienzan como negro y cambian conforme se introducen
  diferentes niveles de rojo, verde y/o azul.

- Para agregar color mediante RGB utilizamos la función `rgb()` . Como ejemplo,
  para introducir el color negro escribiremos `rgb(0, 0, 0)` .
Mientras que para el color blanco, el código será `rgb(255, 255, 255)` . Como
podemos ver, los valores de color se introducen en el orden (red, green, blue)
separados entre sí por una coma.

- Cada valor puede contener un numero que irá desde el 0 (que es el 0% y
  significa negro) hasta 255 (que es 100% de ese color).

- Como ejemplo, para poner un marcador de color rojo escribiremos la función
`rgb(255, 0, 0);` .

- La palabra clave del color `green` , es en realidad una sombra mas oscura que
  el verde puro de `rgb()` . Para obtener un verde del mismo tono que teníamos
con la palabra clave `green` , ponemos el valor `rgb()` a 127. De ese modo,
reducimos su intensidad.

- Con la _propiedad-valor_ `padding: 10px 0px;` separamos los marcadores del
elemento con clase `.container` . La forma de introducir los valores en
`padding` es idéntica a como lo hicimos anteriormente.

- Para conseguir el blanco puro es necesario poder combinar todos los colores
  con todos los valores _rgb_ en su máximo nivel. Debido a esto, volvemos a
poner el color verde en su maximo valor (255).

- Los colores **primarios** son los colores puros. Los colores **secundarios**
  son los que obtienes al combinar los primarios.

- La combinación de colores primarios con colores secundarios cercanos crea
  colores terciarios.

- En _rgb_ , 0 es color negro, 255 es color puro y 127 es color medio.

- Tipos de color:

- - Primarios:
- - - rojo: (255, 0, 0)
- - - verde: (0, 255, 0)
- - - azul: (0, 0, 255)
<br>
- - Secundarios:
- - - amarillo: (255, 255, 0)
- - - cian: (0, 255, 255)
- - - magenta: (255, 0, 255)
<br>
- - Terciarios:
- - - naranja: (255, 127, 0)
- - - verde primavera: (0, 255, 127)
- - - violeta: (127, 0, 255)

- Ademas de los colores terciarios descritos arriba, existen muchos más. Otros
  ejemplos serian:
- - verde chartreuse [verde + amarillo]: (127, 255, 0)
- - azur [azul + cian]: (0, 127, 255)
- - rosa [rojo + magenta]: (255, 0, 127)

- Una rueda de color es un circulo donde colores similares o *hues *, están cerca unos de otros, y los diferentes están mas separados. Como ejemplo, el rojo puro esta entre los tonos rosa y naranja.

- Dos colores opuestos entre si en la rueda de color se llaman "complementary colors". Si se combinan dos *colores complementarios* , estos producen gris. Pero cuando se colocan lado a lado, estos colores producen un fuerte contraste visual y **parecen** mas brillantes.

- Dos colores que sean muy brillantes, estando uno al lado del otro, pueden distraer la atención. Además, puede hacer que un texto sea difícil de leer. Es mejor elegir un color como dominante, y utilizar su complementario como énfasis para dirigir la atención sobre determinado contenido de la página.

- Ademas de los colores complementarios, hay otras combinaciones de colores importantes.

- Los valores de color **hexadecimales** no son más que otra forma de expresar colores **RGB** .

- Los valores hexadecimales comienzan con una almohadilla (#), seguida de 6 caracteres entre 0-9 y A-F. El primer par de numeros representa el color rojo, el segundo el verde y el tercer par el color azul. Un ejemplo de valor hexadecimal seria: #4B5320

- Los valores hexadecimales no deben de ir dentro de una función RGB, sino que se escriben fuera de cualquier función:
    `background-color: #4B5320`

- Estamos familiarizados a utilizar los valores en **base 10** que tienen los valores:
    (0, 1, 2, 3, 4, 5, 6, 7, 8, 9).
    Los valores en **base 16** , tambien llamados velores **hexdecimales** , van de 0 a 9 y a continuacion de A  a F, es decir:
    (0, 1, 2, 3, 4, 5, 6, 7, 8, 9, A, B, C, D, E, F)

- El par 00 se traduce como el 0% de color, siendo FF el 100%. como ejemplo, el valor hexadecimal #00FF00 se traduce en 0% rojo (R), 100% verde (G) y 0% azul (B).

- Disminuyendo el valor del primer numero del par, bajamos la intensidad de dicho color. Por ejemplo, 7F será menos intenso que FF.

- Otra forma de representar colores es el modelo HSL, que son las siglas de **hue** (matiz), **saturation** (saturación) y **lightness** (luminosidad).

- El **matiz** (hue) es el tono de color. Se indica en grados, representado en el circulo cromático. El color *rojo* está en 0°, el *verde* está en 120° y el *azul* en 240°.

- La **saturación** es la intensidad de un color y va desde el 0% o *gris*  hasta el 100% para el *color puro* .

- La **luminosidad** es lo brillante que parece un color. Va desde el 0% que es *completamente negro* , hasta el 100% que es *completamente blanco* . El *neutro* se representa con el 50%.

- La función HSL se escribe:
    `hsl(240, 100%, 50%)`

- Podemos representar los colores utilizando gradientes, en lugar de colores planos. Para ello tenemos la función CSS `linear-gradient` . `linear-gradient` permite controlar la dirección de la transición a lo largo de una linea, así como los colores que participan en el degradado.

- Es importante destacar que `linear-gradient` en realidad crea un elemento `image` , y se asocia normalmente con la propiedad `background` , la cual acepta una imagen como valor.

- Ejemplo de código con `linear-gradient` :
    `linear-gradient(direccionDelGradiente, color1, color2, …);`
    Así por ejemplo podríamos aplicar lo siguiente:
    `background: linear-gradient(90deg, rgb(255, 0, 0), rgb(0, 255, 0));`
    El primer parametro se da en *grados(deg)* , el resto de parametros (los de color) pueden expresarse tanto en `rgb` , como en *hex*  0 `hsl` .
    La linea de codigo de arriba crea un degradado suave que va desde el rojo hasta el verde. Aunque el mínimo de colores necesarios para un degradado es de dos, `linear-gradient` acepta bastantes más.

- Existe otro parametro llamado **parada de color** . En la función `liner-gradient` , podemos agregar una valor en `px` o porcentaje `%` justo detrás del valor de color que queremos modificar. Por ejemplo, para alargar en un 75% dentro de la transición del gradiente, el primer color (rojo) del anterior código, escribiríamos lo siguiente:
    `background: linear-gradient(90deg, rgb(255, 0, 0) 75%, rgb(0, 255, 0));`

- Oscureciendo los bordes podemos darle a un elemento un efecto de mayor volumen.

- Un `linear-gradient` con valores *hexadecimales* se verá de la siguiente forma:
    `background: linear-gradient(180deg, #55680D, #71F53E, #116C31);`

- La funcion `linear-gradient` calcula de forma automática los valores de *parada* , repartiendo de forma equitativa los colores a lo largo de la linea del gradiente. Por defecto, este reparto sera del 0%, 50% y 100% para un gradiente de tres colores.

- Si no se especifica el argumento `direccionDelGradiente` en la funcion `linear-gradient` , este tendrá un valor por defecto de 180 grados, disponiendo los colores desde arriba hacia abajo.

- La propiedad `opacity` establece la **opacidad** de un elemento.

- Existe otra forma de establecer la **opacidad** , el **canal alpha** .

- El canal `alpha` puede ser utilizado tanto para `rgb` como para *hex*  y `hsl` .

- Ejemplo `rgb` :
    `rgba(255, 255, 255, 50%);`

- Todos los elementos HTML tienen **bordes** , pero por defecto están establecidos a *none* .Con CSS se tiene el control total sobre los bordes de un elemento. Para que un borde sea visible, hay que darle un grosor (width) y estilo (style). Un ejemplo seria:  `border-left-width`  `border-left-style` .

- Los **bordes** tienen varios estilos para elegir:
    - linea continua: `solid`
    - linea discontinua: `dashed`
    - Linea punteada: `dotted`

    Lo normal es que sean lineas continuas.

- El color del borde por defecto sera el negro. Aunque, por razones de legibilidad, es mejor que especifiques el color `border-left-color: black`

- La propiedad abreviada `border-left` , permite establecer el grosor, el estilo y el color del borde de forma simultanea:
    `border-left: 10px solid black;`

- También tenemos el estilo de borde `double` , que nos genera un linea doble (dos lineas).

- Podemos aplicar **sombras** a los elementos HTML con la propiedad `box-shadow` .

- La sintaxis de `box-shadow` es:
    `box-shadow: offsetX offsetY color;`
    - Tanto `offsetX` como `offsetY` aceptan valores numericos en `px` y otras unidades CSS.
    - Los valores positivos en `offsetX` mueven la sombra hacia la derecha y los valores negativos la mueven hacia la izquierda.
    - Los valores positivos en `offsetY` mueven la sombra hacia abajo, mientras que un valor negativo la sube.
    - Si queremos un valor 0 para `offsetx`  y/o `offsetY` , no es necesario agregar una unidad, ya que los navegadores entienden que cero significa que no hay cambios.

- La *altura*  y la *anchura*  de las **sombras** están determinadas por la altura y la anchura del elemento al que se aplica. También se puede utilizar un valor `spreadRadius` opcional para extender el alcance de la sombra.

- Podemos difuminar los limites de la sombra con `blurRadius` , haciendo que los limites de esta no sean tan bruscos.
    `box-shadow: offsetX offsetY blurRadius color;`
    `box-shadow: 5px 5px 5px green;`
    Para el valor *cero*  no es necesario indicar la unidad:
    `box-shadow: 0 0 20px green;`

- El parametro de color de `box-shadow` obviamente se puede expresar en `rgba` , *hex* y `hsla`

- Fin

