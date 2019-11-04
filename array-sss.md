# Array  SPLICE // SLICE // SPLIT

## SPLICE() array.splice()
@params{
    startIndex,
    numberOfElementsToDelete,
    ...lists of elements to add
}
this method add, remove or replace elements of an array depending of the parameters given to the function
### Add with .splice();
```js
    var arr = [1,2,3,5,6,'test'];
    var res = arr.splice(2,0,100,101,'me');
    // Explanation :: from Index 2 Delete 0 elements and add 100,101,'me'
    // arr ==> [1,2,100,101,"me",3,5,6,"test"];
    // res ==> undefined :: no return from the function
```

### Delete elements with .splice();
```js
    var arr = [1,2,3,5,6,'test'];
    var res = arr.splice(2,3);
    // Explanation :: from Index 2 Delete 3 elements 
    // arr ==> [1,2,"test"];
    // res ==> [3,5,6];
```

### Replace elements with .splice()
```js
    var arr = [1,2,3,5,6,'test'];
    var res = arr.splice(2,2,30,50);
    // Explanation :: from Index 2 Delete 2 elements and add 30,50 
    // arr ==> [1, 2, 30, 50, 6, "test"]
    // res ==> [3,5]
```

## SLICE arr.slice(startIndex, endIndex) , string.slice(startIndex, endIndex)
this function return a part of an array or a string but not edit the existing array
!! pas de modification sur le tableau ou la chaine de caractere originale
!! endIndex is not included in the returned array
```js
    var arr = [1,2,3,4,5];
    res = arr.slice(1,3);
    //  res ==> [2,3]
    //  arr ==> [1,2,3,4,5]
```
