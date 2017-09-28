[//]: # (Documentación Botón)
# 1. Botón

## 1.1. Descripción
Existen tres tipos de botones, cada uno puede trabajarse en tres tamaños distintos y cada uno tiene diferentes estados, estas características deben ser transversales sin importar los estilos que se usen para personalizarlos.
Lo anterior se puede dividir en dos grupos: “Botones Evidentes” y “Botones Sutiles”. 

## 1.1.1. Botones evidentes
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
<button class="small">Click me</button>

#### Medium
<button class="medium">Click me</button>

#### Big
<button class="big">Click me</button>

#### Ícono y texto
<button><i></i><span>Click me</span></button>

#### Inactivo
<button class="inactive">Click me</button>


## 1.1.2. Botones sutiles
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
<button class="small sutil">Click me</button>

#### Medium
<button class="medium sutil">Click me</button>

#### Big
<button class="big sutil">Click me</button>

#### Ícono
<button class="sutil"><i></i></button>

#### Ícono y texto
<button class="sutil"><i></i><span>Click me</span></button>

#### Inactivo
<button class="inactive sutil">Click me</button>

## 1.2. ¿Cuándo se usa?
Cuándo se necesita un llamado a una acción.

## 1.3. ¿Cómo se usa?
* Mantener un verbo en su etiqueta, que invite a la acción que se quiere al hacer clic en el botón.
* Debe existir una respuesta de interacción al usuario (La apariencia del botón cambia de acuerdo a su estado)
* Se debe jerarquizar a través de su color o su tamaño, dependiendo la importancia de su acción respecto a los demás botones.
* Debe ser consistente (ej Si se definen botones de borde rectangular, todos deben ser así)
* Para dispositivos móviles el tamaño mínimo en mm debe ser 10x10mm

## 1.4. Referencias
* <https://www.smashingmagazine.com/2009/10/call-to-action-buttons-examples-and-best-practices/>
* <https://www.smashingmagazine.com/2016/11/the-golden-rules-of-mobile-navigation-design/>
* <https://www.smashingmagazine.com/2016/11/a-quick-guide-for-designing-better-buttons/>
