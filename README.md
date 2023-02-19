# Checkers.js
JavaScript checkers library for generating/validating checkers moves, placing/moving pieces, and detecting win/draw.

## Example Code
The code below plays a complete game of checkers randomly.

```js
var checkers = new Checkers();
while (!checkers.in_game_over()) {
  var moves = checkers.moves();
  var move = moves[Math.floor(Math.random() * moves.length)];
  checkers.move(move);
}
console.log(checkers.fen());
```
