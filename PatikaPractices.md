#  Patika.dev Array Practices
You can find the practices with their explanations.

##  Practice 1
let arr = [2,5,8,11,15,17];

//  Using the appropriate array methods, create a new array consisting of 5 times each of the elements greater than 10 in the array elements given above. (should be [55, 75, 85] )

let newArr= arr.filter((num) => num>10).map((num2) => num2* 5)

console.log(newArr) // newArr=[55,75,85]

## Practice 2

let arr = [3,6,9,14,16];

//   Using the appropriate array methods, write the function myFunction that satisfies the following conditions for the above array.
//  If there is an element greater than 5 among the elements, the console will say "An element greater than five exists." otherwise "Element greater than 5 does not exist." print.

function myFunction (arr){
 arr.some((num) => num>5) ? console.log("An element greater than five exists.") : console.log("Element greater than 5 does not exist.");
}

myFunction(arr);

##  Practice 3
// Write a function that returns the result (24) of multiplying the elements of the below array using the appropriate array method.

let arr = [2,3,4];

function reductive(num,num1) {
  return num* num1;
}

let result = arr.reduce(reductive,1);

console.log(result)
