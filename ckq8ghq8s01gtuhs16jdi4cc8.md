---
title: "Building Simple Javascript Projects"
seoTitle: "Building Simple Javascript Projects"
datePublished: Sun May 08 2022 10:25:00 GMT+0000 (Coordinated Universal Time)
cuid: ckq8ghq8s01gtuhs16jdi4cc8
slug: building-simple-javascript-projects
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1624391002219/ocrlYgiWB.png
tags: web-development, 2articles1week, 7daystreak, thw-web-apps, thw-mobile-apps

---

<head> <meta name="monetization" content="$ilp.uphold.com/fXgYL9dgXzHk"> </head>
# Introduction

> 
The concepts are easy and understandable. I have explained the meaning of the different functions and methods in the comments. For better understanding, I would suggest you to go through the code and practice by executing it.

## Reversing Text

** index.html **
```
<html>
<body>
  <div id="container">
    <br /><br />
    <div>
      <label id="input_text">Reversing Text</label>
      <input id="text_field" type="text" maxlength="20" placeholder="Enter the text here!"></input>
    </div>
    <div>
      <button id="submit" type="button">ENTER</button>
    </div>
    <div>
      <p id="answer"></p>
    </div>
  </div>
</body>
</html>
```

** style.css **
```
body,
html {
  background: #ba1c2e;
  font-family: cursive;
  height: 100%;
  margin: 0;
}

#container {
  background: #f7f7f7;
  font-family: cursive;
  text-align: center;

  width: 480px;
  height: 100%;
  padding: 10px 20px;
  border: 2px solid tomato;
  border-radius: 20px;
  outline: dashed lightgray;
  margin: 200px auto;
}

input {
  color: #f74a5c;
  font-size: 24px;
  font-family: cursive;
  background-color: lightgray;
  text-align: center;
  width: 100%;
  box-sizing: border-box;
  border: 3px solid gray;
  margin: 60px auto;
}

#input_text {
  background: #f74a5c;
  font-family: cursive;
  font-size: 34px;
  color: black;
  padding: 3px 10px;
  border-radius: 5px;
  margin: 100px auto;
}

#text_field {
  padding: 50px 70px;
}

#answer {
  color: #f74a5c;
  font-size: 24px;
  font-family: cursive;
  text-align: center;

  padding: 5px 5px;
}

#submit {
  font-family: cursive;
  color: black;
  background-color: #f74a5c;
  font-size: 20px;
  height: 100%;
  letter-spacing: 1px;
}
```
** script.js **
```
// Let's start with writing the function
function reversing() {
// Fetching the items using the ID
// and assigning to the declared variable.
  var text_field = document.getElementById("text_field").value;
  var answer = document.getElementById("answer");
// Using the if-else looping statement.
// Here, we read the characters entered and stored in text_field,
// if there is no text entered,
// i.e. no. of characters entered is less than 1, 
// then answer appearing on the screen will be textbox must contain characters.
// If that condition was false,
// then the else statement executes.
// Here, the array is read and stored and then reversed.
// The reversed string is printed on the screen.
  if (text_field.length < 1) {
    answer.textContent = "Textbox must contain characters!";
  } else {
    var array = text_field.split("");
    var text = array.reverse();
    var input_text = text.join("");
    answer.textContent = "Here's your reversed text " + '"' + input_text + '"';
  }
}
// All the above action starts when the submit button is clicked.
var submit = document.getElementById("submit"); 
// This is where the function is called, and all the execution starts.
// All starts when the event "click" happens,
// the function is walked through and then condition is made false after all execution. 
// That's where the code stops. 
submit.addEventListener("click", reversing, false);

```
### Output

<iframe height="600" style="width: 100%;" scrolling="no" title="Reversing Text" src="https://codepen.io/bhumikhokhani/embed/dyvEZLB?height=265&theme-id=dark&default-tab=result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/bhumikhokhani/pen/dyvEZLB'>Reversing Text</a> by Bhumi Khokhani
  (<a href='https://codepen.io/bhumikhokhani'>@bhumikhokhani</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

<hr></hr>

## Simple Calculator

** index.html **

```
<body>
  <div class="container">
  </div>
  <div id="containing">
    <div class="calc">
      <center>
        <p><b style="font-size: 30px;">Calculator</b></p>
      </center>
      <span class="btn">C</span>
      <div class="equation"></div>
    </div>
    <div class="clicked">
      <span>7</span>
      <span>8</span>
      <span>9</span>
      <span class="operator">+</span>
      <span>4</span>
      <span>5</span>
      <span>6</span>
      <span class="operator">-</span>
      <span>1</span>
      <span>2</span>
      <span>3</span>
      <span class="operator">÷</span>
      <span>0</span>
      <span>.</span>
      <span class="selection">=</span>
      <span class="operator">x</span>
    </div>
  </div>
</body>
```

** style.css **

```
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font: bold 14px Arial, sans-serif;
}
html {
  height: 100%;
  background: white;
  background: url(https://i.pinimg.com/564x/81/a0/65/81a065a50ecabac9fd7f860a4af72c76.jpg);
  background-size: cover;
}
#containing {
  width: 325px;
  height: auto;
  margin: 10px auto 100px;
  padding: 20px 20px 19px;
  background: #9dd2ea;
  background: linear-gradient(#9dd2ea, #8bceec);
  border-radius: 3px;
  box-shadow: 0px 4px #009de4, 0px 10px 15px rgba(0, 0, 0, 0.2);
}
.calc span.btn {
  float: left;
}
.calc .equation {
  height: 40px;
  width: 212px;
  float: right;
  padding: 0 10px;
  background: rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  box-shadow: inset 0px 4px rgba(0, 0, 0, 0.2);
  font-size: 17px;
  line-height: 40px;
  color: white;
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.2);
  text-align: right;
  letter-spacing: 1px;
}
.clicked,
.calc {
  overflow: hidden;
}
.clicked span,
.calc span.btn {
  float: left;
  position: relative;
  top: 0;
  cursor: pointer;
  width: 66px;
  height: 36px;
  background: white;
  border-radius: 3px;
  box-shadow: 0px 4px rgba(0, 0, 0, 0.2);
  margin: 0 7px 11px 0;
  color: #888;
  line-height: 36px;
  text-align: center;
  user-select: none;
  transition: all 0.2s ease;
}
.clicked span.operator {
  background: #fff0f5;
  margin-right: 0;
}
.clicked span.selection {
  background: #b595ed;
  box-shadow: 0px 4px #a17be3;
  color: white;
}
.calc span.btn {
  background: #ff9fa8;
  box-shadow: 0px 4px #ff7c87;
  color: white;
}
.clicked span:hover {
  background: #89f6d0;
  box-shadow: 0px 4px #54d39e;
  color: white;
}
.clicked span.selection:hover {
  background: #9976d6;
  box-shadow: 0px 4px #7650b8;
  color: #ffffff;
}
.calc span.btn:hover {
  background: #f68991;
  box-shadow: 0px 4px #d3545d;
  color: white;
}
.clicked span:active {
  box-shadow: 0px 0px #54d39e;
  top: 4px;
}
.clicked span.selection:active {
  box-shadow: 0px 0px #7650b8;
  top: 4px;
}
.calc span.btn:active {
  top: 4px;
  box-shadow: 0px 0px #d3545d;
}
.container {
  padding-top: 170px;
  padding-left: 90px;
  text-align: center;
}
.container p,
.container a {
  text-decoration: none;
  color: black;
}
```

** script.js **

```
// Here we use the querySelectorAll to store the equation entered.
var keys = document.querySelectorAll("#containing span");
// Operators are stored in the variable.
var operators = ["+", "-", "x", "÷"];
// By default, the decimal value added is set to false,
// As we consider having integer values. It can be changed.
var decimalAdded = false;
// For loop to read the entire equation.
for (var i = 0; i < keys.length; i++) {
// We use the event Handler here, onClick function.
  keys[i].onclick = function (e) {
    var input = document.querySelector(".equation");
    var inputVal = input.innerHTML;
    var btnVal = this.innerHTML;
// If C is selected, it means  the screen need to be again back to blank.
// That is what happens here, else, if the = is selected,
// The equation is read and operations are performed.
    if (btnVal == "C") {
      input.innerHTML = "";
      decimalAdded = false;
    } else if (btnVal == "=") {
      var equation = inputVal;
      var lastChar = equation[equation.length - 1];
      equation = equation.replace(/x/g, "*").replace(/÷/g, "/");
      if (operators.indexOf(lastChar) > -1 || lastChar == ".")
        equation = equation.replace(/.$/, "");
      if (equation) input.innerHTML = eval(equation);
      decimalAdded = false;
    } else if (operators.indexOf(btnVal) > -1) {
      var lastChar = inputVal[inputVal.length - 1];
      if (inputVal != "" && operators.indexOf(lastChar) == -1)
        input.innerHTML += btnVal;
      else if (inputVal == "" && btnVal == "-") input.innerHTML += btnVal;
      if (operators.indexOf(lastChar) > -1 && inputVal.length > 1) {
        input.innerHTML = inputVal.replace(/.$/, btnVal);
      }
      decimalAdded = false;
    } else if (btnVal == ".") {
      if (!decimalAdded) {
        input.innerHTML += btnVal;
        decimalAdded = true;
      }
    } else {
      input.innerHTML += btnVal;
    }
    e.preventDefault();
  };
}

```
### Output

<iframe height="700" style="width: 100%;" scrolling="no" title="Simple Calculator" src="https://codepen.io/bhumikhokhani/embed/PopbzaK?height=265&theme-id=dark&default-tab=result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/bhumikhokhani/pen/PopbzaK'>Simple Calculator</a> by Bhumi Khokhani
  (<a href='https://codepen.io/bhumikhokhani'>@bhumikhokhani</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

<hr></hr>


> 
If you found working with Javascript interesting, you can check my other codepens, and give it a shot. Practice. Learn. Discover.
https://codepen.io/bhumikhokhani/

<hr></hr>

# Wrapping Up

Hope this article gave you some practice and grip on working with Javascript.
Feel free to put up any questions if you have/had. I will try my best to answer them.

Also, you can leave you suggestions in the comment section and give a reaction if you enjoyed reading it 💖 <br>
Feel free to connect with me on  [LinkedIn](https://www.linkedin.com/in/bhumikhokhani/)  |  [Twitter](https://twitter.com/bhumikhokhani) 
<br>
> 
If you like my work, you can extend your support by buying me a ☕. Thank you!

<a href="https://www.buymeacoffee.com/bhumikhokhani"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=bhumikhokhani&button_colour=FF5F5F&font_colour=ffffff&font_family=Cookie&outline_colour=000000&coffee_colour=FFDD00"></a>