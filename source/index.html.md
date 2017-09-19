---
title: API Reference

language_tabs: # must be one of https://git.io/vQNgJ
  - html
  - css
  - javascript

toc_footers:
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/tripit/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true
---

# Introducción

Intro bella redactada por Andy aquí :)

# Botón

## Descripción
Existen tres tipos de botones, cada uno puede trabajarse en tres tamaños distintos y cada uno tiene diferentes estados, estas características deben ser transversales sin importar los estilos que se usen para personalizarlos.
Lo anterior se puede dividir en dos grupos: “Botones Evidentes” y “Botones Sutiles”. 

### Botones evidentes
Que tienen un color de fondo
#### Small
<button class="small">Click me</button>
```html
<button class="small">Click me</button>
```

```css
.small{
	
}
```
#### Ícono y texto
<button><i></i><span>Click me</span></button>
```html
<button><i></i><span>Click me</span></button>
```



### Botones sutiles
Que tienen fondo transparente.

## ¿Cuándo se usa?
Cuándo se necesita un llamado a una acción.

## ¿Cómo se usa?
* Mantener un verbo en su etiqueta, que invite a la acción que se quiere al hacer clic en el botón.
* Debe existir una respuesta de interacción al usuario (La apariencia del botón cambia de acuerdo a su estado)
* Se debe jerarquizar a través de su color o su tamaño, dependiendo la importancia de su acción respecto a los demás botones.
* Debe ser consistente (ej Si se definen botones de borde rectangular, todos deben ser así)
* Para dispositivos móviles el tamaño mínimo en mm debe ser 10x10mm

## Referencias
* https://www.smashingmagazine.com/2009/10/call-to-action-buttons-examples-and-best-practices/
* https://www.smashingmagazine.com/2016/11/the-golden-rules-of-mobile-navigation-design/
* https://www.smashingmagazine.com/2016/11/a-quick-guide-for-designing-better-buttons/

<aside class="notice">
You must replace <code>meowmeowmeow</code> with your personal API key.
</aside>

# Kittens

## Get All Kittens

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.get
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.get()
```

```shell
curl "http://example.com/api/kittens"
  -H "Authorization: meowmeowmeow"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let kittens = api.kittens.get();
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "name": "Fluffums",
    "breed": "calico",
    "fluffiness": 6,
    "cuteness": 7
  },
  {
    "id": 2,
    "name": "Max",
    "breed": "unknown",
    "fluffiness": 5,
    "cuteness": 10
  }
]
```

This endpoint retrieves all kittens.

### HTTP Request

`GET http://example.com/api/kittens`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
include_cats | false | If set to true, the result will also include cats.
available | true | If set to false, the result will include kittens that have already been adopted.

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Get a Specific Kitten

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.get(2)
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.get(2)
```

```shell
curl "http://example.com/api/kittens/2"
  -H "Authorization: meowmeowmeow"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let max = api.kittens.get(2);
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "name": "Max",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```

This endpoint retrieves a specific kitten.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### HTTP Request

`GET http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to retrieve

## Delete a Specific Kitten

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.delete(2)
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.delete(2)
```

```shell
curl "http://example.com/api/kittens/2"
  -X DELETE
  -H "Authorization: meowmeowmeow"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let max = api.kittens.delete(2);
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "deleted" : ":("
}
```

This endpoint retrieves a specific kitten.

### HTTP Request

`DELETE http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to delete

