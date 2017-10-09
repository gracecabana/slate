
# Date input

## Descripción

```html
<div class="date-input">
	<div class="date-campo">
        <label>Día</label>
        <input type="number">
    </div>
    <div class="date-campo">
        <label>Mes</label>
        <input type="number">
    </div>
    <div class="date-campo">
        <label>Año</label>
        <input type="number">
    </div>
    <div class="date-campo">
    	<button><i></i></button>
    </div>
</div>
```

```css
.date-input{
	float:left;
}
.date-campo{
	float:left;
}
.date-campo input{
	width:30px;
}
.date-campo button i{
	width:15px;
	height:15px;
	display:inline-block;
	background:url(../svg/icon-calendar.svg) no-repeat 50% 50%;
	background-size:100% auto;
}
```

<div class="date-input">
	<div class="date-campo">
        <label>Día</label>
        <input type="number">
    </div>
    <div class="date-campo">
        <label>Mes</label>
        <input type="number">
    </div>
    <div class="date-campo">
        <label>Año</label>
        <input type="number">
    </div>
    <div class="date-campo">
    	<button><i></i></button>
    </div>
</div>

## ¿Cuándo se usa?
Cuando se requiere el ingreso de una fecha por parte del usuario.

## ¿Cómo se usa?
* Se debe evitar mostrar opciones de fechas inválidas o ilógicas.
* Incluso cuando se ofrece un componente gráfico para ingresar la fecha, se debe permitir el ingreso a modo de texto de la misma.
* Se debe mostrar un formato de guía.
* Debe ser lo suficientemente flexible para interpretar modificaciones del formato sugerido. Por ejemplo, separadores de otro tipo (“04-05-2018” en lugar de “04/05/2018”) o valores para día y mes de un único dígito sin cero a la izquierda (“4/5/2018”) deben ser válidos.
* En caso de presentarse un error humano, se debe informar de manera clara qué está mal y cómo solucionarlo.
* Si el público objetivo es global, el formato debe ser especialmente claro, facilitando la identificación de los parámetros que corresponden a día y mes como se ilustra a continuación.
<<<<<<< HEAD

* El uso de los nombres de los meses puede ayudar a facilitar esta identificación.
* En caso que las opciones de fechas sean pocas, se pueden mostrar a modo de lista seleccionable (Ej.: Hoy, mañana, pasado mañana).


=======
![alt text](../images/dateinput1.png "Parámetros separados")
* El uso de los nombres de los meses puede ayudar a facilitar esta identificación.
* En caso que las opciones de fechas sean pocas, se pueden mostrar a modo de lista seleccionable (Ej.: Hoy, mañana, pasado mañana).

>>>>>>> d80c180c88e8a894e0cabdfd43c60181271c1edd
## Referencias
* <https://www.nngroup.com/articles/date-input/>
