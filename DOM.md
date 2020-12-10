# DOM

## Part One
```javascript

console.log(document)

// console.log(document.getElementById("firstItem"))
// console.log(document.getElementById("firstItem").innerText)

// document.getElementById("firstItem").innerText = "Kaleb"
// document.getElementById("secondItem").innerText = "Michael"
// document.getElementById("thirdItem").innerText = "Burd"
// document.getElementById("fourthItem").innerText = "1st"

// console.log(document.getElementsByTagName("ul")[0].innerHTML += "<li>Another Listitem</li>")


// for(let i = 0; i < 10; i++){
//     document.getElementsByTagName("ul")[0].innerHTML += "<li>" + i + "</li>"
// }

// console.log(document.getElementsByTagName("ul")[0].innerHTML)

document.getElementById("title").innerText = "Kaleb is da best";

document.getElementsByTagName("h1")[0].innerText = "Kaleb is da best";

let names = ["Denae", "Hakim", "Elu", "Kaleb"]

// for(let i = 0; i < names.length; i++){
//     // document.getElementById("authors").innerHTML += `<li>${names[i]}</li>`
//     document.getElementById("authors").innerHTML += names[i]
//     if(i > 0){
//         document.getElementById("authors").innerHTML += "<br>"
//     }
// }

console.log(document.getElementById("authors").innerHTML);


let skills = ["Nunchuck", "Bow Hunting", "Computer Hacking"]

for(let i = 0; i < skills.length; i++){
    document.getElementById("skills").innerHTML += `<li>${skills[i]}</li>`;
}


//Search by Class
let elements = document.getElementsByClassName("text")
console.log(elements)

//Query Selectors
let temp = document.querySelector("#title.text")
console.log(temp)

let img = document.getElementById("pic")
console.log(img)

// let size = +prompt("How big do you want your img?")

// img.height = size
// img.width = size


let choice = prompt("Do you like blue?")

if(choice === "Y"){
img.src = ""
}

let flag = true;

function toggle(){
    
    let color = (flag) ? "salmon" : "cyan";
    let src = (flag) ? "blueCheckIcon.png" : "The_Eminem_Show.jpg";
    let size = (flag) ? 500 : 250;
    flag = !flag;

    document.getElementById("title").style.backgroundColor = color;
    let img = document.getElementById("pic")
    img.height = size
    img.width = size
    img.src = src
}
```

```html
<!DOCTYPE html>
<html lang="en">
<body>

    <h1 id="title" class="text"></h1>

    <!-- <ul id="authors"></ul> -->
    <div id="authors" class="text"></div>

    <ul id="skills">

    </ul>

    <img id="pic" src="The_Eminem_Show.jpg" height="500" width="500">

    <button onclick="toggle()">Click Me</button>

</body>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <script src="script.js"></script>
</head>
</html>
```

## Part 2
```javascript

console.log(document.getElementsByTagName("ul"));

let unorderList = document.getElementById("albums");
console.log(unorderList)

unorderList.innerHTML += "<li>The Slim Shady LP</li>";
unorderList.innerHTML += "<li>Kamakazi</li>";
unorderList.innerHTML += "<li>Recovery</li>";


// Create a new element
let listItem = document.createElement("li")
listItem.innerText = "The Marshel Matters LP 2"
console.log(listItem)

// Append an element
unorderList.appendChild(listItem)


// let elements = document.getElementsByTagName("h1");
// console.log(elements[0])

let title = document.getElementById("title")
console.log(title)


let author = document.createElement("p");
author.innerText = "By: Kaleb"
document.body.appendChild(author);

let listItems = unorderList.childNodes

console.log(listItems[1])
unorderList.removeChild(listItems[1])

document.body.removeChild(unorderList)


// Add 5 items to a list 
// 1 -> 5, Alpha -> Echo

//Prompt the user for a number and delete that elemnt form the list

let nums = document.getElementById("nums");
console.log(nums)

let item;
for(let i = 1; i <= 5; i++){
    item = document.createElement("li");
    item.innerText = i;
    nums.appendChild(item)
}

// let userNum = Number(prompt("Enter a number to delete"));


//DOM Tree
let ul = document.getElementById("nums");
let li1 = ul.childNodes[0];
console.log(li1.nextSibling.nextSibling)

console.log(li1.parentNode)


// Timeout
function alertMe(){
    nums.removeChild(nums.childNodes[userNum]);
}
// setTimeout(alertMe, 3000);

function hola(){ 
    console.log("Hello");
}

//Interval
// let log = setInterval(hola, 500);

//Events
let button2 = document.getElementById("secondButton");
button2.addEventListener('click', hola)
```

```html
<!DOCTYPE html>
<html lang="en">

    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Document</title>
    </head>

    <body>
        <h1 id="title">Eminem Fan Page</h1>
        <h2>Albums</h2>
        <ul id="albums"></ul>
        <ul id="nums"></ul>
        <button id="secondButton">Click Me TOO!</button>

        <script src="script.js"></script>

        <button onclick="hola()">Click Me!</button>
    </body>

</html>
```