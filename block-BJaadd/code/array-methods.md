Watch this video to understand what to do in this exercise block [link](https://www.youtube.com/watch?v=zGpplZj4zY0&feature=youtu.be)

## Getting To Know Array Methods

Go to this [link](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) and look for the name of method to learn about it.

**Write in your own way of understanding (don't copy paste)**

Only if you are done with step 1 you should go ahead.

1. Practice it by yourself in console (2-3 times to understand)
2. Data types of parameters
3. Return value type
4. Write three examples
5. In your words what this method does.
6. Does it mutate the original value or not (check https://doesitmutate.xyz)

Example:

1. `concat`

   - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)
   - Return: a single Array consisting of by all the values passed as parameters in the same order.
   - Example:
     ```js
     let numbers = [1, 2, 3];
     numbers.concat(4); //[1,2,3,4]
     let sentanceArray = 'A quick brown fox jumped over a lazy'.split(' ');
     sentanceArray.concat('dog').join(' '); //"A quick brown fox jumped over a lazy dog"
     let colors = ['red', 'green', 'blue'];
     colors.concat('black', 'red', 21, true); // ['red','green','blue','black', 'red', 21, true]
     ```
   - `concat` accepts n number of values and returns one array with all the values in same order. It does not change the original array.
   - No it does not mutate the original array

2. `join`
   - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)the array elements are separated with a comma (","). If separator is an empty string, all elements are joined without any characters in between them.
   - Return: A string with all array elements joined. If arr.length is 0, the empty string is returned.

   - Example:
     ```js
     let colors = ["blue","orange","yellow","purple"];
     colors.join(); //'blue,orange,yellow,purple'
     let sentanceArray = 'An Elephant throw away all the'.split(' ');
     sentanceArray.concat('tree').join(' '); //'An Elephant throw away all the tree'
     let cities = ['solapur', 'pune', 'mumbai','nagpur'];
     colors.join('-'); // 'blue-orange-yellow-purple'
     ```
   - `concat` accepts n number of values and returns A string with all array elements joined. It does not change the original array.
   - No it does not mutate the original array

3. `flat`
   - Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)(depth) optional--The depth level specifying how deep a nested array structure should be flattened. Defaults to 1.

   - Return: A new array with the sub-array elements concatenated into it.

   - Example:
     ```js
     let numbers = [1,2,[3,4,[5,6,[7,8]]]];
     numbers.flat(); //(5) [1, 2, 3, 4, Array(3)]
     numbers.flat(2); //(7) [1, 2, 3, 4, 5, 6, Array(2)]
     numbers.flat(4); //(8) [1, 2, 3, 4, 5, 6, 7, 8]
     ```
   - `flat` accepts n number of values and returns A new array with the sub-array elements concatenated into it. It does not change the original array.
   - No it does not mutate the original array

4. `push`
   - Parameter: n (element) number of values (number, string, boolean, array, null, undefined, object and function etc)The element(s) to add to the end of the array.

   - Return: The new length property of the object upon which the method was called.

   - Example:
     ```js
     let cities = ['solapur', 'pune', 'mumbai','nagpur'];
     cities.push('delhi'); //(5) ['solapur', 'pune', 'mumbai', 'nagpur', 'delhi']
     cities.push('chennai','asam'); //(7) ['solapur', 'pune', 'mumbai', 'nagpur', 'delhi', 'chennai', 'asam']
     cities.push('uttar pradesh','himachal pradesh','keral'); //(10) ['solapur', 'pune', 'mumbai', 'nagpur', 'delhi', 'chennai', 'asam', 'uttar pradesh', 'himachal pradesh', 'keral']
     ```
   - `push` The element(s) to add to the end of the array and returns The new length property of the object upon which the method was called.
   - It mutate the original array.

5. `indexOf`
   - Parameter: n (element) number of values (number, string, boolean, array, null, undefined, object and function etc)Element to locate in the array.(fromIndex) optional--The index to start the search at. If the index is greater than or equal to the array's length, -1 is returned.

   - Return: The first index of the element in the array; -1 if not found.

   - Example:
     ```js
     let colors = ["blue","orange","yellow","purple"];
     colors.indexOf('purple'); //3
     let numbers = [1,2,3,4,5,6,7,8];
     numbers.indexOf(6); //5
     let cities = ['solapur', 'pune', 'mumbai','nagpur'];
     cities.indexOf('solapur'); //0
     ```
   - `indexOf` Element to locate in the array and returns The first index of the element in the array; -1 if not found.
   - It only finds the index of elements in the  original array.

6. `lastIndexOf`
   - Parameter: n (element) number of values (number, string, boolean, array, null, undefined, object and function etc)Element to locate in the array.(fromIndex) optional--The index to start the search at. If the index is greater than or equal to the array's length, -1 is returned.

   - Return: The last index of the element in the array; -1 if not found.

   - Example:
     ```js
     let colors = ["blue","orange","yellow","purple"];
     colors.lastIndexOf('yellow'); //2
     let numbers = [1,2,3,4,5,6,7,8];
     numbers.lastIndexOf(8); //7
     let cities = ['solapur', 'pune', 'mumbai','nagpur'];
     cities.lastIndexOf('nagpur'); //3
     ```
   - `lastIndexOf` Element to locate in the array and returns The last index of the element in the array; -1 if not found.
   - It only finds the last index of elements in the  original array.

7. `includes`
   - Parameter: n (element) number of values (number, string, boolean, array, null, undefined, object and function etc)Element to locate in the array.(fromIndex) optional--The index to start the search at. If the index is greater than or equal to the array's length, -1 is returned.

   - Return: A boolean value which is true if the value searchElement is found within the array  but false is not considered to be the same as 0.

   - Example:
     ```js
     let colors = ["blue","orange","yellow","purple"];
     colors.includes('blue'); //true
     let numbers = [1,2,3,4,5,6,7,8];
     numbers.includes(5); //true
     let cities = ['solapur', 'pune', 'mumbai','nagpur'];
     cities.includes('kolhapur'); //false
     ```
   - `includes` Element to locate in the array and returns A boolean value which is true if the value searchElement is found within the array  but false is not considered to be the same as 0.

   - It only finds the elements in the original array.

8. `reverse`
   - Parameter: none
   - Return: The reversed array.

   - Example:
     ```js
     let colors = ["blue","orange","yellow","purple"];
     colors.reverse(); //(4) ['purple', 'yellow', 'orange', 'blue']
     let numbers = [1,2,3,4,5,6,7,8];
     numbers.reverse(); //(8) [8, 7, 6, 5, 4, 3, 2, 1]
     let cities = ['solapur', 'pune', 'mumbai','nagpur'];
     cities.reverse(); //(4) ['nagpur', 'mumbai', 'pune', 'solapur']
     ```
   - `reverse` Views the Elements in the array and returns The reversed array.
   - It mutate the original array.

9. `every`
   - Parameter: (callbackfn)A function to test for each element, taking three arguments:(element),(index)optional--(array),(thisarg)optional.

   - Return: true if the callbackFn function returns a truthy value for every array element. Otherwise, false.

   - Example:
     ```js
     let colors = ["blue","orange","yellow","purple"];
     let retColors = colors.every(function(color)){
       return color.length > 2;
     }
     retColors; //true
     let numbers = [1,2,3,4,5,6,7,8];
     let retNumbers = numbers.every(function(number)){
       return number > 0;
     }
     retNumbers; //true
    let numbers = [1,2,3,4,5,6,7,8];
     let retNumbers = numbers.every(function(number){
       return number < 5;
     });
     retNumbers; //false
     ```
   - `every` A callback function to test for each element, taking three arguments returns true if the callbackFn function returns a truthy value for every array element. Otherwise, false.
   - It returns only boolean value of every element in original array.

10. `shift`
  - Parameter: none.
   - Return:The removed element from the array; undefined if the array is empty.

   - Example:
     ```js
     let colors = ["blue","orange","yellow","purple"];
     colors.shift(); //(3) ['orange', 'yellow', 'purple']
     let numbers = [1,2,3,4,5,6,7,8];
     numbers.shift(); //(7) [2, 3, 4, 5, 6, 7, 8]
     let cities = ['solapur', 'pune', 'mumbai','nagpur'];
     cities.shift(); //(3) ['pune', 'mumbai', 'nagpur']
     ```
   - `shift` Views the Element to in the array and returns The removed element from the array; undefined if the array is empty.

   - It mutate the original array.

11. `splice`
 - Parameter: (start)The index at which to start changing the array.(deleteCount)optional--(item1, item2, ... )Optional---

   - Return:An array containing the deleted elements.

   - Example:
     ```js
     let colors = ["blue","orange","yellow","purple"];
     colors.splice(1); //['blue']
     let numbers = [1,2,3,4,5,6,7,8];
     numbers.splice(4); //(4) [1, 2, 3, 4]
     let cities = ['solapur', 'pune', 'mumbai','nagpur'];
     cities.splice(3,1,"Kolhapur"); //(4) ['solapur', 'pune', 'mumbai', 'Kolhapur']
     ```
   - `splice` The index at which to start changing the array and returns An array containing the deleted elements.

   - It mutate the original array.

12. `find`
   - Parameter: (callbackfn)A function to test for each element, taking three arguments:(element),(index)optional--(array),(thisarg)optional.

   - Return: The first element in the array that satisfies the provided testing function. Otherwise, undefined is returned.

   - Example:
     ```js
     let colors = ["blue","orange","yellow","purple"];
     function isOrange(color){
       return color === "orange";
     }
     let findReturnc = colors.find(isOrange); //'orange'
     let numbers = [1,2,3,4,5,6,7,8];
      function isSeven(number){
       return number === 7;
     }
     let findReturn = numbers.find(isSeven); //7
     ```
   - `find` A callback function to test for each element, taking three arguments returns The first element in the array that satisfies the provided testing function. Otherwise, undefined is returned.

   - It only finds element in original array.

13. `unshift`
  - Parameter: (element)The elements to add to the front of the arr.

   - Return:The new length property of the object upon which the method was called.

   - Example:
     ```js
     let colors = ["blue","orange","yellow","purple"];
     colors.unshift("red"); //(5) ['red', 'blue', 'orange', 'yellow', 'purple']
     let numbers = [1,2,3,4,5,6,7,8];
     numbers.unshift(10); //(7) [10,1,2, 3, 4, 5, 6, 7, 8]
     let cities = ['solapur', 'pune', 'mumbai','nagpur'];
     cities.unshift("x","y"); //(3) ['x','y''solapur','pune', 'mumbai', 'nagpur']
     ```
   - `unshift` adds the Element to the array and returns The new length property of the object upon which the method was called.

   - It mutate the original array.

14. `findIndex`
   - Parameter: (callbackfn)A function to test for each element, taking three arguments:(element),(index)optional--(array),(thisarg)optional.

   - Return: The index of the first element in the array that passes the test. Otherwise, -1.

   - Example:
     ```js
     let colors = ["blue","orange","yellow","purple"];
     function isOrange(color){
       return color === "orange";
     }
     let findIndexReturnc = colors.findIndex(isOrange); //1
     let numbers = [1,2,3,4,5,6,7,8];
      function isSeven(number){
       return number === 7;
     }
     let findIndexReturnc = numbers.findIndex(isSeven); //6
     ```
   - `findIndex` A callback function to test for each element, taking three arguments returns The index of the first element in the array that passes the test. Otherwise, -1.

   - It only finds index of element in original array.

15. `filter`
- Parameter: (callbackfn)A function to test for each element, taking three arguments:(element),(index)optional--(array),(thisarg)optional.

   - Return: A new array with the elements that pass the test. If no elements pass the test, an empty array will be returned.

   - Example:
     ```js
     let colors = ["blue","orange","yellow","purple"];
     function isOrange(color){
       return color === "orange";
     }
     let findReturnc = colors.filter(isOrange); //['orange']
     let numbers = [1,2,3,4,5,6,7,8];
      function isEven(number){
       return number % 2 === 0;
     }
     let findReturn = numbers.filter(isEven); //(4) [2, 4, 6, 8]
     ```
   - `findIndex` A callback function to test for each element, taking three arguments returns  A new array with the elements that pass the test. If no elements pass the test, an empty array will be returned.

   - It doesn't mutate in original array.

16. `flat`
- Parameter: n (any) number of values (number, string, boolean, array, null, undefined, object and function etc)(depth) optional--The depth level specifying how deep a nested array structure should be flattened. Defaults to 1.

   - Return: A new array with the sub-array elements concatenated into it.

   - Example:
     ```js
     let numbers = [1,2,[3,4,[5,6,[7,8]]]];
     numbers.flat(); //(5) [1, 2, 3, 4, Array(3)]
     numbers.flat(2); //(7) [1, 2, 3, 4, 5, 6, Array(2)]
     numbers.flat(4); //(8) [1, 2, 3, 4, 5, 6, 7, 8]
     ```
   - `flat` accepts n number of values and returns A new array with the sub-array elements concatenated into it. It does not change the original array.
   - No it does not mutate the original array

17. `forEach`
- Parameter: (callbackfn)A function to test for each element, taking three arguments:(element),(index)optional--(array),(thisarg)optional.

   - Return: undefined.

   - Example:
     ```js
     let colors = ["blue","orange","yellow","purple"];
     colors.forEach((color) => console.log(color));  // blue
                                                     //  orange
                                                      // yellow
                                                     //  purple
                                                     // undefined 
     let numbers = [1,2,3,4,5,6,7,8];
      numbers.forEach((number) => console.log(number)); // 1
                                                        // 2
                                                        // 3
                                                        // 4
                                                        // 5
                                                        // 6
                                                        // 7
                                                        // 8
                                                      //undefined 
                                                    
   - //`forEach` A callback function to test for each element, taking three arguments returns undefined.

   - //It doesn't mutate in original array.

18. `map`
- Parameter: (callbackfn)A function to test for each element, taking three arguments:(element),(index)optional--(array),(thisarg)optional.

   - Return: A new array with each element being the result of the callback function.

   - Example:
     ```js
     let numbers = [1,2,3,4,5,6,7,8];
      function double(number){
       return number * 2;
     }
     let doubleNumbers = numbers.map(double); //(8) [2, 4, 6, 8, 10, 12, 14, 16]
     let numbers = [1,2,3,4,5,6,7,8];
      function divide(number){
       return number / 2;
     }
     let divideNumbers = numbers.map(divide); //(8) [0.5, 1, 1.5, 2, 2.5, 3, 3.5, 4]
     ```
   - `map` A callback function to test for each element, taking three arguments returns  A new array with each element being the result of the callback function.

   - It doesn't mutate in original array.

19. `pop`
 - Parameter: none.
   - Return: The removed element from the array; undefined if the array is empty.

   - Example:
     ```js
     let cities = ['solapur', 'pune', 'mumbai','nagpur'];
     cities.pop(); //(3) ['solapur', 'pune', 'mumbai']
     let numbers = [1,2,3,4,5,6,7,8];
     numbers.pop(); //(7) [1, 2, 3, 4, 5, 6, 7]
     let cities = ['solapur-station', 'pune-station', 'mumbai-station','nagpur-station'];
     cities.pop(); //(3) ['solapur-station', 'pune-station', 'mumbai-station']
     ```
   - `pop` view elements of the array and returns The removed element from the array; undefined if the array is empty.

   - It mutate the original array.

20. `reduce`- 
  - Parameter: (callbackfn)A function to test for each element, taking four arguments:(previousValue),(currentValue)(currentIndex),(array).(initialValue) Optional

   - Return: The value that results from running the "reducer" callback function to completion over the entire array.


   - Example:
     ```js
     let numbers = [1,2,3,4,5,6,7,8];
      let sum = numbers.reduce((acc,num) => {
       return acc + num;
     },0)
     console.log(sum); //36
     let cities = ['solapur', 'pune', 'mumbai','nagpur'];
      let allCities = cities.reduce((acc,num) => {
       return acc + num;
     }, " ")
     console.log(allCities); // solapurpunemumbainagpur
     ```
   - `reduce` A callback function to test for each element, taking three arguments returns The value that results from running the "reducer" callback function to completion over the entire array.

   - It doesn't mutate in original array.

21. `slice`
- Parameter: (start)Optional--(end)Optional--.
   - Return: A new array containing the extracted elements.

   - Example:
     ```js
     let cities = ['solapur', 'pune', 'mumbai','nagpur'];
     cities.slice(2); //(2) ['mumbai', 'nagpur']
     let numbers = [1,2,3,4,5,6,7,8];
     numbers.slice(5); //(3) [6, 7, 8]
     let colors = ["blue","orange","yellow","purple"];
     colors.slice(2,4); //(3) (2) ['yellow', 'purple']
     ```
   - `slice` view elements of the array and returns A new array containing the extracted elements.

   - It doesn't mutate the original array.

22. `some`
- Parameter: (callbackfn)A function to test for each element, taking four arguments:(previousValue),(currentValue)  (currentIndex),(array).(initialValue) Optional

   - Return: true if the callback function returns a truthy value for at least one element in the array. Otherwise, false.

   - Example:
     ```js
     let numbers = [1,2,3,4,5,6,7,8];
      let ret = numbers.some(function(number) {
       return number > 0;
     })
     console.log(ret); //true
     let cities = ['solapur', 'pune', 'mumbai','nagpur'];
      let retCities = cities.some(function(city) {
       return city.includes("pune");
     })
      console.log(retCities); // true
    ```
   - `reduce` A callback function to test for each element, taking three arguments returns true if the callback function returns a truthy value for at least one element in the array. Otherwise, false.

   - It doesn't mutate in original array.

