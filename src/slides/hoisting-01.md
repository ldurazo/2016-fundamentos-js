# Hoisting

Es el comportamiendo de mover las declaraciones al inicio del scope (global o de la función actual).

De esta forma podemos usar la función o variable antes de que sea declarada.

``` javascript
foo = 2;
var foo;

// Es implicitamente entendido como:

var foo;
foo = 2;
```

``` javascript
hoisted(); // imprime "foo"

function hoisted() {
  console.log("foo");
}
```

---