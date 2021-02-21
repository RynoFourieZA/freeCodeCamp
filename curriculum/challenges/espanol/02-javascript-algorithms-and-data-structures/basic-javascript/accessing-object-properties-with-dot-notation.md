---
id: 56533eb9ac21ba0edf2244c7
title: Accede a propiedades de objetos con notación de punto
challengeType: 1
videoUrl: 'https://scrimba.com/c/cGryJs8'
forumTopicId: 16164
dashedName: accessing-object-properties-with-dot-notation
---

# --description--

Hay dos maneras de acceder a las propiedades de un objeto: notación de punto (`.`) y notación de corchete (`[]`), similar a un arreglo.

La notación de punto es lo que se usa cuando conoces el nombre de la propiedad a la que intentas acceder con antelación.

Aquí hay un ejemplo de cómo usar la notación de punto (`.`) para leer la propiedad de un objeto:

```js
var myObj = {
  prop1: "val1",
  prop2: "val2"
};
var prop1val = myObj.prop1; // val1
var prop2val = myObj.prop2; // val2
```

# --instructions--

Lee los valores de las propiedades de `testObj` utilizando la notación de punto. Asigna la variable `hatValue` igual a la propiedad `hat` del objeto y asigna la variable `shirtValue` igual a la propiedad `shirt` del objeto.

# --hints--

`hatValue` debe ser una cadena

```js
assert(typeof hatValue === 'string');
```

El valor de `hatValue` debe ser `"ballcap"`

```js
assert(hatValue === 'ballcap');
```

`shirtValue` debe ser una cadena

```js
assert(typeof shirtValue === 'string');
```

El valor de `shirtValue` debe ser `"jersey"`

```js
assert(shirtValue === 'jersey');
```

Debes usar la notación de punto dos veces

```js
assert(code.match(/testObj\.\w+/g).length > 1);
```

# --seed--

## --after-user-code--

```js
(function(a,b) { return "hatValue = '" + a + "', shirtValue = '" + b + "'"; })(hatValue,shirtValue);
```

## --seed-contents--

```js
// Setup
var testObj = {
  "hat": "ballcap",
  "shirt": "jersey",
  "shoes": "cleats"
};

// Only change code below this line

var hatValue = testObj;      // Change this line
var shirtValue = testObj;    // Change this line
```

# --solutions--

```js
var testObj = {
  "hat": "ballcap",
  "shirt": "jersey",
  "shoes": "cleats"
};

var hatValue = testObj.hat;
var shirtValue = testObj.shirt;
```
