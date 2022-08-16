# Arrays
## Splice

splice() is another handy method that allows you to add and remove elements from anywhere within an array.

While push() and pop() limit you to adding and removing elements from the end of an array, splice() lets you specify the index location to add new elements, as well as the number of elements you'd like to delete (if any).

var donuts = ["glazed", "chocolate frosted", "Boston creme", "glazed cruller"];
donuts.splice(1, 1, "chocolate cruller", "creme de leche"); 


# Directions:

Use a nested for loop to take the numbers array below and replace all of the values that are divisible by 2 (even numbers) with the string "even" and all other numbers with the string "odd".
/*
 * Programming Quiz: Nested Numbers (6-10)
 * QUIZ REQUIREMENTS
 *   - The `numbers` variable is an array of arrays.
 *   - Use a nested `for` loop to cycle through `numbers`.
 *   - Convert each even number to the string "even"
 *   - Convert each odd number to the string "odd"
 */


var numbers = [
    [243, 12, 23, 12, 45, 45, 78, 66, 223, 3],
    [34, 2, 1, 553, 23, 4, 66, 23, 4, 55],
    [67, 56, 45, 553, 44, 55, 5, 428, 452, 3],
    [12, 31, 55, 445, 79, 44, 674, 224, 4, 21],
    [4, 2, 3, 52, 13, 51, 44, 1, 67, 5],
    [5, 65, 4, 5, 5, 6, 5, 43, 23, 4424],
    [74, 532, 6, 7, 35, 17, 89, 43, 43, 66],
    [53, 6, 89, 10, 23, 52, 111, 44, 109, 80],
    [67, 6, 53, 537, 2, 168, 16, 2, 1, 8],
    [76, 7, 9, 6, 3, 73, 77, 100, 56, 100]
];

// your code goes here
for(var row=0;row<numbers.length;row++){
    for(var col=0;col<numbers[row].length;col++){
        if(numbers[row][col]%2===0){
            numbers[row][col]="even";
        }
        else{
             numbers[row][col]="odd";
        }
    }
}
console.log(numbers);



# Object in Java Script
Using the umbrella example from the previous video, see if you can follow the example open() method and create the close() method. It's alright if you have trouble at first! We'll go into more detail later in this lesson
var umbrella = { 
  color: "pink",
  isOpen: false,
  open: function() { 
    if (umbrella.isOpen === true) {
      return "The umbrella is already opened!";
    } else {
      umbrella.isOpen = true;
      return "Julia opens the umbrella!";
    }
   }
};


Directions:

Using the umbrella example from the previous video, see if you can follow the example open() method and create the close() method. It's alright if you have trouble at first! We'll go into more detail later in this lesson.
/*
 * Programming Quiz: Umbrella (7-1)
 */
/*
 * QUIZ REQUIREMENTS
 * - Your code should have a variable `umbrella`
 * - The variable `umbrella` should be an object
 * - Your `umbrella` object should have the `color` and `isOpen` property
 * - Your `umbrella` object should have an `open()` method that toggles the value of `isOpen` property
 * - Your `umbrella` object should have an `close()` method that toggles the value of `isOpen`
 */

var umbrella = {
    color: "pink",
    isOpen: true,
    open: function() {
        if (umbrella.isOpen === true) {
            return "The umbrella is already opened!";
        } else {
            umbrella.isOpen = true;
            return "Julia opens the umbrella!";
        }
    },
    close:function(){
         if (umbrella.isOpen === false) {
            return "The umbrella is already closed!";
        } else {
            umbrella.isOpen = false;
            return "Julia closes the umbrella!";
        }
    }
    // your code goes here
};
console.log(umbrella.open());
console.log(umbrella.close());


## Object-literal notation

var sister = {
  name: "Sarah", 
  age: 23,
  parents: [ "alice", "andy" ],
  siblings: ["julia"],
  favoriteColor: "purple",
  pets: true
};

The syntax you see above is called object-literal notation. There are some important things you need to remember when you're structuring an object literal:

    The "key" (representing a property or method name) and its "value" are separated from each other by a colon
    The key: value pairs are separated from each other by commas
    The entire object is wrapped inside curly braces { }.

