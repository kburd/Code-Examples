```javascript

//Defining a function
function displayHelloWorld(){
    console.log("Hello World");
}

//Call a function
// displayHelloWorld();

//Display Hello world three times
// displayHelloWorld();
// displayHelloWorld();
// displayHelloWorld();

//Display Hello world 10 times
//start stop step
// for(let i = 0; i < 10; i++){
//     displayHelloWorld();
// }

//Parameters
function displayInConsole(text){
    console.log(text);
}

let message = "Hello Kaleb";
displayInConsole(message);

//Missing parameter
displayInConsole();

//Add two numbers and display
function numbers(numOne, numTwo){
    let answer = numOne + numTwo;
    console.log(answer);
}

numbers(3,4);


//Return 
function add(numOne, numTwo){
    let answer = numOne + numTwo;
    return answer;
}

let solution = add(6, 2);
console.log(solution);

// Circumference
// c = 2 pi r
function circumference(radius){
    let answer = 2 * Math.PI * radius;
    return answer;
}

solution = circumference(3);
console.log(solution)

solution = circumference(1);
// alert(solution);


// Area of a square
// a = side * side
function getAreaOfSquare(side){
    return Math.pow(side, 2);
}

console.log(getAreaOfSquare(3));
console.log(getAreaOfSquare(6));
console.log(getAreaOfSquare(2));

// Double the number
function doubleNumber(number){
    return number * 2;
}

console.log(doubleNumber(3))

// Display dollar amount
function displayDollarAmount(amount){
    console.log(`Amount: ${amount} dollars`)
}


//Four parts of a function
//1. Name
//2. Inputs
//3. Logic
//4. Output

//Create a function that subtracts two values

function subtract(numOne, numTwo){
    let answer = numOne - numTwo;
    return answer;
}

console.log(subtract(3, 1));
// console.log(answer);
// console.log(numOne);


// console.log(name);
// let name = "Kaleb";

//Create a function that multiplies three numbers: a, b, and c

//Create a "My name is..."
function myNameis(name){
    console.log(`My name is ${name}`);
}

myNameis("What?")
myNameis("Who?")
myNameis("(chicka-chicka) Slim Shady")

//Create a Celsius to farenheit conversion function
// function cToF(c){
//     return 1.8 * c + 32;
// }

//Function Expression
// const name = function(input){logic, output}
// const cToF = function(c){return 1.8 * c + 32;}

//Lambda
// input => logic
const cToF = c => 1.8 * c + 32;

console.log("Celsius    Farhrenheit")
for(let c = 0; c <= 100; c++){
    let f = cToF(c);
    // console.log(c, f);
}



// Normal
function circumference(radius){
    let answer = 2 * Math.PI * radius;
    return answer;
}

//Expression 
// const circumference = function(radius){return 2 * Math.PI * radius;}

//Lambda
// const circumference = radius => 2 * Math.PI * radius;


// Default Parameters
function speak(message = "Hola Mundo"){
    console.log(message);
}

speak("Hello World")
speak()

function displayMoneyAmount(amount, symbol="$"){
    console.log(`Amount: ${symbol}${amount}`)
}

displayMoneyAmount(45)
displayMoneyAmount(45, "&")


// prompt()
// prompt("Hello")
// prompt("Hello", "default")


//Spread Operator
let data = [1,2,3,4];
console.log(data);
console.log(...data);
console.log(data[0], data[1], data[2], data[3])

function sum(x, y, z, w){
    return x + y + z + w;
}

let answer = sum(data[0], data[1], data[2], data[3]);
console.log(answer);

answer = sum(...data)
console.log(answer)
```