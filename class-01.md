## JavaScript Array map() Method
- The ***map*()** method creates a ***new*** array with the results of calling a function for *every array element*, the **map()** method calls the provided function once for each element in an array, in order,  
- the map() does not execute the function for array elements **without values**.  

 ## JavaScript Array reduce() Method
                   
- The ***reduce*()** method reduces the array to a **single value**, the **reduce()** method executes a provided function *for each value* of the array.
-  reduce() does not execute the function for array elements **without values** (*same as ***map*()** method*). 
##  code snippets 
1. **With normal Promise .then() syntax**:

```
function functionHandler(req, res) {
    let url = `valid URL`
    superagent.get(url)
        .then(data => {
            let X = data.body.map(val => {
                return new Y(val);
            })
        })
}
```
2. **With async / await syntax**:
```
async function functionHandler() {
   let data = await GetSomeData()
   //  code to handle data
}
getData()
.catch(err => console.erorr(err));
```
## promises explain:
-  Promises are a pattern that helps with one particular kind of asynchronous programming, a function that returns a single result asynchronously.
- In other words the Promises is like this 'hey browser you can run all the codes lines and when you done Promise y that you will retun to me'



