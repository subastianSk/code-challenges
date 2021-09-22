//01-random-integer.md
  rand = function(min, max) {
    if (min==null && max==null)
      return 0;    

    if (max == null) {
        max = min;
        min = 0;
      }
      return min + Math.floor(Math.random() * (max - min + 1));
    };
   console.log(rand(20,1));
   console.log(rand(1,10));
   console.log(rand(6));
   console.log(rand());

//02-choose-your-decimal.md
  function decimals(n, d) {
   if ((typeof n !== 'number') || (typeof d !== 'number'))
     return false;
        n = parseFloat(n) || 0;
    return n.toFixed(d);
    }
  console.log(decimals(2.100212, 2));
  console.log(decimals(2.100212, 3));
  console.log(decimals(2100, 2));


// 03-is-it-numeric.md
function isItNumeric(num) {
  return !isNaN(parseFloat(num)) && isFinite(num);
}

console.log(isItNumeric(12));
console.log(isItNumeric('abcd'));
console.log(isItNumeric('12'));
console.log(isItNumeric(' '));
console.log(isItNumeric(1.20));
console.log(isItNumeric(-200));
