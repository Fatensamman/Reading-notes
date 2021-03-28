## Node Ecosystem, TDD, CI/CD

* `Array.map()`:

- It's a process that takes a callback method and does an operation on the array's elements by calling a function of array elements. It returns a new array with the values obtained by performing the operation on each element. 

```
let numbers = [1, 4, 9];
let roots = numbers.map(function(num) {
    return Math.sqrt(num);
});
// roots is now     [1, 2, 3]
// numbers is still [1, 4, 9]
```

* `Array.reduce()`:
- The arr.reduce() method in JavaScript is used to reduce an array to a single value by running a given function for each array value (from left to right) and saving the function's return value in an accumulator.

```
[0, 1, 2, 3, 4].reduce((accumulator, currentValue, currentIndex, array) => {
   accumulator+=currentValue;
 return accumulator;
}, 0);
// it will return 10 
```

* `superagent.get()`:

- with `.then()`:
```
 function data(req,res){
    superagent.get(url).then(result=>{
        res.send(result.body);
      });
    };
```
- with async / await
```
async function data(req,res){
        let result = await superagent.get(url);
        res.send(result);
    };
```

* Promises:
A promise is an object that may produce a single value some time in the future: either a resolved value, or a reason that it’s not resolved. A promise may be in one of 3 possible states: fulfilled, rejected, or pending. Promise users can attach callbacks to handle the fulfilled value or the reason for rejection.

* Are all callback functions considered to be Asynchronous?
No, For example there's forEach in Array. It iterates over each item and calls the function once per item.
