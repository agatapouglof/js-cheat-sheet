# Array manipulations

- get the lentgth of an array ==> arr.length 
- you can do arr.length = i to reduce the array to length i **
- On peut reduire la taille d'un tableau en modifiant la valeur de sa proprite length a une valeur plus petite **

## Array declaration
```js
    var arr = []; // empty array
    var arr = ['daniel', 2, true, {name:'daniel', username : 'agatapouglof'}]; //  array containing differents types of elements
```

## Iteration through an array

### Iteration IN (by index)
```js
    var arr = [2,4,6];
    for(idx in arr){
        console.log("index : " + idx + " value ==> " + arr[idx ]); //index : 0 value ==> 2 ...
    }
```

### Iteration OF (by element)
```js
    var arr = [2,4,6];
    for(elt of arr){
        console.log(elt); // 2,4,6
    }
```

## Add element to array

### add element to the end of the array '.PUSH'
- this function return the length of the new array

```js
    var arr = [];
    arr.push(1); // ==> [1]
    arr.push(2,3,6); // ==> [1,2,3,6]
```

### add element to the beginning of the array '.UNSHIFT'
- this function return the length of the new array

```js
    var arr = [];
    arr.unshift(1); // ==> [1]
    arr.unshift(2,3,6); // ==> [2,3,6,1]
```

## Remove element from array

### revome the last the array '.POP'
- this function return the last element of the array

```js
    var arr = [1,2,3,6];
    arr.pop(); // ==> [1,2,3]
```

### revome first element of the array '.SHIFT'
- this function return the first element of the array

```js
    var arr = [1,2,3,6];
    arr.shift(); // ==> [2,3,6]
```