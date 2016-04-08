# Prototype

``` javascript
function Piece() {
  // Code
}
Piece.prototype.move = function () {
  console.log('move piece');
}

function Pawn() {
  // Code
}
Pawn.prototype = new Piece();
Pawn.prototype.move = function () {
  console.log('move pawn');
}

var piece = new Piece();
var pawn = new Pawn();

piece.move(); // 'move piece'
pawn.move(); // 'move pawn'
```

---