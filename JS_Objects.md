```JavaScript

// Primatives
// let name = "Kaleb"
// let age = 87;
// let isMarried = true;

// Empty Object
let person = {}

person = {
    name: "Kaleb",
    age: 87,
    isMarried: true
}

// Log obj
console.log(person)

// Dot notation
console.log(person.isMarried);
console.log(person.age)
console.log(person.name);

// Math Obj
let answer = Math.max(4, 0);

// Bracket Notation
console.log()

// Update attributes
person.age = 56;
console.log(person.age)

person["age"] = 21;
console.log(person.age);

console.log(person.age);

//Adding new attributes
person.lastName = "Burd"
console.log(person);

let dog = {
    name: "Gracie",
    age: 3,
    isMarried: false
}

console.log(person, dog)

dog.isMarried = true;
person.age++;

console.log(person, dog)

//Exercise
// 1. Create an empty obj
// 2. Create an atrribute with a value
// 3. Model your driver's license

let license = {
    state: "DE",
    firstName: "Denae",
    lastName: "Griggs",
    organDoner: true,
    dlNo: 2354282,
    dob: "6/20/86",
    exp: "12/9/2022",
    height: 6.0,
    img: "https://avatars2.githubusercontent.com/u/12243135?s=400&u=243a336abe3e8803d9625fc6ac642ed9eec223de&v=4"
};

// document.getElementById("pic").setAttribute("src", license.img)


// license.state = prompt("What is your state")

console.log(license)

// Arrays of Obj
let cars = [
    {
        model: "Jetta",
        year: 2012
    },
    {
        model: "Camero",
        year: 1978
    },
    {
        model: "Delorean",
        year: 1984
    }
]

console.log(cars)
console.log(cars[2]);
console.log(cars[2]["year"])

// let attr = prompt("What do you want to see?")
// console.log(cars[2][attr]);

//Exercise 2: Rectangle

function loadRectangleData(rectangle){
    rectangle.length = Number(prompt("Enter Length: "));
    rectangle.width = Number(prompt("Enter Width: "));
    return rectangle;
}

function calcArea(rectangle){
    return rectangle.length * rectangle.width;
}

function calcPerm(rectangle){
    return 2 * (rectangle.length + rectangle.width)
}

function isSquare(rectangle){
    return rectangle.length === rectangle.width;
}


let rectangle = {};

// rectangle = loadRectangleData(rectangle);

console.log(rectangle);
console.log(calcArea(rectangle))
console.log(calcPerm(rectangle))

// let pokemon = {id:1,name:"Bulbasaur",img:"https://img.pokemondb.net/sprites/bank/normal/bulbasaur.png"}

// let img = document.createElement("img");
// img.setAttribute("src", pokemon.img);


// let card = document.createElement("div");
// card.innerText = pokemon.name + " " + pokemon.id;
// card.appendChild(img)

// document.getElementById("content").appendChild(card);


function renderPokemon(pokemon){
    return( 
        `<div class="card m-3" style="width: 10rem;">
            <div class="card-header">#00${pokemon.id} ${pokemon.name}</div>
            <img class="card-img-top" src="${pokemon.img}" alt="Card image cap">
        </div>`
    )
}

function buildAll(pokemonArray){

    console.log(pokemonArray)

    let html = "";

    for(let i = 0; i < pokemonArray.length; i++){
        html += renderPokemon(pokemonArray[i]);
    }

    document.getElementById("content").innerHTML = html;

}




let xhttp = new XMLHttpRequest();
xhttp.onreadystatechange = function() {
  if (this.readyState == 4 && this.status == 200) {
    buildAll(JSON.parse(this.responseText))
  }
};

xhttp.open("GET", "http://localhost:3000/pokemons", true);
// xhttp.send();

let post = {
    user: "Kaleb",
    date: "1/2/1999",
    time: "1:20 AM",
    message: "What uuppp!",
    likes: 45,
    shares: ["DaRon", "Hakim", "Gee"],
    comments: []
}

function sharePost(user, post){
    post.shares.push(user)
    return post
}

post = sharePost("John", post)
console.log(post)

function addComment(post, comment){
    post.comments.push(comment);
    return post;
}

function buildComment(user, message){
    return (
        {
            user: user,
            message: message
        }
    );
}

let comment = buildComment("Hakim", "Not much")
console.log(comment);

post = addComment(post, comment);
console.log(post)

// Part 2
// person = {
//     name: "Kaleb",
//     age: 87,
//     isMarried: true
// }

class Person {

    constructor(startingAge, startingName, startingGender){
        this.age = startingAge;
        this.name = startingName;
        this.gender = startingGender;
    }

    //getters or accessors
    getAge(){
        return this.age;
    }

    getName(){
        return this.name;
    }

    getGender(){
        return this.gender;
    }

    //settors or mutators
    setAge(newAge){
        this.age = newAge;
    }

    setName(newName){
        this.name = newName;
    }

    setGender(gender){
        this.gender = gender;
    }

    haveBirthday(){
        this.age++
    }

}


let child = new Person(24, "Kaleb", "Male");
console.log(child);

// Access attributes
console.log(child.age);
console.log(child["name"]);
console.log(child.getAge())

console.log(console)
console.log(Math.abs(Math.E))

// Update info
child.gender = "Female";
child["name"] = "Michelle"
child.setAge(65);

console.log(child);

for(let i = 0; i < 10; i++){
    child.haveBirthday()
}   
console.log(child.age);

class BankAccount{

    constructor(){
        this.balance = 0;
        this.interest = .08;
    }

    deposit(amount){
        this.balance += amount;
    }

    withdraw(amount){
        if(this.balance > amount){
            this.balance -= amount;
        }
    }

    getBalance(){
        return this.balance;
    }

    applyInterest(){
        this.balance *= 1 + this.interest;
    }

}

let savingsAccount = new BankAccount();
let retirementAccount = new BankAccount();


// savingsAccount.deposit(150);
// savingsAccount.deposit(200);
// console.log(savingsAccount.getBalance())

// savingsAccount.applyInterest()
// console.log(savingsAccount.getBalance())

// console.log(retirementAccount.getBalance())

for(let i = 20; i <= 65; i++){
    retirementAccount.deposit(6000);
    retirementAccount.applyInterest()
}

console.log(retirementAccount.getBalance())


// Rectangle class
// + width
// + length
// + getters, setters
// + calcArea()
// + calcPermimeter()

class Rectangle {

    constructor(width, length){
        this.width = width;
        this.length = length;
    }

    getWidth(){
        return this.width;
    }

    getLength(){
        return this.length;
    }

    setWidth(width){
        this.width = width;
    }

    setLength(length){
        this.length = length;
    }

    getPerimeter(){
        return 2 * (this.length + this.width);
    }

    getArea(){
        return this.length * this.width;
    }

}

console.log("".slice(0, -1))


// Tweet Class
// + message => max length of 140
// + getMessage()
// + addLetter(letter)
// + removeLetter()

class Tweet {

    MAX_CHAR_COUNT = 4;

    constructor(){
        this.message = "";
    }

    addLetter(letter){
        if(this.message.length < this.MAX_CHAR_COUNT){
            this.message += letter;
        }
    }

    removeLetter(){
        this.message = this.message.slice(0, -1);
    }

    getMessage(){
        return this.message;
    }

}

let tweet = new Tweet();

for(let i = 0; i < 7; i++){
    tweet.addLetter("A");
    console.log(tweet.getMessage())
}

for(let i = 0; i < 7; i++){
    tweet.removeLetter();
    console.log(tweet.getMessage())
}


```