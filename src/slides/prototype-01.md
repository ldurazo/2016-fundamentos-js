# Prototype

Cada objeto esta ligado internamente a otro objeto llamado `prototype`

``` javascript
Array.prototype.sum = function () {
  // Fun code
}

[1,2,3].sum(); // fun code happens
```

Cuando agregamos mas variables al `prototype` todas las instancias de esa función pueden acceder a esa nueva variable.

---