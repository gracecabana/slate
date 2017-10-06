
# Validación

## Descripción
Manera en que se informa al usuario que ha ingresado valores incorrectos en uno o más campos de un formulario, que no ha diligenciado campos obligatorios o que diligenció con valores diferentes los campos de confirmación (ej.: "Confirme contraseña"). Igualmente, para darle tranquilidad al usuario, se puede confirmar que se diligenciaron correctamente con color verde.


```html
<div class="input-error">
    <label>Etiqueta</label>
    <input type="text">
    <span>Completar este campo</span>
</div>

<div class="input-validado">
    <label>Etiqueta</label>
    <input type="text"><i></i>
</div>
```

```css
.input-validado{
    position:relative;
    width:200px;
}
.input-validado input{
    width:100%;
    border:solid 1px #00dd00;
}
.input-validado i{
    width:15px;
    height:15px;
    display:inline-block;
    background:url(../svg/icon-validado.svg) no-repeat 50% 50%;
    background-size:100% auto;
    float:right;
    margin-right:-20px;
    margin-top:-20px;   
}
.input-error{
    position:relative;
    width:200px;
}
.input-error input{
    width:100%;
    border:solid 1px #dd0000;
}
.input-error span{
    color:#dd0000;
    float:right;
    text-align:right;
    font-size:0.7em;
}
```

<div class="input-error">
    <label>Etiqueta</label>
    <input type="text">
    <span>Completar este campo</span>
</div>

<div class="input-validado">
    <label>Etiqueta</label>
    <input type="text"><i></i>
</div>

## ¿Cuándo se usa?
Se debe mostrar un error por cada campo del formulario en el momento que se interactúa con el elemento.

## ¿Cómo se usa?
* En primer lugar se deben ofrecer pistas para minimizar los errores, esto se logra marcando los campos obligatorios y usando placeholders para evidenciar el formato deseado.
* Se debe resaltar el campo errado con un mensaje en línea, un marcador de error junto al campo, resaltando el campo, cambiando el color de la etiqueta del campo o mostrando el mensaje de error en un tool-tip.
* Se debe elegir por lo menos uno de los elementos anteriores y usar color rojo para resaltar los errores. 
* La validación se debe hacer del lado del cliente antes de enviar el formulario, cuando un campo pierde el foco (real time validation).
* Se pueden mostrar sugerencias mientras se diligencia un campo para evitar errores.



## Referencias
* <https://www.smashingmagazine.com/2009/07/web-form-validation-best-practices-and-tutorials/>
