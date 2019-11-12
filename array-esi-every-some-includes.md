# Array function EVERY // SOME // INCLUDES

## EVERY array.every(callbackFunction())
This function checks if all items in an array pass the specified condition in the callback function 
- callbackFunction(value) ==> return true or false
- check callback for all elements in array

```js
    var numbers = [-1,2,4,7];
    var  isAllPositive = numbers.every((value) => {
        return value >= 0;
    });
    // isAllPositive ==> false
```


## SOME array.some(callbackFunction())
This function checks if at least one item in an array pass the specified condition in the callback function 
- callbackFunction(value) ==> return true or false
- .some() function return true or false

```js
    var numbers = [-1,2,4,7];
    var  isatLeastOnePositive = numbers.some((value) => {
        return value >= 0;
    });
    // isatLeastOnePositive ==> true
```

## INCLUDES array.includes(element, startIndex:optional)
This function check if the array contains a certain item starting at a specified index
- return true or false
- Si on utilise une valeur négative, la recherche commencera à partir de la fin du tableau (autrement dit à l'indice array.length - indiceDépart)

```js
    [1, 2, 3].includes(2);     // true
    ['a', 'b', 'c'].includes('c', 5);    // false
    ['a', 'b', 'c'].includes('c', -100); // true
```