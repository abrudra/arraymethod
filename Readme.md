# Array Methods :-

## 1. concat( ):-
  
* <u>Parameter it accepts :- </U>

    n (any) number of values (number, string, boolean, array, null, undefined, object and function etc).

* <u> what it will return :- </u>
   
   A single Array consisting of by all the values passed as parameters in the same order.

* <u> Example :-</u>

        let numbers = [1, 2, 3];

        numbers.concat(4); //[1,2,3,4]

        let sentanceArray = 'A quick brown fox jumped over a lazy'.split(' ');

        sentanceArray.concat('dog').join(' '); //"A quick brown fox jumped over a lazy dog"

        let colors = ['red', 'green', 'blue'];

        colors.concat('black', 'red', 21, true); // ['red','green 'blue','black', 'red', 21, true]

* <u> Discription :  - </u>

    concat accepts n number of values and returns one array with all the values in same order. It does not change the original array.

* <u> Does it mutate the original array? </u>

    No.

## 2. flat( ) :-

* <u>Parameter it accepts :- </U>
 
  The depth level specifying how deep a nested array structure should be flattened. Defaults to 1.

* <u> what it will return :- </u>

    A new array with the sub-array elements concatenated into it.

* <u> Example :-</u>

        const arr1 = [1, 2, [3, 4]];

        arr1.flat();
        // [1, 2, 3, 4]

        const arr2 = [1, 2, [3, 4, [5, 6]]];
        arr2.flat();
        // [1, 2, 3, 4, [5, 6]]

* <u> Discription :  - </u>

    It removes the values from nested array and gives the new array that are present in one array.

* <u> Does it mutate the original array? </u>

    No.

## 3. push ( )  :-


* <u>Parameter it accepts :- </U>
 
    The element(s) to add to the end of the array.

* <u>what it will return :- </u>

   The new length property of the object upon which the method was called.

* <u>Example :-</u>

        const sports = ['soccer', 'baseball'];
        const total = sports.push('football', 'swimming');

        console.log(sports); // ['soccer', 'baseball', 'football', 'swimming']
        console.log(total); // 4

* <u> Discription :  - </u>

    Push method is used for adding new element in the array list and that element added at last in elment.

* <u> Does it mutate the original array? </u>

    Yes.

## 4. pop ( )  :-


* <u>Parameter it accepts :- </U>
 
    The element(s) to remove to the end of the array.

* <u> 2. what it will return :- </u>

   The removed element from the array; undefined if the array is empty.

* <u> 3. Example :-</u>

        const myFish = ['angel', 'clown', 'mandarin', 'sturgeon'];

        const popped = myFish.pop();

        console.log(myFish); //['angel', 'clown', 'mandarin']

        console.log(popped); // 'sturgeon'

* <u> Discription :  - </u>

    The pop() method removes the last element from an array and returns that value to the caller. If you call pop() on an empty array

* <u> Does it mutate the original array? </u>

    Yes.

## 5. shift ( )  :-


* <u>Parameter it accepts :- </U>
 
    The shift() method removes the first element from an array and returns that removed element

* <u> 2. what it will return :- </u>

   The removed element from the array; undefined if the array is empty.

* <u> 3. Example :-</u>

        const array1 = [1, 2, 3];

        const firstElement = array1.shift();

        console.log(array1);
        // expected output: Array [2, 3]

        console.log(firstElement);
        // expected output: 1'

* <u> Discription :  - </u>

    The shift( ) method removes the element from zeroth index and shifts all values in consecutive way. 

* <u> Does it mutate the original array? </u>

    Yes.

## 6. unshift ( )  :-


* <u>Parameter it accepts :- </U>
 
    The elements to add to the front of the arr.

* <u> 2. what it will return :- </u>

   The new length property of the object upon which the method was called.

* <u> 3. Example :-</u>

        let arr = [4, 5, 6];

        arr.unshift(1, 2, 3);
        console.log(arr);
        // [1, 2, 3, 4, 5, 6]

* <u> Discription :  - </u>

    The unshift() method inserts the given values to the beginning of an array-like object.

* <u> Does it mutate the original array? </u>

    Yes.

## 7. indexOf ( )  :-


* <u>Parameter it accepts :- </U>
 
    <i> searchElement </i>

    Element to locate in the array.



* <u> 2. what it will return :- </u>

   The first index of the element in the array; -1 if not found.

* <u> 3. Example :-</u>

        const array = [2, 9, 9];
        array.indexOf(2);     // 0
        array.indexOf(7);     // -1
        array.indexOf(9, 2);  // 2
        array.indexOf(2, -1); // -1
        array.indexOf(2, -3); // 0

* <u> Discription :  - </u>

    indexOf( ) method is used to find the index of element in given array .if any think not found then it will return -1.

* <u> Does it mutate the original array? </u>

    No.

## 8. lastIndexdOf ( )  :-


* <u>Parameter it accepts :- </U>
 
    <i> searchElement </i>

    Element to locate in the array.

* <u> 2. what it will return :- </u>

    The last index of the element in the array; -1 if not found.

* <u> 3. Example :-</u>

        const numbers = [2, 5, 9, 2];
        numbers.lastIndexOf(2);     // 3
        numbers.lastIndexOf(7);     // -1
        numbers.lastIndexOf(2, 3);  // 3
        numbers.lastIndexOf(2, 2);  // 0
        numbers.lastIndexOf(2, -2); // 0
        numbers.lastIndexOf(2, -1); // 3

* <u> Discription :  - </u>

    lastindexOf( ) method is used to find the index of last element in given array .if any think not found then it will return -1.

* <u> Does it mutate the original array? </u>

    No.

## 9. includes ( )  :-


* <u>Parameter it accepts :- </U>
 
    <i> searchElement </i>

    The value to search for.


* <u> 2. what it will return :- </u>

    true , if values found that search in array.

* <u> 3. Example :-</u>

        [1, 2, 3].includes(2)         // true
        [1, 2, 3].includes(4)         // false
        [1, 2, 3].includes(3, 3)      // false
        [1, 2, 3].includes(3, -1)     // true
        [1, 2, NaN].includes(NaN)     // true
        ["1", "2", "3"].includes(3)   // false

* <u> Discription :  - </u>

    The includes() method compares searchElement to elements of the array using the SameValueZero algorithm.

    When used on sparse arrays, the includes() method iterates empty slots as if they have the value undefined.

* <u> Does it mutate the original array? </u>

    No.

## 10. reverse ( )  :-


* <u>Parameter it accepts :- </U>
 
    Given array.


* <u> 2. what it will return :- </u>

    The reference to the original array, now reversed. 

* <u> 3. Example :-</u>

        const items = [1, 2, 3];
        console.log(items); // [1, 2, 3]

        items.reverse();
        console.log(items); // [3, 2, 1]

* <u> Discription :  - </u>

   using revese( ) method it reverse the given  array in to the new array.

* <u> Does it mutate the original array? </u>

    Yes.

## 11. splice ( )  :-


* <u>Parameter it accepts :- </U>
 
     <i> start </i>

    Zero-based index at which to start changing the array, converted to an integer.

    <i>deleteCount (Optional)</i>

    An integer indicating the number of elements in the array to remove from start.


* <u> 2. what it will return :- </u>

    An array containing the deleted elements.

* <u> 3. Example :-</u>

        const myFish = ['angel', 'clown', 'mandarin', 'sturgeon'];
        const removed = myFish.splice(2, 0, 'drum');

        // myFish is ["angel", "clown", "drum", "mandarin", "sturgeon"]
        // removed is [], no elements removed

* <u> Discription :  - </u>

   The splice() method is a mutating method. It may change the content of this. If the specified number of elements to insert differs from the number of elements being removed, the array's length will be changed as well. 

* <u> Does it mutate the original array? </u>

    Yes.

## 12. slice ( )  :-


* <u>Parameter it accepts :- </U>
 
    <i>start (Optional)</i>

    Zero-based index at which to start extraction, converted to an integer.

    <i>end (Optional)</i>

    Zero-based index at which to end extraction, converted to an integer. slice() extracts up to but not including end.


* <u> 2. what it will return :- </u>

    An array containing the deleted elements.

* <u> 3. Example :-</u>

        const myFish = ['angel', 'clown', 'mandarin', 'sturgeon'];
        const removed = myFish.splice(2, 0, 'drum');

        // myFish is ["angel", "clown", "drum", "mandarin", "sturgeon"]
        // removed is [], no elements removed

* <u> Discription :  - </u>

   The splice() method is a mutating method. It may change the content of this. If the specified number of elements to insert differs from the number of elements being removed, the array's length will be changed as well. 

* <u> Does it mutate the original array? </u>

    No.

## 13. forEach ( )  :-


* <u>Parameter it accepts :- </U>
 
    <i>callbackFn</i>

    A function to execute for each element in the array. Its return value is discarded.

    The function is called with the following arguments:

    <i>element</i>

    The current element being processed in the array.

    <i>index</i>
    
    The index of the current element being processed in the array.


* <u> 2. what it will return :- </u>

    undefined.

* <u> 3. Example :-</u>

        const arraySparse = [1, 3, /* empty */, 7];
        let numCallbackRuns = 0;

        arraySparse.forEach((element) => {
        console.log({ element });
        numCallbackRuns++;
        });

        console.log({ numCallbackRuns });

* <u> Discription :  - </u>

   The forEach() method is an iterative method. It calls a provided callbackFn function once for each element in an array in ascending-index order. 

* <u> Does it mutate the original array? </u>

    No.

## 14. map   ( )  :-


* <u>Parameter it accepts :- </U>
 
    <i>callbackFn</i>

    A function to execute for each element in the array. Its return value is added as a single element in the new array.

    The function is called with the following arguments:

    <i>element</i>

    The current element being processed in the array.

    <i>index</i>
    
    The index of the current element being processed in the array.


* <u> 2. what it will return :- </u>

    A new array with each element being the result of the callback function.

* <u> 3. Example :-</u>

        const numbers = [1, 4, 9];
        const roots = numbers.map((num) => Math.sqrt(num));

        // roots is now     [1, 2, 3]
        // numbers is still [1, 4, 9]

* <u> Discription :  - </u>

    The map() method is an iterative method. It calls a provided callbackFn function once for each element in an array and constructs a new array from the results.

* <u> Does it mutate the original array? </u>

    No.

## 15. filter   ( )  :-


* <u>Parameter it accepts :- </U>
 
    <i>callbackFn</i>

    A function to execute for each element in the array. It should return a truthy to keep the element in the resulting array, and a falsy value otherwise.

    The function is called with the following arguments:

    <i>element</i>

    The current element being processed in the array.

    <i>index</i>
    
    The index of the current element being processed in the array.


* <u> 2. what it will return :- </u>

    A shallow copy of a portion of the given array, filtered down to just the elements from the given array that pass the test implemented by the provided function.

* <u> 3. Example :-</u>

        function isBigEnough(value) {
        return value >= 10;
        }

        const filtered = [12, 5, 8, 130, 44].filter(isBigEnough);
        // filtered is [12, 130, 44]

* <u> Discription :  - </u>

    The filter() method is an iterative method. It calls a provided callbackFn function once for each element in an array, and constructs a new array of all the values for which callbackFn returns a truthy value.

* <u> Does it mutate the original array? </u>

    No.

## 16. find   ( )  :-


* <u>Parameter it accepts :- </U>
 
    <i>callbackFn</i>

    A function to execute for each element in the array. It should return a truthy value to indicate a matching element has been found.

    The function is called with the following arguments:

    <i>element</i>

    The current element being processed in the array.

    <i>index</i>
    
    The index of the current element being processed in the array.


* <u> 2. what it will return :- </u>

    The first element in the array that satisfies the provided testing function. Otherwise, undefined is returned.

* <u> 3. Example :-</u>

        const inventory = [
        { name: "apples", quantity: 2 },
        { name: "bananas", quantity: 0 },
        { name: "cherries", quantity: 5 },
        ];

        function isCherries(fruit) {
        return fruit.name === "cherries";
        }

        console.log(inventory.find(isCherries));
        // { name: 'cherries', quantity: 5 }

* <u> Discription :  - </u>

    The find() method is an iterative method. It calls a provided callbackFn function once for each element in an array in ascending-index order, until callbackFn returns a truthy value. 

* <u> Does it mutate the original array? </u>

    No.

## 17. findIndex   ( )  :-


* <u>Parameter it accepts :- </U>
 
    <i>callbackFn</i>

    A function to execute for each element in the array. It should return a truthy value to indicate a matching element has been found.

    The function is called with the following arguments:

    <i>element</i>

    The current element being processed in the array.

    <i>index</i>
    
    The index of the current element being processed in the array.


* <u> 2. what it will return :- </u>

    The index of the first element in the array that passes the test. Otherwise, -1.

* <u> 3. Example :-</u>

        function isPrime(element) {
        if (element % 2 === 0 || element < 2) {
            return false;
        }
        for (let factor = 3; factor <= Math.sqrt(element); factor += 2) {
            if (element % factor === 0) {
            return false;
            }
        }
        return true;
        }

        console.log([4, 6, 8, 9, 12].findIndex(isPrime)); // -1, not found
        console.log([4, 6, 7, 9, 12].findIndex(isPrime)); // 2 (array[2] is 7)

* <u> Discription :  - </u>

   The findIndex() is an iterative method. It calls a provided callbackFn function once for each element in an array in ascending-index order, until callbackFn returns a truthy value.

* <u> Does it mutate the original array? </u>

    No.

## 18. some   ( )  :-


* <u>Parameter it accepts :- </U>
 
    <i>callbackFn</i>

    A function to execute for each element in the array. It should return a truthy to indicate the element passes the test, and a falsy value otherwise.

    The function is called with the following arguments:

    <i>element</i>

    The current element being processed in the array.

    <i>index</i>
    
    The index of the current element being processed in the array.


* <u> 2. what it will return :- </u>

    true if the callback function returns a truthy value for at least one element in the array. Otherwise, false.

* <u> 3. Example :-</u>

        function isBiggerThan10(element, index, array) {
        return element > 10;
        }

        [2, 5, 8, 1, 4].some(isBiggerThan10);  // false
        [12, 5, 8, 1, 4].some(isBiggerThan10); // true

* <u> Discription :  - </u>

   The some() method is an iterative method. It calls a provided callbackFn function once for each element in an array, until the callbackFn returns a truthy value.

* <u> Does it mutate the original array? </u>

    No.

## 19. every   ( )  :-


* <u>Parameter it accepts :- </U>
 
    <i>callbackFn</i>

    A function to execute for each element in the array. It should return a truthy to indicate the element passes the test, and a falsy value otherwise.

    The function is called with the following arguments:

    <i>element</i>

    The current element being processed in the array.

    <i>index</i>
    
    The index of the current element being processed in the array.


* <u> 2. what it will return :- </u>

    true if callbackFn returns a truthy value for every array element. Otherwise, false.

* <u> 3. Example :-</u>

        function isBigEnough(element, index, array) {
        return element >= 10;
        }
        [12, 5, 8, 130, 44].every(isBigEnough);   // false
        [12, 54, 18, 130, 44].every(isBigEnough); // true

* <u> Discription :  - </u>

   The every() method is an iterative method. It calls a provided callbackFn function once for each element in an array, until the callbackFn returns a falsy value.

* <u> Does it mutate the original array? </u>

    No.

## 20. sort   ( )  :-


* <u>Parameter it accepts :- </U>
 
    <i>compareFn</i>

    Specifies a function that defines the sort order. If omitted, the array elements are converted to strings, then sorted according to each character's Unicode code point value.

    The function is called with the following arguments:

    <i>a</i>

    The first element for comparison.

    <i>b</i>
    
    The second element for comparison.


* <u> 2. what it will return :- </u>

    The reference to the original array, now sorted. Note that the array is sorted in place, and no copy is made.

* <u> 3. Example :-</u>

        const stringArray = ['Blue', 'Humpback', 'Beluga'];

        function compareNumbers(a, b) {
        return a - b;
        }

        stringArray.join(); // 'Blue,Humpback,Beluga'
        stringArray.sort(); // ['Beluga', 'Blue', 'Humpback']

* <u> Discription :  - </u>

   If compareFn is not supplied, all non-undefined array elements are sorted by converting them to strings and comparing strings in UTF-16 code units order.

* <u> Does it mutate the original array? </u>

    Yes.

## 21. reduce   ( )  :-


* <u>Parameter it accepts :- </U>
 
    <i>callbackFn</i>

    A function to execute for each element in the array. Its return value becomes the value of the accumulator parameter on the next invocation of callbackFn.

    The function is called with the following arguments:

    <i>accumulator</i>

    The value resulting from the previous call to callbackFn. On first call, initialValue if specified, otherwise the value of array[0].

    <i>currentValue</i>
    
    The value of the current element. On first call, the value of array[0] if an initialValue was specified, otherwise the value of array[1].

    <i>currentIndex</i>
    
    The index position of currentValue in the array. On first call, 0 if initialValue was specified, otherwise 1.

* <u> 2. what it will return :- </u>

    The value that results from running the "reducer" callback function to completion over the entire array.

* <u> 3. Example :-</u>

        const array = [15, 16, 17, 18, 19];

        function reducer(accumulator, currentValue, index) {
        const returns = accumulator + currentValue;
        console.log(
            `accumulator: ${accumulator}, currentValue: ${currentValue}, index: ${index}, returns: ${returns}`,
        );
        return returns;
        }
        array.reduce(reducer);

* <u> Discription :  - </u>

   The reduce() method is an iterative method. It runs a "reducer" callback function over all elements in the array, in ascending-index order, and accumulates them into a single value. 

* <u> Does it mutate the original array? </u>

    No.