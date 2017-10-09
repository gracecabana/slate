
# Tooltip

## Descripción
Es una caja pequeña que revela información útil cuando un usuario hace hover sobre un elemento gráfico o etiqueta designada.

```html
<div class="tooltip"><p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor.</p></div>
```

```css
.tooltip{
    width: 300px;
    background-color: #ccc;
    padding: 10px;
}
.tooltip p{
    margin: 0;
}
.tooltip::after{
    content: "";
    width: 16px;
    height: 16px;
    position: relative;
    float: left;
    margin: 10px 0 0 -8px;
    left: 50%;
    border-right:8px solid transparent;
    border-left:8px solid transparent;
    border-top:8px solid #cccccc;
    box-sizing:border-box;
}
.input-tooltip{
    position:relative;
    width:100%;
}
```

<div class="tooltip"><p>Lorem ipsum dolor sit amet, consectetuer adipiscing elit. Aenean commodo ligula eget dolor.</p></div>

## ¿Cuándo se usa?
* Cuando el control no tiene una etiqueta de texto, siendo un botón, icono o etiqueta no descriptiva que necesita una explicación corta para mejor entendimiento del usuario.
* Cuando el control se beneficia de información adicional.
* NO USAR cuando el usuario necesita interactuar con el contenido del tooltip.
* NO USAR en móvil.

## ¿Cómo se usa?
* Deben incluir texto corto, conciso y de ayuda.
* Deben ser ubicados junto al objeto de interés.
* No deben interferir con la acción que el usuario esté haciendo en el momento.
* Deben ser fáciles de descubrir.

## Referencias
* <https://www.usability.gov/what-and-why/glossary/hover-help-or-tool-tiptooltip.html>
* <https://uxplanet.org/tooltips-in-ui-design-f63e117aa3d1>
