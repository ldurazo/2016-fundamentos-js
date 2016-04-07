# Closure

Usar variables de un scope externo (que ya terminó de ejecutarse) desde cualquier otro scope.

``` javascript
function greaterThan(n) {
  return function(m) { 
    return m > n; 
  };
}
var greaterThan10 = greaterThan(10);
greaterThan10(11); // true
```

---