1. Construct a function intersection that compares input arrays and returns a new array with elements found in all of the inputs. You can only use reduce method to do this.

```js
function intersection(arrays) {
     return arrays.reduce((current, next) => {
        const filtered = []
        next.forEach((el) => {
            if(current.includes(el)) filtered.push(el)
        })
        return filtered
    }) 
}

// Test
console.log(
  intersection(
    [5, 10, 15, 20],
    [15, 88, 1, 5, 7],
    [1, 10, 15, 5, 20]
  )
); // should log: [5, 15]
```

2. Construct a function `union` that compares input arrays and returns a new array that contains all elements. If there are duplicate elements, only add it once to the new array. Preserve the order of the elements starting from the first element of the first input array. You can only use reduce method to do this.

```js
function union(arrays) {
 // setting output to array
      const output = [] 
     // initial value is of accumulator is an object 
      reduce(arrays,function(acc,currentArray){ 
     // for each item check if item exist in accumulator(object)
            forEach(currentArray,function(item){
     // if it does 
              if(item in acc) {
      // increment its value 
                        acc[item]++
              }else {
       // else  make it a property of accumulator(object) and set value to 1  
                acc[item] = 1;
              }
       // if accumulator property of current item is === length of arrays i.e appears once  
              if(acc[item] === 1){
       //  push item onto output 
                output.push(item)
        }
            })
        // returns accumulator into reduce function
        return acc
        },{})
     //returns output as the union
     return output
    }

// Test
console.log(
  union([5, 10, 15], [15, 88, 1, 5, 7], [100, 15, 10, 1, 5])
);
// should log: [5, 10, 15, 88, 1, 7, 100]
```
