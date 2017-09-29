[//]: # (Documentación Menu select)
# Menu select

## Descripción

```html
<select>
  <option>Seleccionar...</option>
  <option>Uno</option>
    <option>Dos</option>
    <option>Tres</option>
</select>
```

```css
select:focus{
  outline:none;
}
```

<select>
  <option>Seleccionar...</option>
  <option>Uno</option>
    <option>Dos</option>
    <option>Tres</option>
</select>

## ¿Cuándo se usa?
Se utiliza para permitir seleccionar al usuario una opción de una lista. Mediante una lista desplegable de opciones se permite una mejor organización de la información y se lleva al usuario a centrarse en la acción requerida. 

## ¿Cómo se usa?
* Se recomienda que la lista de opciones utilizada en este componente sea superior a 5 e inferior a 20.
* En el caso de que la lista de opciones sea inferior a 5 se recomienda utilizar radiobuttons
* En el caso que la lista sea superior a 20 se recomienda utilizar un campo de texto con la opción de “autocomplete”
* Se deben agrupar las correctamente las opciones del menú si estas llegan a presentar algún tipo de jerarquía o categorización para facilitar la lectura y posterior acción al usuario.
* Los menús de selección pueden ser utilizados para navegación siempre y cuando cada opción de la lista lleve a una página nueva.

## Referencias
* <http://uxmovement.com/forms/stop-misusing-select-menus/>
