```javascript

let name = "Kaleb";

//Initializing empty array
let info = [];

//Initializing and array with values
let cars = ["Jetta", "GTI", "Beetle"];

//Length
console.log(cars.length)

//Indexing
console.log(cars[0]);
console.log(cars[1]);
console.log(cars[2]);

//Index out of bounds
console.log(cars[3]);

//Iterate through an array
for(let i = 0; i < cars.length; i++){
    console.log(cars[i]);
}

// Exercise 1: Summing values in an array
let nums = [3, 8, 2, 1];
let total = 0;
for(let i = 0; i < nums.length; i++){
    total += nums[i];
}
console.log(total);

/*
nums:   [3, 8, 2, 1];
total:  14
i:      4
*/

//Updating Arrays
cars = ["Jetta", "GTI", "Beetle"];
console.log(cars);
cars[1] = "Golf";
console.log(cars);

//Exercise 2: Double each elements
//[6, 16, 4, 2]
nums = [3, 8, 2, 1, 5];
for(let i = 0; i < nums.length; i++){
    nums[i] *= 3;
}
console.log(nums)

// Append a value
cars = ["Jetta", "GTI", "Beetle"];
cars.push("Passat");
cars.push("VW Bus");
console.log(cars);
console.log(cars.length);

//Given an length and value
//Fill an array of size length with the value
let length = 40;
let value = "Hakim"; //["Kaleb", "Kaleb", "Kaleb", "Kaleb"]

let myArray = [];
for(let i = 0; i < length; i++){
    myArray.push(value);
}
console.log(myArray);

// Removing/Pop
cars = ["Jetta", "GTI", "Beetle"];
let singleCar = cars.pop();
console.log(cars);
// console.log(singleCar);

cars.push(singleCar);
console.log(cars);

// Slicing
cars = ["Jetta", "Golf", "Passat", "Beetle", "VW Bus", "GTI", "ID.4"];
let antiques = cars.slice(3,5);
console.log(antiques);

//Get Last 3
cars = ["Jetta", "Golf", "Passat", "Beetle", "VW Bus", "GTI", "ID.4", "Eos", "CC"];
let lastThree = cars.slice(cars.length-3, cars.length);
console.log(lastThree);

//Two Dimmensional Arrays
cars = [
    ["Jetta", "Passat", "GLI"],
    ["Beetle", "VW Bus", "CC"],
    ["Golf", "GTI", "Atlas"]
];

cars[1][2] = "Eos";
console.log(cars)

//Iterating a 2D array
// console.log(cars[0][0])
// console.log(cars[0][1])
// console.log(cars[0][2])
// console.log(cars[1][0])
// console.log(cars[1][1])
// console.log(cars[1][2])
// console.log(cars[2][0])
// console.log(cars[2][1])
// console.log(cars[2][2])

// let i = 0;
// console.log(cars[i][0])
// console.log(cars[i][1])
// console.log(cars[i][2])

// i = 1;
// console.log(cars[i][0])
// console.log(cars[i][1])
// console.log(cars[i][2])

// i = 2;
// console.log(cars[i][0])
// console.log(cars[i][1])
// console.log(cars[i][2])

// for(let i = 0; i < 3; i++){
//     console.log(cars[i][0])
//     console.log(cars[i][1])
//     console.log(cars[i][2])
// }

// for(let i = 0; i < 3; i++){

//     let j = 0;
//     console.log(cars[i][j]);

//     j = 1;
//     console.log(cars[i][j]);

//     j = 2;
//     console.log(cars[i][j]);

// }

for(let i = 0; i < 3; i++){
    for(let j = 0; j < 3; j++){
        console.log(cars[i][j]);
    }
}

/*
i: 0, j: 0
i: 0, j: 1
i: 0, j: 2
i: 1, j: 0
i: 1, j: 1
i: 1, j: 2
i: 2, j: 0 
i: 2, j: 1
i: 2, j: 2
*/
```