# El Contexto de una función

``` javascript
function multiplyBy(num) {
  return this.x * num;
}

var obj = {x: 2;}
var other = {x: 20}

multiplyBy.call(obj, 2); // 4
multitplyBy.call(other, 2); // 40

multiplyBy.apply(obj, [3]); // 6
multiplyBy.apply(other, [3]); // 60
```

---