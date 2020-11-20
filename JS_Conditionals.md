```javascript

//Boolean Data Type
let flag = true; //or false
console.log(flag);

//Relational Operators
let value;

//Greater than
value = 4 > 1;
console.log(value);

//Less than
value = 4 < 1;
console.log(value);

value = 1 < 1;
console.log(value);

//Equals to (abstract equality)
value = (3 == 3);
console.log(value);

value = (6 == 2);
console.log(value);

value = (6 == "6");
console.log(value);

value = (false == 0);
console.log(value);

//Equals to (strict equality)
value = (6 === "6");
console.log(value);

value = (6 === 6);
console.log(value);

// Not equals
value = (4 !== 6); 
console.log(value);

value = (6 !== 6); 
console.log(value);

//Less than or equal to
value = 6 <= 7;
console.log(value);

//Greater than or equal to
value = 7 >= 7;
console.log(value);

value = 6 >= 7;
console.log(value);

// If/else statement
let age = 21;
if(age >= 21){
    console.log("You can vote");
}

else{
    console.log("Next time :(")
}

//Else if
let grade; // = Number(prompt("Enter your grade:"));

if(grade >= 90){
    console.log("Grade: A");
}
else if(grade >= 80){
    console.log("Grade: B");
}
else if(grade >= 70){
    console.log("Grade: C");
}
else if(grade >= 60){
    console.log("Grade: D");
}
else{
    console.log("Grade: F");
}


//Class Solution
// Ask the user to enter a number. Display the following:
let number; // = prompt("Enter a number:");

// "FizzBuzz" if the number is divisable by both
if(number%5 === 0 && number%3 === 0){
    console.log("FizzBuzz");
}

// "Fizz" if the number is divisble by three
else if(number%3 === 0){
    console.log("Fizz");
}

// "Buzz" if the number is divisable by five
else if(number%5 === 0){
    console.log("Buzz");
}


//Kaleb's Solution
// Ask the user to enter a number.
number = prompt("Enter a number:");
let result = "";

// "Fizz" if the number is divisble by three
if(number%3 === 0){
    result += "Fizz";
}

// "Buzz" if the number is divisable by five
if(number%5 === 0){
    result += "Buzz";
}

// Display
console.log(result);


//Logical Operators

//AND operator
value = (6 > 4) && (8 == 8);
console.log(value);

value = (5 > 0) && (3 < 2);
console.log(value);

// Will not evaluate the second expression because the first is already false
value = (1 > 5) && (6 == 6);
console.log(value);

//OR
value = (5 > 4) || (4 < 2);
console.log(value);

value = (5 < 4) || (4 < 2);
console.log(value);

// Will not check the second expression because the first evaluated to true
value = (12 >= 11) || (4 < 2);
console.log(value);

// NOT
value = !(12 > 6);
console.log(value);

//Used as a toggle
let toggle = true;
toggle = !toggle;
console.log(toggle);
toggle = !toggle;
console.log(toggle);

//Ternary

// If/else example
age = 20;
if(age >= 21){
    console.log("You can vote");
}

else{
    console.log("Next time :(")
}

//Equivalent Ternary
let answer = (age >= 21) ? "You can vote" : "Next time :(";
console.log(answer);

//Kaleb's Solution
number = prompt("Enter a number:");
let result = "";
if(number%3 === 0){
    result += "Fizz";
}
if(number%5 === 0){
    result += "Buzz";
}
console.log(result);

let output = (number%3 === 0) ? "Fizz" : "";
output += (number%5 === 0) ? "Buzz" : "";
console.log(output);
```