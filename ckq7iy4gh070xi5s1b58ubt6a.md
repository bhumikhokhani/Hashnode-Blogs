---
title: "Getting Started with JavaScript - 2"
seoTitle: "Getting started with Javascript"
datePublished: Fri May 06 2022 10:24:51 GMT+0000 (Coordinated Universal Time)
cuid: ckq7iy4gh070xi5s1b58ubt6a
slug: getting-started-with-javascript-2
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1624293882390/oHsvvfiBv.png
tags: web-development, beginners, 7daystreak, thw-web-apps, thw-mobile-apps

---

<head> <meta name="monetization" content="$ilp.uphold.com/fXgYL9dgXzHk"> </head>
> 
In previous blog we learnt what javascript is, different datatypes, operators, methods etc., in it. So now, let's continue learning further, the basics of Javascript.

## What is a DOM?
DOM, **Document Object Model**. When a particular web page loads, by default, a DOM is created. Basically, it's the** code of the page structure**. This model is constructed as a **tree of objects**. We can find these objects by searching for its **id, name or tags**. 

## What is a Node?
Every single item in the DOM tree is known as a node. Now it's important to know that, the node present in DOM tree can be a **element **or a **text**.

## Which are the different kinds of node?
** 1) Child Node:** A node derived from it's parent. There can be only one parent node.

** 2) Sibling Node: **A node which shares the same parent node.

** 3) Parent Node:** A node having a child node. This can be one or many.

** 4) Descendant Node:** A node which has nested nodes.

## Fetching items in DOM
**- Using  get**
```
document.getElementByClassName('class_name');
```
```
document.getElementById('id_name');
```
```
document.getElementByTagName('element_name');
```
**- Using Query**
```
document.querySelector('css_selector_name');
```

## Fetching item details
```
node.firstChild;
node.lastChild;
node.childNodes;
node.children;
node.nextSibling;
node.parentNode;
```
## Creating elements
```
document.createElement('sample');
document.createTextNode('Successfully created a Text Node');
node.textContent='Successfully created a Text Content';
```
## Adding a node
```
parentNode.appendChild(node_name);
parentNode.insertAfter(node_name, childNode);
```
## Remove a node
```
parentNode.removeChild(node_name);
```
## Cloning elements
```
node.cloneNode();
```
## Events
```
node.addEventListener('event_name', 'function_name');
node.removeEventListener('event_name', 'function_name');
```
## User Events
** 1) Mouse :** onclick, onhover, onmousemove, oncontextmenu, onmousedown, onmouseenter, onmouseleave, onmouseout, onmouseover.

** 2) Keyboard :** onkeydown, onkeypress, onkeyup.

** 3) Drag:** ondrag, ondrop, ondragstart, ondragend, ondragenter, ondragleave.

** 4) Form:** onfocus, onfocusin, onfocusout, onselect, onchange, oninput, onreset, oninvalid,   onblur,  onsearch,  onsubmit.

** 5) Animation:**  animationstart, animationend, animationiteration.

** 6) Others**

## General Functions
In a single function we can perform several tasks.

### Syntax
```
function function_name(parameters){
//Function Code
}
```

## Functions to get outputs

<table>
  <tr>
    <th>Function</th> 
    <th>Definition</th>
    <th>Example</th>
  </tr>
  <tr>
    <td>alert()</td>
    <td>Displays output in a dialog box that pops up on the screen.</td>
    <td>```alert("Here's the pop-up");```</td>
  </tr>
  <tr>
    <td>prompt()</td>
    <td>Usually used for entering wrong input in the input box.</td>
    <td>``` prompt("This will appear on window", "Default input text")```</td>
  </tr>
  <tr>
    <td>confirm()</td>
    <td>Pops up a dialog box where Yes/No options are to be selected.</td>
    <td>```confirm("Did you understand this concept?");```</td>
  </tr>
  <tr>
    <td>console.log()</td>
    <td>Displayed on the console window when debugged.</td>
    <td>```console.log("This will appear in the console window");```</td>
  </tr>
  <tr>
    <td>document.write()</td>
    <td>Here, we enter the output to the HTML document.</td>
    <td>```document.write("This text is written in the document");```</td>
  </tr>
</table>


## Loops
*Repeating a task a number of times until the given condition is not satisfied.*

** 1) For loop**
  - Initially, the expression execuetes.
  - Next, the condition is checked. If the condition is satisfied, the code in the loop is executed, else the control comes out of the loop to the next statement.
  - After the execution of the code in the loop, either increment/decrement operation takes place.
  - The cycle repeats.

### Syntax
```
for(expression;condition;increment/decrement)
{
//Code
}
```
** 2) While loop**
  - The condition is checked.
  - If the condition is satisfied, the code in it is executed and the loop repeats to re-check the condition and it goes on.
  - If the condition is false, the control comes out of the loop to the next statement.

### Syntax
```
while(condition){
//Code
}
```
** 3) Do-while loop**  
  - The control is in the loop, the code runs.
  - Then the condition is checked, if it satisfies the condition,the code is executed.
  - It loops over again, doing the same.
  - Else the previous action is discarded and control moves out of the loop to the next statement.

### Syntax
```
do{
//Code
}while(condition);
```
## Conditional Statements
These statements let the code run only if certain conditions are met.

** 1) If- else statement**

 - If the condition in if is met, the code block 1 is executed.
 - Else the control is passed onto the else and the code block 2 is executed.

### Syntax
```
if(condition){
//Code block 1
}
else{
//Code block 2
}
```

** 2) Switch Statement**

  - A switch expression is matched with different cases.
  - When the expression matches any case, the code / statement in it is executed.
  - Later, the break statement brings the control out of the switch statement.
  - If no cases match, the default case is executed and control moves out of the switch statement.

### Syntax
```
switch(expression){
case 1: //Code block 1 ;
            break;
case 2: //Code block 2 ;
            break;
case 3: //Code block 3 ;
            break;
default: //Code block n ;
            break;
}
```
 ## this keyword
this keyword behaves as **reference to another object**. Usually used inside a function.
It's implementation changes according to the places its implemented in.
```
//3 cases where we will use this keyword:

var student_name= "Bhumi";
function student_details(){
console.log(this.student_name); 
//this is called inside a function, thus it points to global object.
}
const student = {
stud_name: "Bhumi",
birth_year : 2000,
age : function(){
//Code
}}

student_details(); //called inside a function, this is global object. 
student.age(); // it points to a method, here this is a user object.
student_details.call(student); //Here, first parameter becomes the object, this is user object.
```

## Errors

**1) try** -> Code to be executed when there are no errors.

**2) catch** -> Code to be executed when there are errors.

**3) throw** -> Creating some custom error message.

**4) finally** -> This block is executed, independent of errors present or not.

<br>
***Meet you on my next blog where I will discuss some simple Javascript projects.***

<hr></hr>
## Wrapping Up

Hope this article gave you some basic knowledge on Javascript and it's working.
Feel free to put up any questions if you have/had. I will try my best to answer them.

Also, you can leave you suggestions in the comment section and give a reaction if you enjoyed reading it 💖 <br>
Feel free to connect with me on  [LinkedIn](https://www.linkedin.com/in/bhumikhokhani/)  |  [Twitter](https://twitter.com/bhumikhokhani) 
<br>
> 
If you like my work, you can extend your support by buying me a ☕. Thank you!

<a href="https://www.buymeacoffee.com/bhumikhokhani"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=bhumikhokhani&button_colour=FF5F5F&font_colour=ffffff&font_family=Cookie&outline_colour=000000&coffee_colour=FFDD00"></a>