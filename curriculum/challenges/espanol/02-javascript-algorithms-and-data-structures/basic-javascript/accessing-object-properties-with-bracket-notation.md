---
id: 56533eb9ac21ba0edf2244c8
title: Accede a propiedades de objetos con notación de corchete
challengeType: 1
videoUrl: 'https://scrimba.com/c/cBvmEHP'
forumTopicId: 16163
dashedName: accessing-object-properties-with-bracket-notation
---

# --description--

La segunda manera de acceder a las propiedades de un objeto es con la notación de corchete (`[]`). Si la propiedad del objeto al que intentas acceder tiene un espacio en el nombre, necesitarás usar notación de corchete.

Sin embargo, también puedes utilizar la notación de corchete en propiedades de un objeto sin espacios.

Aquí hay un ejemplo de cómo usar la notación de corchete para leer la propiedad de un objeto:

```js
var myObj = {
  "Space Name": "Kirk",
  "More Space": "Spock",
  "NoSpace": "USS Enterprise"
};
myObj["Space Name"]; // Kirk
myObj['More Space']; // Spock
myObj["NoSpace"];    // USS Enterprise
```

Ten en cuenta que los nombres de las propiedades con espacios deben estar entre comillas (simples o dobles).

# --instructions--

Lee los valores de las propiedades `"an entree"` y `"the drink"` de `testObj` usando la notación de corchete y asígnalos a `entreeValue` y `drinkValue` respectivamente.

# --hints--

`entreeValue` debe ser una cadena de texto

```js
assert(typeof entreeValue === 'string');
```

El valor de `entreeValue` debe ser `"hamburger"`

```js
assert(entreeValue === 'hamburger');
```

`drinkValue` debe ser una cadena de texto

```js
assert(typeof drinkValue === 'string');
```

El valor de `drinkValue` debe ser `"water"`

```js
assert(drinkValue === 'water');
```

Debes usar la notación de corchete dos veces

```js
assert(code.match(/testObj\s*?\[('|")[^'"]+\1\]/g).length > 1);
```

# --seed--

## --after-user-code--

```js
(function(a,b) { return "entreeValue = '" + a + "', drinkValue = '" + b + "'"; })(entreeValue,drinkValue);
```

## --seed-contents--

```js
// Setup
var testObj = {
  "an entree": "hamburger",
  "my side": "veggies",
  "the drink": "water"
};

// Only change code below this line

var entreeValue = testObj;   // Change this line
var drinkValue = testObj;    // Change this line
```

# --solutions--

```js
var testObj = {
  "an entree": "hamburger",
  "my side": "veggies",
  "the drink": "water"
};
var entreeValue = testObj["an entree"];
var drinkValue = testObj['the drink'];
```
