# Prototype Chain

``` javascript
function A() {
  this.x = 1;
}
A.prototype.sum = function () { return 20; }

function B() {
  this.y = 2;
}
B.prototype = new A();

var b = new B();

b.y; // 2
b.x; // 1
b.sum; // 20
b.toString(); // [object Object]
b.noExists(); // undefined
```

---