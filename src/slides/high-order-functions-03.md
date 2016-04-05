# High Order Functions

``` JavaScript
var numbers = [1,2,3,4,5];

var numbersDoubled = numbers.map(function (number) {
  return number * 2;
});

console.log(numbersDoubled); // [2,4,6,8,10]
```

``` javascript
var sum = 0;
[1,2,3,4].forEach(function (num) {
  sum += num;
});
console.log(sum); // 10
```

---