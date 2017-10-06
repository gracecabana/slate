
# Tabla

## Descripción

```html
<table>
	<thead>    	
          <tr>
            <th>4ner</th>
            <th>Contacto</th>
            <th>Sede</th>
          </tr>
    </thead>
    <tbody>
    	  <tr>
            <td data-th="4ner">Ximena Paola Sánchez</td>
            <td data-th="Contacto">ximenasanchez@seven4n.com</td>
            <td data-th="Sede">Bogotá</td>
          </tr>
          <tr>
            <td data-th="4ner">Sandra Robayo</td>
            <td data-th="Contacto">sandrarobayo@seven4n.com</td>
            <td data-th="Sede">Bogotá</td>
          </tr>
          <tr>
            <td data-th="4ner">Juan Carlos Alfonso Garzón </td>
            <td data-th="Contacto">juancarlosalfonso@seven4n.com</td>
            <td data-th="Sede">Bogotá</td>
          </tr>
          <tr>
            <td data-th="4ner">Laura Marcela Camacho Vásquez</td>
            <td data-th="Contacto">lauracamacho@seven4n.com</td>
            <td data-th="Sede">Medellín</td>
          </tr>
          <tr>
            <td data-th="4ner">Carlos Zuluaga</td>
            <td data-th="Contacto">carloszuluaga@seven4n.com</td>
            <td data-th="Sede">Medellín</td>
          </tr>
          <tr>
            <td data-th="4ner">Ronnie Dave Cañas Pineda</td>
            <td data-th="Contacto">ronniecanas@seven4n.com</td>
            <td data-th="Sede">Medellín</td>
          </tr>
    </tbody>
</table>
```

```css
table {
    border-collapse: collapse;
    width: 100%;
    font-size:0.8em;
}

td, th {
    border: 1px solid #dddddd;
    text-align: left;
    padding: 8px;
}

tr:nth-child(even) {
    background-color: #ededed;
}
@media (max-width: 991px){
	table, thead, tbody, td, tr { 
		display: block;
		text-align:left; 
	}
	table thead tr { 
		position: absolute;
		top: -9999px;
		left: -9999px;
	}
	table td { 
		border: none;
		border-bottom: 1px solid #d8d9dd; 
		position: relative;
		padding-left: 50%; 
	}	
	table td:before { 
		position: absolute;
		left: 10px;
		width: 45%; 
		padding-right: 10px;
		font-weight:bold; 
	}
	table td::before { 
		content: attr(data-th)": ";
	}
}
```

<table>
	<thead>    	
          <tr>
            <th>4ner</th>
            <th>Contacto</th>
            <th>Sede</th>
          </tr>
    </thead>
    <tbody>
    	  <tr>
            <td data-th="4ner">Ximena Paola Sánchez</td>
            <td data-th="Contacto">ximenasanchez@seven4n.com</td>
            <td data-th="Sede">Bogotá</td>
          </tr>
          <tr>
            <td data-th="4ner">Sandra Robayo</td>
            <td data-th="Contacto">sandrarobayo@seven4n.com</td>
            <td data-th="Sede">Bogotá</td>
          </tr>
          <tr>
            <td data-th="4ner">Juan Carlos Alfonso Garzón </td>
            <td data-th="Contacto">juancarlosalfonso@seven4n.com</td>
            <td data-th="Sede">Bogotá</td>
          </tr>
          <tr>
            <td data-th="4ner">Laura Marcela Camacho Vásquez</td>
            <td data-th="Contacto">lauracamacho@seven4n.com</td>
            <td data-th="Sede">Medellín</td>
          </tr>
          <tr>
            <td data-th="4ner">Carlos Zuluaga</td>
            <td data-th="Contacto">carloszuluaga@seven4n.com</td>
            <td data-th="Sede">Medellín</td>
          </tr>
          <tr>
            <td data-th="4ner">Ronnie Dave Cañas Pineda</td>
            <td data-th="Contacto">ronniecanas@seven4n.com</td>
            <td data-th="Sede">Medellín</td>
          </tr>
    </tbody>
</table>

## ¿Cuándo se usa?
Cuando se deba presentar al usuario un “set” de datos agrupados y relacionados, permitiendo analizar, comparar, filtrar y organizar de una manera rápida y sencilla.

## ¿Cómo se usa?
* Los datos se deben agrupar por columnas.
* Cada columna debe tener la propiedad de ordenar de manera ascendente o descente alfanumérico.
* El orden de las columnas de izquierda a derecha, deben estar organizadas de manera que el usuario pueda leer los datos fácilmente.
* El estilo gráfico debe permitir al usuario diferenciar claramente entre título de columna y contenido de celda.
* Se deben tener en cuenta la cantidad de datos presentados al usuario al momento de incluir paginado de datos.
* Se debe permitir al usuario ajustar el orden y tamaño de las columnas.
* El título de columna debe ser presentado en una sola línea de texto y con la cantidad mínima de palabras posibles, se recomienda 2 palabras máximo.
* Las acciones relacionadas con la información dispuesta (descargar, filtrar, imprimir, etc) en la tabla, deben estar ubicadas de manera visible y de fácil acceso al usuario sin interferir con la lectura de la información.
* Se deben evitar acciones redundantes en el contenido de la tabla, es decir, varias columnas con link a un mismo lugar del sistema.


## Referencias
* <https://uxdesign.cc/design-better-data-tables-4ecc99d23356>
* <https://uxdesign.cc/designing-better-tables-for-enterprise-applications-f9ef545e9fbd>