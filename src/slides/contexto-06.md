# El Contexto de una función

``` javascript
var obj = {x: 2};
var obj2 = {x: 5};

var calculate = function () {
  return this.x * 10;
}

calculate(); // NaN

var bindCalculate = calculate.bind(obj);
bindCalculate(); // 20
bindCalculate.call(obj2); // 20
```

---