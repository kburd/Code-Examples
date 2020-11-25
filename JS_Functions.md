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
alert(solution);


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
```