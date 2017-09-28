
# RadioButton list

## Descripción

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

## ¿Cuándo se usa?
* Cuando se tiene una lista de dos o más opciones que son mutuamente excluyentes y el usuario debe elegir una única opción.
* Cuando se pueda usar en lugar de una lista desplegable. Al mostrar todas las opciones, se minimiza la carga cognitiva al usuario.

## ¿Cómo se usa?
* Los grupos de opciones deben estar claramente separados de otros grupos.
* En lo posible, se deben listar las opciones verticalmente, con una opción por línea. Si es necesario listarlas horizontalmente, se deben mostrar de tal manera que sea evidente a qué etiqueta le corresponde cada radio button.
* Se deben mostrar con una opción seleccionada por defecto. Si el usuario requiere abstenerse de elegir alguna de las opciones, se debe incluir una opción “Ninguna” o equivalente.
* Las opciones deben ser claramente diferenciables. Si el usuario no sabe a ciencia cierta cuál de las opciones es la más relevante en su caso se debe ofrecer la opción “Otro”.
* La etiqueta de cada radio button también debe ser clickeable.
* NO se debe usar como control que genera una acción. 

##Referencias
<https://www.nngroup.com/articles/checkboxes-vs-radio-buttons/>
