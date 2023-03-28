---
title: "Getting Started with JavaScript - 1"
seoTitle: "Getting started with Javascript"
datePublished: Wed May 04 2022 10:24:39 GMT+0000 (Coordinated Universal Time)
cuid: ckq6cfn7v09d8ubs1ce8r8vnt
slug: getting-started-with-javascript-1
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1624263209155/yhXUAq_71.png
tags: javascript, web-development, webdev, beginners, 7daystreak

---

<head> <meta name="monetization" content="$ilp.uphold.com/fXgYL9dgXzHk"> </head>
## What is JavaScript?

> 
Javascript is well known as the programming language for the Web. It's a client-side scripting language.

## What is its function?

> 
Basically, javascript functions when some action is performed by the client. The actions can be hovering over using a mouse, clicking on something, scrolling, anything based on what's coded.

## Syntax?
```
<script type = “text/javascript”> 
// Enter the code here.
</script>
```
```
   // Linking an external javascript file.
  <script src="example.js"></script>
```
## Now let's dive into Javascript basics.
** - Comments **
```
// Single line comments are typed here
/* Multi line comments are typed in this. 
    Comments are used to explain the code, 
    Basically, to make the code understandable to the reader.*/
```
** - Variables **

These hold values and are used to perform different operations.

3 Types:

1) **var** - Frequently used. Values can be assigned can be modified over the operations and working. Works only in the functions its declared in.
```
var example = "value";
```

2) **const** - These values can't be modified again and again. The values assigned in the start remains unchanged until the end.
```
const example = "value";
```

3) **let** - Values assigned can change, works only inside the particular block.
```
let example = "value";
```

**- Datatypes**

<table>
  <tr>
    <th>Datatype</th>
    <th>Example</th>
    <th>Syntax</th>
  </tr>
  <tr>
    <td>Number</td>
    <td>300.3</td>
    <td>``` var roll_no = 10;   ```</td>
  </tr>
  <tr>
    <td>Null</td>
    <td>null</td>
    <td>``` var example = null;  ```</td>
  </tr>
  <tr>
    <td>Undefined</td>
    <td>undefined</td>
    <td>``` var example; 
                   typeof example;    ```</td>
  </tr>
  <tr>
    <td>String</td>
    <td>"Hello"</td>
    <td>``` var text = "Hello";  ```</td>
  </tr>
  <tr>
    <td>Boolean</td>
    <td>True/False</td>
    <td>``` var answer = false;   ```</td>
  </tr>
  <tr>
    <td>Symbol</td>
    <td>Giovanni Rovelli</td>
    <td>``` var example = /()/; ```</td>
  </tr>
</table>

**- Objects**

It's another type of data-type which stores in key-value pair format.

```
var student = {
// Here, name,roll,dob are the keys. 
// Opposite to them are their respective values.
  name : Bhumi Khokhani,
  roll : 10,
  dob : "2000-03-27",
  age : function() {
  // Code written for the function
  }; //Method
}
```

**- Functions**

Set of code written to perform a specific task. It runs when it's called. Having functions also increases the reusability of code.

Two steps to create as function:

** 1) Define it **

** 2) Call it **

```
//Defining the function.
function function_name ( parameters ) {
//Block of Code
var abc=parameters;
return abc; //returns this value at the end of the function. It's optional.
}
function_name(parameters); //Calling the function.
```

**- Arrays**

A group of similar datatypes is called an array. We can access by referring to the index number.

**Syntax**

```
// First way of defining an array
datatype array_name=["value1", "value2", "value3", ...];
//Second way of defining an array
datatype array_name = [];
array_name[0] = "value1";
array_name[1] = "value2";
array_name[2] = "value3";
//Third way of defining an array
datatype array_name = new Array("value1", "value2", "value3");
// Accessing the array elements
datatype variable_name = array_name[index_value];
// Altering a value of array
array_name[index_value] ="new value";
// Printing the array elements
for (var i = 0; i < array_name.length; i++) {
     console.log(array_name[i]);
}
```

**Functions on Array**

<table>
  <tr>
    <th>Function</th> 
    <th>Definition</th>
    <th>Example</th>
  </tr>
  <tr>
    <td>concat()</td>
    <td>Used for concatenating arrays.</td>
    <td>``` array_name.concat(arr1, arr2);   ```</td>
  </tr>
  <tr>
    <td>join()</td>
    <td>Joining all elements in the particular array giving back a string.</td>
    <td>``` array_name.join("*");  ```</td>
  </tr>
  <tr>
    <td>indexof()</td>
    <td>Returns the first position (index) of an array.</td>
    <td>``` array_name.indexof();     ```</td>
  </tr>
  <tr>
    <td>lastindexof()</td>
    <td>Returns the last position (index) of an array.</td>
    <td>``` array_name.lastindexof();  ```</td>
  </tr>
  <tr>
    <td>sort()</td>
    <td>Sorting of array elements in alphabetical order.</td>
    <td>``` array_name.sort();    ```</td>
  </tr>
  <tr>
    <td>reverse()</td>
    <td>Sorting of array elements in reverse alphabetical order.</td>
    <td>``` array_name.reverse(); ```</td>
  </tr>
 <tr>
    <td>shift()</td>
    <td>Popping of first element, and returning the value of the popped element.</td>
    <td>``` array_name.shift(); ```</td>
  </tr>
 <tr>
    <td>unshift()</td>
    <td>Pushing of element in the beginning of the array.</td>
    <td>``` array_name.unshift("value"); ```</td>
  </tr>
 <tr>
    <td>splice()</td>
    <td>Used for adding items to te array, it returns the deleted items of the array. // pushing index; no_of items to be deleted; item value</td>
    <td>``` array_name.splice(index1, no._of "values"); ```</td>
  </tr>
 <tr>
    <td>slice()</td>
    <td>Derives a new array form the existing array. Slicing doesn't affect the already existing array. // index1 slicing begins, index2 slicing end.</td>
    <td>``` array_name.slice(index1, index2); ```</td>
  </tr>
 <tr>
    <td>toString()</td>
    <td>Converts the array separated by commas to a single string.</td>
    <td>``` array_name.toString(); ```</td>
  </tr>
 <tr>
    <td>push()</td>
    <td>Pushing an item to the end of the array.</td>
    <td>``` array_name.push(item); ```</td>
  </tr>
 <tr>
    <td>pop()</td>
    <td>Popping an item from the end of the array.</td>
    <td>``` array_name.pop(); ```</td>
  </tr>
</table>

**- Operators**

1) **Basic Operators**

<table>
  <tr>
    <th>Operator</th> 
    <th>Definition</th>
    <th>Example</th>
  </tr>
  <tr>
    <td>+</td>
    <td>Addition.</td>
    <td>``` var1 = var2 + var3;   ```</td>
  </tr>
  <tr>
    <td> - </td>
    <td>Subtraction.</td>
    <td>``` var1 = var2 - var3; ```</td>
  </tr>
  <tr>
    <td>*********</td>
    <td>Multiplication.</td>
    <td>var1 = var2 * * * * * * * * * var3;</td>
  </tr>
  <tr>
    <td> / </td>
    <td>Division.</td>
    <td>``` var1 = var2 / var3; ```</td>
  </tr>
<tr>
    <td>%</td>
    <td>Modulus.</td>
    <td>``` var1 = var2 % var3;    ```</td>
  </tr>
  <tr>
    <td>++</td>
    <td>Increment.</td>
    <td>``` var1 ++;    ```</td>
  </tr>
  <tr>
    <td>--</td>
    <td>Decrement.</td>
    <td>``` var1 --;    ```</td>
  </tr>
</table>

2) **Bitwise Operator**

<table>
  <tr>
    <th>Operator</th> 
    <th>Definition</th>
    <th>Example</th>
  </tr>
  <tr>
    <td>&</td>
    <td>AND</td>
    <td>``` var1 & var2 ```</td>
  </tr>
  <tr>
    <td> | </td>
    <td>OR</td>
    <td>``` var1 | var2 ```</td>
  </tr>
  <tr>
    <td>~</td>
    <td>NOT.</td>
    <td>```~ var1```</td>
  </tr>
  <tr>
    <td> ^ </td>
    <td>XOR</td>
    <td>``` var1 ^ var2 ```</td>
  </tr>
  <tr>
    <td> << </td>
    <td>	Left Shift </td>
    <td>``` var1 << var2```</td>
  </tr>
  <tr>
    <td>>></td>
    <td>Right Shift </td>
    <td>```var1>>var2```</td>
  </tr>
</table>

3) **Comparison Operator**

<table>
  <tr>
    <th>Operator</th> 
    <th>Definition</th>
    <th>Example</th>
  </tr>
  <tr>
    <td>==</td>
    <td>Equals to</td>
    <td>``` var1 == var2 ```</td>
  </tr>
  <tr>
    <td> === </td>
    <td>Equal to or type</td>
    <td>``` var1 === var2 ```</td>
  </tr>
  <tr>
    <td>!=</td>
    <td>Not equal to</td>
    <td>``` var1 != var2```</td>
  </tr>
  <tr>
    <td> !== </td>
    <td>Not equal to or type</td>
    <td>``` var1 !== var2 ```</td>
  </tr>
  <tr>
    <td> < </td>
    <td>Less than </td>
    <td>``` var1 < var2```</td>
  </tr>
  <tr>
    <td>></td>
    <td>Greater than </td>
    <td>```var1>var2```</td>
  </tr>
  <tr>
    <td> ? </td>
    <td>Ternary Operator </td>
    <td>``` var1 ? var2```</td>
  </tr>
  <tr>
    <td><=</td>
    <td>Less than or equal to </td>
    <td>```var1<=var2```</td>
  </tr>
  <tr>
    <td>>=</td>
    <td>Greater than or equal to </td>
    <td>```var1>=var2```</td>
  </tr>
</table>

4) **Logical Operators**

<table>
  <tr>
    <th>Operator</th> 
    <th>Definition</th>
    <th>Example</th>
  </tr>
  <tr>
    <td>&&</td>
    <td>Logical AND</td>
    <td>``` var1 && var2 ```</td>
  </tr>
  <tr>
    <td> || </td>
    <td>Logical OR</td>
    <td>``` var1 || var2 ```</td>
  </tr>
  <tr>
    <td> ! </td>
    <td>Logical NOT</td>
    <td>``` !(var1 == var2) ```</td>
  </tr>
</table>

*Yet, Javascript consists of many different attributes, functions, methods etc., which I will cover in the next blog.*

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