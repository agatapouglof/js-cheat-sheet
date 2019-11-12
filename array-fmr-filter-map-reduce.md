# Array function FILTER // MAP // REDUCE

## FILTER arr.filter(callbackFuction, thisArg)
this function return a new array respecting the conditions given in callback function
-
callbackFunction(element, index, originalArray) return true or false
- element : element courant du tableau
- index : indice de l'element courant du tableau
- originalArray : tableau de depart sans modification

- thisArg : object to use as this for the callback function

** ne modifie pas le tableau original
```js
    var arr = [1,2,3,4,5,6,7,8];
    var res = arr.filter(function(elt, i, ar){
        return elt % 2 == 0;
    });
    // res ==> [2,4,6,7] 
```

## MAP arr.map(callbackFunction, thisArg)
this function return a new array of element after the call of callback function  on each element 

- callbackFunction(element, index, originalArray) return array 
- element : element courant du tableau
- index : indice de l'element courant du tableau
- originalArray : tableau de depart sans modification

- thisArg : object to use as this for the callback function

```js
    var arr = [1,2,3];
    var res = arr.map(function(elt, i, ar){
        return elt * i;
    });
    // res  ==> [0,2,6]
```

```js
    var nombres = [1, 4, 9];
    var racines = nombres.map(Math.sqrt);
    // racines vaut désormais [1, 2, 3]
```

## REDUCE arr.reduce()
Reduit a un seul element un tableau bon pour les totaux
```js
    let value = array.reduce(function(previousValue, item, index, array) {
    // ...
}, initial);

```
*********************************

```js
    var res = [0, 1, 2, 3, 4].reduce(function(accumulateur, valeurCourante, index, array){
    return accumulateur + valeurCourante;
    }, 10);
    //  res ==> 20
```