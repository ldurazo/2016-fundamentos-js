# Scope

``` javascript
var a = 1;
(function () {
  // puede ver: a,b,x
  var b;

  function something() {
    // puede ver: a,b,c,x
    var c;

    function whatever() {
      // puede ver: a,b,c,d,x
      var d;
    }

    x = 5;
  }
})();
```

---