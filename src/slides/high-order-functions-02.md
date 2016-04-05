# High Order Functions

``` javascript
function doSomething() {
  return 'I do something';
}

function other(callback) {
  return callback();
}

other(doSomething); // return 'I do something'

other(function () {
  return 'I do other thing';
}); // Return 'I do other thing'

var result = other(function () {
  return function () {
    console.log('inception');
  }
});
result(); // prints 'inception'
```

---