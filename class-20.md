/// JS Templates ///
Template Strings/Literals:
- with regular strings, "\n" for new line or multi-line strings
    - with template strings, any whitespace betw backticks is part of string
- string substitution w/ placeholders ${expression}
- functions inside expressions
- can access props from an object inside placeholder syntax

/// Array .forEach /// - only works on arrays
- forEach() method executes a function once for each array; a method on the array prototype

//const array1 = ['a', 'b', 'c'];

/* array1.forEach(element => console.log(element));

// expected output: "a"
// expected output: "b"
// expected output: "c"

arr.forEach(callback(currentValue[, index[, array]]) {
  // execute something
}[, thisArg]); /*

- Parameters :
    - callback = function to execute on each ele (can take 3 args)
        - currentValue = value of ele
        - index = of ele 
        - array = array forEach() was called upon
    - thisArg = Value to use when executing callback
    - always return undefined
    - used to execute side effects

Converting a for loop to forEach:
/* const items = ['item1', 'item2', 'item3']
const copyItems = []

// before
for (let i = 0; i < items.length; i++) {
  copyItems.push(items[i])
}

// after
items.forEach(function(item){
  copyItems.push(item)
}) /*