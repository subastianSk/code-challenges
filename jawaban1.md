`// 01-check-string-blank-or-not.md
        is_Blank =  function(input) {
                if (input.length === 0)
                return true;
                else 
                return false;
              }
        console.log(is_Blank(''));
        console.log(is_Blank('abc'));`

`// 02-string-from-number-range.md
        truncate_string = function (str1, length) {

            if ((str1.constructor === String) && (length>0)) {
                return str1.slice(0, length);
            }
        };
        console.log(truncate_string("Terra Skilvul",5));`

//03-is-it-numeric.md

`// 04-capitalize-phrase.md
        capitalize = function(str1){
          return str1.charAt(0).toUpperCase() + str1.slice(1);
        }

         console.log(capitalize('javascript adalah sebuah bahasa pemrograman yang sangat powerful'));`

`// 05-text-truncate.md
 text_truncate = function(str, length, ending) {
    if (length == null) {
      length = 100;
    }
    if (ending == null) {
      ending = '...';
    }
    if (str.length > length) {
      return str.substring(0, length - ending.length) + ending;
    } else {
      return str;
    }
  };
console.log(text_truncate('We are doing JS string exercises.'))
console.log(text_truncate('We are doing JS string exercises.',19))
console.log(text_truncate('We are doing JS string exercises.',15,'!!'))`
