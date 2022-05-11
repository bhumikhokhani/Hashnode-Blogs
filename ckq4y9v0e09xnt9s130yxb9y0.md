## Building Simple CSS Projects

<head><meta name="monetization" content="$ilp.uphold.com/fXgYL9dgXzHk"></head>
# Introduction
> 
The concepts are easy and understandable. I have explained the meaning of the different attributes and concepts in the comments. For better understanding, I would suggest you to go through the code and practice by executing it.

## Flip-Card

**style.css**
```
body {
  font-family: cursive;
  background-color: #add8e6;
  padding: 25%;
  border: 4px solid black;
  outline: 4px dashed #edb7d6;
}
.flip-card {
  width: 500px;
  height: 500px;
  perspective: 1000px; //Used for the 3D positioning of the element.
}
.flip-card-inner {
  position: relative; 
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 0.6s; //Speed of animation is controlled.
  transform-style: preserve-3d;
}
.flip-card:hover  //Adding some hovering effect
.flip-card-inner {
  transform: rotateY(180deg); //Flips by rotating 180 deg wrt Y-axis.
}
.flip-card-front,
.flip-card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  -webkit-backface-visibility: hidden;
 /* This property comes in picture when there s rotation. 
    It let's us define if you want it's back face to be displayed or not. */
  backface-visibility: hidden; 
}
.flip-card-back {
  background-color: #ffe8f5;
  transform: rotateY(180deg);
  color: #323738;
  border: 2px solid black;
  //Adds thickness, style and color to the outline.
  outline: 3.5px dashed #de97c0; 
}
u {
  text-decoration: underline;
  text-decoration-color: #aee9fc;
  box-shadow: inset 0 -6px 0 0 #8edaf5; //inset shows the physical offset.
}

```
**flip.html**
```
<html>
<head>
  <title>Flip-Flip</title>
</head>
<!-- Linking some external css files --> 
<link rel="stylesheet" href="style.css"/>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
  <body>
    <!-- Calling the division class style rules -->
    <div class="flip-card"> 
      <div class="flip-card-inner">
        <div class="flip-card-front">
          <!-- Adding image using url and giving some inline styles. -->
          <img src="https://tinyurl.com/2rc5ru8k" border="2px" 
          style="width:500px; height:500px; outline: 3.5px dashed #de97c0"> 
        </div>
        <div class="flip-card-back">
          <h1><u>Bhumi Khokhani</u></h1>
          <h3><u>About Me</u></h3>
          <p>Currently in 3rd year, pursuing my BE in CSE from SCEM, Mangalore.
          </p>
          <h3><u>Passion?</u></h3>
          <p>
            Crazy about Blender3D.<br> 
            Love Web-development, graphic designing and Android Development and 
           <br> Content-Writing.
          </p>
          <h3><u>Contact?</u></h3>
          <p>
            <!-- Adding reference links. -->
            <a href="https://www.linkedin.com/in/bhumikhokhani/">
             <!-- Adding icons using external stylesheet and giving some inline styling. -->
            <i class="fa fa-linkedin" style="font-size: 40px; color:#1083e8; 
              border-width: 4px; border-style: solid; border-color: #5ab0fa; 
              border-image: initial; padding: 8px; box-shadow: 0 0 6px #719ECE;">
            </i>
           </a>
         </p>
        </div>
      </div>
    </div>
  </body>
</html>
```
## Output
*Hover over it to see the effect.*

<iframe height="700" style="width: 120%;" scrolling="no" title="Task 3- Flip Flip" src="https://codepen.io/bhumikhokhani/embed/OJpyvXq?height=265&theme-id=dark&default-tab=result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/bhumikhokhani/full/OJpyvXq'>Task 3- Flip Flip</a> by Bhumi Khokhani
  (<a href='https://codepen.io/bhumikhokhani'>@bhumikhokhani</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

<hr></hr>

## Animated VIBGYOR Cube
```
<html>
<head>
  <style>
    div {
      width: 100px; // Cube width
      height: 100px; //Cube height
      position: relative; //Adjusts according to the elements on the screen
      animation-name: cube; //Specifying name of the animation
      animation-duration: 7s; //Total duration of the animation
      background-color: pink;
    }
// Playing around with keyframes. 
// Specifying the styles at different durations of the animation.
    @keyframes cube {
      0% {
        // Color of the Cube
        background-color: violet; 
       // Positioning of the Cube
        left: 0px; 
        top: 0px;
      }
      15% {
        background-color: indigo;
        left: 200px;
        top: 0px;
      }
      30% {
        background-color: blue;
        left: 200px;
        top: 200px;
      }
      45% {
        background-color: green;
        left: 400px;
        top: 200px;
      }
      60% {
        background-color: yellow;
        left: 400px;
        top: 400px;
      }
      75% {
        background-color: orange;
        left: 200px;
        top: 200px;
      }
      100% {
        background-color: red;
        left: 0px;
        top: 0px;
      }
    }
    u {
      color: white;
    }
  </style>
</head>
<body style="background-color:black;">
  <center><u>
      <h1 style="color:white;">Animated VIBGYOR Cube</h1>
    </u></center>
  <div> </div>
</body>
</html>
```

## Output

<iframe height="700" style="width: 100%;" scrolling="no" title="Animated VIBGYOR Cube" src="https://codepen.io/bhumikhokhani/embed/OJpGRZv?height=265&theme-id=dark&default-tab=result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/bhumikhokhani/pen/OJpGRZv'>Animated VIBGYOR Cube</a> by Bhumi Khokhani
  (<a href='https://codepen.io/bhumikhokhani'>@bhumikhokhani</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>
<hr> </hr>

## Responsive CSS Image Gallery

```
<html>
<head>
<!-- Internal Styling --> 
  <style> 
    div.ele {
      margin: 15px; //Adding margins
      border: 2px solid black; //Giving border attributes.
      float: left;
      width: 200px;
    }
    div img {
      width: 100%;
      height: auto;
    }
    div.texts {
      color: black;
      font-size: 17px;
      font-family: Verdana;
      text-align: center;
      padding: 20px;
    }
  </style>
</head>
<!-- Inline Styling -->
<body style="background-color:lightblue"> 
  <center>
    <h1 style="font-family:cursive"><u>Image Gallery</u></h1>
    <center>
      <div class="ele">
        <a target="_blank" href="https://tinyurl.com/4bx3ej77">
          <img src="https://tinyurl.com/4bx3ej77" width="600" height="400">
        </a>
        <div class="texts">Image 1</div>
      </div>
      <div class="ele">
      <!-- Open the image link in a new window. -->
        <a target="_blank" href="https://tinyurl.com/47msc6"> 
    <!-- Fetching image using a url and giving some attributes. -->
          <img src="https://tinyurl.com/47msc6" width="600" height="400">
        </a>
        <div class="texts">Image 2</div>
      </div>
      <div class="ele">
        <a target="_blank" href="https://tinyurl.com/ta88rfnk">
          <img src="https://tinyurl.com/ta88rfnk" width="600" height="400">
        </a>
        <div class="texts">Image 3</div>
      </div>
      <div class="ele">
        <a target="_blank" href="https://tinyurl.com/4bx3ej77">
          <img src="https://tinyurl.com/4bx3ej77" width="600" height="400">
        </a>
        <div class="texts">Image 4</div>
      </div>
      <div class="ele">
        <a target="_blank" href="https://tinyurl.com/47msc6">
          <img src="https://tinyurl.com/47msc6" width="600" height="400">
        </a>
        <div class="texts">Image 5</div>
      </div>
      <div class="ele">
        <a target="_blank" href="https://tinyurl.com/ta88rfnk">
          <img src="https://tinyurl.com/ta88rfnk" width="600" height="400">
        </a>
        <div class="texts">Image 6</div>
      </div>
      <div class="ele">
        <a target="_blank" href="https://tinyurl.com/4bx3ej77">
          <img src="https://tinyurl.com/4bx3ej77" width="600" height="400">
        </a>
        <div class="texts">Image 7</div>
      </div>
      <div class="ele">
        <a target="_blank" href="https://tinyurl.com/47msc6">
          <img src="https://tinyurl.com/47msc6" width="600" height="400">
        </a>
        <div class="texts">Image 8</div>
      </div>
      <div class="ele">
        <a target="_blank" href="https://tinyurl.com/ta88rfnk">
          <img src="https://tinyurl.com/ta88rfnk" width="600" height="400">
        </a>
        <div class="texts">Image 9</div>
      </div>
      <div class="ele">
        <a target="_blank" href="https://tinyurl.com/4bx3ej77">
          <img src="https://tinyurl.com/4bx3ej77" width="600" height="400">
        </a>
        <div class="texts">Image 10</div>
      </div>
      <div class="ele">
        <a target="_blank" href="https://tinyurl.com/47msc6">
          <img src="https://tinyurl.com/47msc6" width="600" height="400">
        </a>
        <div class="texts">Image 11</div>
      </div>
      <div class="ele">
        <a target="_blank" href="https://tinyurl.com/ta88rfnk">
          <img src="https://tinyurl.com/ta88rfnk" width="600" height="400">
        </a>
        <div class="texts">Image 12</div>
      </div>
</body>
</html>
```
## Output
*You will understand the responsiveness when different you change screen size given below. Try changing from 1.0x to 0.5x to 0.25x. You will understand the working.*

<iframe height="500" style="width: 100%;" scrolling="no" title="Responsive CSS Image Gallery" src="https://codepen.io/bhumikhokhani/embed/wvJZzRE?height=265&theme-id=dark&default-tab=result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/bhumikhokhani/pen/wvJZzRE'>Responsive CSS Image Gallery</a> by Bhumi Khokhani
  (<a href='https://codepen.io/bhumikhokhani'>@bhumikhokhani</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>
<hr></hr>

# Wrapping Up

Hope this article gave you some practice and grip on working with CSS.
Feel free to put up any questions if you have/had. I will try my best to answer them.

Also, you can leave you suggestions in the comment section and give a reaction if you enjoyed reading it 💖 <br>
Feel free to connect with me on  [LinkedIn](https://www.linkedin.com/in/bhumikhokhani/)  |  [Twitter](https://twitter.com/bhumikhokhani) 
<br>
> 
If you like my work, you can extend your support by buying me a ☕. Thank you!

<a href="https://www.buymeacoffee.com/bhumikhokhani"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=bhumikhokhani&button_colour=FF5F5F&font_colour=ffffff&font_family=Cookie&outline_colour=000000&coffee_colour=FFDD00"></a>