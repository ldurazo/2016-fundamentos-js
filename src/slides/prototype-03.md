# Prototype

``` javascript
function Connector() {
  // Code
}
Connector.prototype; // Object
Object.protoype; // Object

var c = new Connector
var a = {};

c.prototype; // undefined
a.prototype; // undefined

c.__proto__; // Object
a.__proto__; // Object
```

---