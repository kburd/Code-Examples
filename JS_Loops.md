```javascript

//While loop that counts to 5
// let count = 0;
// while(count < 5){
//     console.log("Hello Howie");
//     count++;
// }

//Infinite loop
//Becareful not to run

// let count = 0;
// while(count < 5){
//     console.log("Hello Howie");
// }

// Exercise 1
// Generate a random number and have the user guess until they guess correctly

//Setup
// let randomNumber = Math.floor(Math.random() * 10) + 1;
// let userGuess = prompt("Guess a number between 1 - 10");

// //Condition
// while(randomNumber != userGuess){

//     //Body Logic
//     userGuess = prompt("Guess a number between 1 - 10");

// }

// alert(`You got it! The number was ${randomNumber}`);

//Do while
// let randomNumber = Math.floor(Math.random() * 10) + 1;
// let userGuess;

// do {
//     userGuess = prompt("Guess a number between 1 - 10");
// } while(randomNumber != userGuess);

// alert(`You got it! The number was ${randomNumber}`);

// Exercise 2
// Sum the number from 1 - 5 using a loop 

// let count = 0;
// let total = 0;

// while(count <= 5){
//     total += count;
//     count++;
// }

// console.log(total);

//For
// let total = 0;

// //Start, stop, step
// for(let count = 0; count <= 5; count++){
//     total += count;
// }

// console.log(total);

// Exercise 3
// Conver the following into a for loop
// let count = 0;
// while(count < 5){
//     console.log("Hello Howie");
//     count++;
// }

//Goes from 0 to 4, one at a time
// for(let i = 0; i < 5; i++){
//     console.log(i);
// }

//Goes from 1 to 9, one at a time
// for(let i = 1; i < 10; i++){
//     console.log(i);
// }

//i++ -> i += 1
//Goes from 0 to 5, two at a time
// for(let i = 0; i < 6; i += 2){
//     console.log(i)
// }

//5 4 3 2 1 0
//Goes from 5 to 0, one at a time
// for(let i = 5; i >= 0; i--){
//     console.log(i);
// }

//Goes from -10 to 10, three at a time
// for(let i = -10; i <= 10; i += 3){
//     console.log(i);
// }

// Break
// for(let i = 0; i < 10; i++){
//     if(i === 5){
//         break;
//     }
//     console.log(i);
// }

//Continue
// for(let i = 0; i < 10; i++){
//     if(i === 5){
//         continue;
//     }
//     console.log(i);
// }

// Exercise 3
// let output = "";
// for(let i = 1; i <= 10; i++){
//     output += `<p>"${i}</p>`;
// }
// console.log(output);
// document.getElementById("kaleb").innerHTML = output;

// let output = "";
// for(let i = 1; i <= 10; i++){
//     output += `<li>${i}</li>`;
// }

let listItems = "";
for(let i = 1; i <= 10; i++){
    listItems += `<li>${i}</li>`;
}
let answer, output;
answer = prompt("Ordered List? (Y/N)");
output = (answer === "Y") ? `<ol>${listItems}</ol>` : `<ul>${listItems}</ul>`;
document.getElementById("kaleb").innerHTML = output;
```