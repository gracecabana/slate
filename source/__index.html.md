---
includes:
- errors
language_tabs:
- html
- css
- javascript
search: True
title: 'S4N - Librería de componentes'
toc_footers:
- '<a href=''#''>Sign Up for a Developer Key</a>'
- |
    <a href='https://github.com/tripit/slate'>Documentation Powered by
    Slate</a>
...

Introducción
============

Intro bella redactada por Andy aquí :)

Botón
=====

Descripción
-----------

Existen tres tipos de botones, cada uno puede trabajarse en tres tamaños
distintos y cada uno tiene diferentes estados, estas características
deben ser transversales sin importar los estilos que se usen para
personalizarlos. Lo anterior se puede dividir en dos grupos: “Botones
Evidentes” y “Botones Sutiles”.

Botones evidentes
-----------------

Que tienen un color de fondo

```html
<button class="small">Click me</button>

<button class="medium">Click me</button>

<button class="big">Click me</button>

<button><i></i><span>Click me</span></button>

<button class="inactive">Click me</button>
```

```css
button{
  font-family:"Raleway";
  cursor:pointer;
  outline:none;
}
button:hover{
  background:#ffffff;
  outline:none;
}
button:active{
  background:#cccccc;
  outline:none;
}
button.small{
  font-size:0.7em;
}
button.medium{
  font-size:1em;
}
button.big{
  font-size:1.5em;
}
button i{
  width:15px;
  height:15px;
  display:inline-block;
  background:url(../svg/icon-download.svg) no-repeat 50% 50%;
  background-size:100% auto;
}
button span{
  display:inline-block;
  margin:0 0 0 5px;
}
button.inactive{
  cursor:not-allowed;
  background:#aaaaaa;
}
button.inactive:hover{
  background:#aaaaaa;
  outline:none;
}
button.inactive:active{
  background:#aaaaaa;
  outline:none;
}
```

#### Small

<button class="small">
Click me
</button>

#### Medium

<button class="medium">
Click me
</button>

#### Big

<button class="big">
Click me
</button>

#### Ícono y texto

<button>
<i></i><span>Click me</span>
</button>

#### Inactivo

<button class="inactive">
Click me
</button>
Botones sutiles
---------------

Que tienen fondo transparente.

```html
<button class="small sutil">Click me</button>

<button class="medium sutil">Click me</button>

<button class="big sutil">Click me</button>

<button class="sutil"><i></i></button>

<button class="sutil"><i></i><span>Click me</span></button>

<button class="inactive sutil">Click me</button>
```

```css
button.sutil{
  font-family:"Raleway";
  cursor:pointer;
  outline:none;
  background:transparent;
}
button.sutil:hover{
  background:transparent;
  outline:none;
  opacity:0.8;
}
button.sutil:active{
  background:transparent;
  outline:none;
  opacity:0.8;
}
button.sutil i{
  width:15px;
  height:15px;
  display:inline-block;
  background:url(../svg/icon-download.svg) no-repeat 50% 50%;
  background-color:transparent;
  background-size:100% auto;
}
button.sutil span{
  display:inline-block;
  margin:0 0 0 5px;
}
button.sutil.inactive{
  cursor:not-allowed;
  background:transparent;
  opacity:0.8;
}
button.sutil.inactive:hover{
  background:transparent;
  outline:none;
  opacity:0.8;
}
button.sutil.inactive:active{
  background:transparent;
  outline:none;
  opacity:0.8;
}
```

#### Small

<button class="small sutil">
Click me
</button>

#### Medium

<button class="medium sutil">
Click me
</button>

#### Big

<button class="big sutil">
Click me
</button>

#### Ícono

<button class="sutil">
<i></i>
</button>

#### Ícono y texto

<button class="sutil">
<i></i><span>Click me</span>
</button>

#### Inactivo

<button class="inactive sutil">
Click me
</button>
¿Cuándo se usa?
---------------

Cuándo se necesita un llamado a una acción.

¿Cómo se usa?
-------------

-   Mantener un verbo en su etiqueta, que invite a la acción que se
    quiere al hacer clic en el botón.
-   Debe existir una respuesta de interacción al usuario (La apariencia
    del botón cambia de acuerdo a su estado)
-   Se debe jerarquizar a través de su color o su tamaño, dependiendo la
    importancia de su acción respecto a los demás botones.
-   Debe ser consistente (ej Si se definen botones de borde rectangular,
    todos deben ser así)
-   Para dispositivos móviles el tamaño mínimo en mm debe ser 10x10mm

Referencias
-----------

-   <https://www.smashingmagazine.com/2009/10/call-to-action-buttons-examples-and-best-practices/>
-   <https://www.smashingmagazine.com/2016/11/the-golden-rules-of-mobile-navigation-design/>
-   <https://www.smashingmagazine.com/2016/11/a-quick-guide-for-designing-better-buttons/>

RadioButton list
================

Descripción
-----------

```html
<ul class="radio-list">
    <li><label><input type="radio">Opción número uno</label></li>
    <li><label><input type="radio">Opción número dos</label></li>
    <li><label><input type="radio">Opción número tres</label></li>
    <li><label><input type="radio">Opción número cuatro</label></li>
</ul>
```

```css
ul.radio-list li{
    list-style:none;
}
```

<ul class="radio-list">
    <li><label><input type="radio">Opción número uno</label></li>
    <li><label><input type="radio">Opción número dos</label></li>
    <li><label><input type="radio">Opción número tres</label></li>
    <li><label><input type="radio">Opción número cuatro</label></li>

</ul>

¿Cuándo se usa?
---------------

-   Cuando se tiene una lista de dos o más opciones que son mutuamente
    excluyentes y el usuario debe elegir una única opción.
-   Cuando se pueda usar en lugar de una lista desplegable. Al mostrar
    todas las opciones, se minimiza la carga cognitiva al usuario.

¿Cómo se usa?
-------------

-   Los grupos de opciones deben estar claramente separados de
    otros grupos.
-   En lo posible, se deben listar las opciones verticalmente, con una
    opción por línea. Si es necesario listarlas horizontalmente, se
    deben mostrar de tal manera que sea evidente a qué etiqueta le
    corresponde cada radio button.
-   Se deben mostrar con una opción seleccionada por defecto. Si el
    usuario requiere abstenerse de elegir alguna de las opciones, se
    debe incluir una opción “Ninguna” o equivalente.
-   Las opciones deben ser claramente diferenciables. Si el usuario no
    sabe a ciencia cierta cuál de las opciones es la más relevante en su
    caso se debe ofrecer la opción “Otro”.
-   La etiqueta de cada radio button también debe ser clickeable.
-   NO se debe usar como control que genera una acción.
