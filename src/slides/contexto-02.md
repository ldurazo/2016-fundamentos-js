# El Contexto de una función

``` javascript
function A() {
  this.x = 1;
}

A(); // El valor de this es window

var obj = new A();
// El new crea un nuevo objeto y regresa este objeto nuevo
// El this este objeto nuevo creado


obj.x; 
// Cuando se usa el punto, el objeto de la derecha es el this
```

---