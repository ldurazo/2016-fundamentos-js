# El Contexto de una función

`call` y `apply`

``` javacscript
var something = {
  x: 10,

  getCalculator: function () {
    return function () {
      return this.x * this.x;
    }
  },

  init: function () {
    var calculator = this.getCalculator();
    return calculator.apply(this);
  }
}

something.init(); // 100
```

---