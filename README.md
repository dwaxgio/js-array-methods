# 1. map()
## This method creates a new array with the results of calling a provided function on every element in this array
console.log("map()");
const arr = [1, 2, 3, 4, 5];

const mapped = arr.map((e) => e + 30);
console.log(mapped);

# 2. filter()
## This method creates a new array with only elements that passes the condition inside theprovided function.
console.log("filter()");
const arr2 = [1, 2, 3, 4, 5];

const filtered = arr2.filter((e) => e == 2 || e == 4);
console.log(filtered);

# 3. sort()
## This method is used to arrage/sort array's elements either in ascending or descending order
console.log("sort()");
const arr3 = [1, 2, 3, 4, 5];
const arr3_2 = ["f", "a", "c", "v", "z"];

// sort in descending order
const descending = arr3.sort((e1, e2) => (e1 > e2 ? -1 : 1));
console.log(descending);

const ascending = arr3_2.sort((e1, e2) => (e1 > e2 ? 1 : -1));
console.log(ascending);

# 4. forEach()
## This method helps to loop over array by executing a provided callback function for each element in an array
console.log("forEach()");

const arr4 = [1, 2, 3];
arr4.forEach((e) => console.log(e * 2));

# 5. concat()
## This method is used to merge two or more arrays and returns a new array
console.log("concat()");

const arr5 = ["a", "b", "c"];
const arr5_2 = ["d", "e", "f"];

const concatenated = arr5.concat(arr5_2);
console.log(concatenated);

# 6. every()
## This method checks every element in the array that passes the condition, returnning true or false as appropriate
console.log("every()");

const arr6 = [1, 2, 3, 4, 5];
const greaterThree = arr6.every((e) => e > 3);
console.log(greaterThree);

const lessThanSix = arr6.every((e) => e < 6);
console.log(lessThanSix);

# 7. some()
## This method checks if at least one element in the array that passes the condition, returning true or false as appropriate
console.log("some()");

const arr7 = [1, 2, 3, 4, 5];
const greaterNumber = arr7.some((e) => e > 3);
console.log(greaterNumber);

const lessNumber = arr7.some((e) => e < 0);
console.log(lessNumber);

# 8. includes()
## This method checks if an array includes the element that passes the condition, returning true or false as appropriate
console.log("includes()");

const arr8 = [1, 2, 3, 4, 5];
console.log(arr8.includes(6));
console.log(arr8.includes(2));

# 9. join()
## This method returns a new string by concatenating all of the array's elements separated by the specified separator
console.log("join()");
const arr9 = ["h", "e", "l", "l", "o"];
console.log(arr9.join(""));

# 10. reduce()
## This method applies a function against an accumulator and each element in the array to reduce it to a single value
console.log("reduce()");

const arr10 = [1, 2, 3, 4, 5];
const reduced = arr10.reduce((total, current) =>
  console.log(total, " ", current)
);
console.log(reduced);

# 11. find()
## This method return the value of the first element in an array that pass the test in a testing function
console.log("find()");

const arr11 = [1, 2, 3, 4, 5];
const found = arr11.find((e) => e > 3);
console.log(found);

# 12. findIndex()
## This method returns the index of the first element in an array that pass the test in a testing function
console.log("findIndex()");

const arr12 = ["Spiderman", "Thor", "Hulk"];
const indexFound = arr12.findIndex((e) => e == "Thor");
console.log(indexFound);

# 13. indexOf()
## This method returns the index of the first occurrence of the specified element in the array, or -1 if it is not found
console.log("indexOf()");

const arr13 = ["Spiderman", "Thor", "Hulk"];
const indexFinder = arr13.indexOf("Thor");
console.log(indexFinder);

# 14. fill()
## This method fills the elements in an array with a static value and returns the modified array
console.log("fill()");

const arr14 = new Array(3);
console.log(arr14);
console.log(arr14.fill(10));

# 15. slice()
## This method returns a new array with specified start to end elements
console.log("slice()");
const arr15 = ["a", "b", "c", "d", "e"];

const sliced = arr15.slice(3, 4);
console.log(sliced);

# 16. reverse()
## This method reverses an array in place. Element at last index will be first and element at 0 index will be last
console.log("reverse()");
const arr16 = [1, 2, 3];
console.log(arr16.reverse());

# 17. push()
## This method adds one or more elements to the end of array and returns the new length of the array
console.log("push()");

const arr17 = ["Apple", "Peach"];
console.log(arr17.push("Banana"));
console.log(arr17);

# 18. pop()
## This method removes the last element from the end of the array and returns that element
console.log("pop()");

const arr18 = ["Apple", "Peach"];
arr18.pop();
console.log(arr18);

# 19. shift()
## This method removes the first element from an array and returns that element
console.log("shift()");
const arr19 = ["Apple", "Peach"];
arr19.shift();
console.log(arr19);

# 20. unshift()
## This method adds one or more elemnts to the beginning of an array and returns the new length of the array
console.log("unshift()");
const arr20 = ["Apple", "Peach"];
console.log(arr20.unshift("Banana"));
console.log(arr20);
