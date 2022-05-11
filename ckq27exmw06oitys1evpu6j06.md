## Building Simple HTML Projects

<head> <meta name="monetization" content="$ilp.uphold.com/fXgYL9dgXzHk"> </head>
# Introduction

> 
The concepts are easy and understandable. I have explained the meaning of the different attributes and concepts in the comments. 
For better understanding, I would suggest you to go through the code and practice by executing it.

## A simple form made using HTML.

### Code

```
<html>
<head>
  <title>HTML Table</title>
  <style>
     body{
           background-color:#E6E6FA;
           font-family:cursive;
           padding-top:110px;
                }
      button{
             border:3px solid darkgray;
             font-size:15px;
             height:30px;
             width:10pc;
                }
   </style>
</head>
<body>
  <form method="" action="">
    <table border="4px" align="center" width="400">
      <h3><b><u>Registration form</u></b></h3>
      <tr>
        <th>Username</th>
         <!-- Input type "text" lets only a single line. -->
        <td><input type="text"></td>
      </tr>
      <tr>
        <th>First name</th>
        <td><input type="text"></td>
      </tr>
      <tr>
        <th>Last name</th>
        <td><input type="text" /></td>
      </tr>
      <tr>
        <th>Email</th>
         <!-- Input type "email" lets only email addresses to be entered.-->
        <td><input type="email" /></td>
      </tr>
      <tr>
        <th>Mobile</th>
         <!-- Input type "let" lets only phone numbers to be entered.-->
        <td><input type="tel" /></td>
      </tr>
      <tr>
        <th>Gender</th>
        <td>
         <!-- Input type "radio" lets you choose only one option from the option list.-->
          Male<input type="radio" name="g" value="m" />
          Female<input type="radio" name="g" value="f" />
        </td>
      </tr>
      <tr>
        <th>Hobbies</th>
        <td>
         <!-- Input type "checkbox" lets you choose as many options as you wish from the option list.-->
          Singing<input type="checkbox" value="h" />
          Dancing<input type="checkbox" value="h2" />
          Reading<input type="checkbox" value="h3" />
        </td>
      </tr>
    </table>
  </form>
  <br>
     <!-- Any url can be mentioned in " " -->
  <a href="">
    <button>Register</button>
  </a>
</body>
</center>

</html>
```

### Output

<iframe height="600" style="width: 100%;" scrolling="no" title="Table and forms" src="https://codepen.io/bhumikhokhani/embed/mdWVdqQ?height=265&theme-id=dark&default-tab=result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/bhumikhokhani/pen/mdWVdqQ'>Table and forms</a> by Bhumi Khokhani
  (<a href='https://codepen.io/bhumikhokhani'>@bhumikhokhani</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

<br\><hr></hr>

## A responsive website using HTML

### Code

```
<html>
<head>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    /* Tablet Screens */
    @media only screen and (max-width:800px) {
      .contents {
        width: 80%;
        padding: 0;
      }
      .right_bar {
        width: 100%;
      }
    }
    /*Mobile Screens */
    @media only screen and (max-width:500px) {
      .left_bar,
      .contents,
      .right_bar {
        width: 100%;
      }
    }
    * {
      box-sizing: border-box;
    }
    .left_bar {
      float: left;
      width: 20%;
    }
    .left_bar_items {
      padding: 10px;
      margin-top: 10px;
      border-bottom: 2px solid pink;
    }
    .contents {
      float: left;
      width: 60%;
      padding-left: 25px;
      padding-right: 15px;
    }
    .right_bar {
      background-color: pink;
      float: left;
      width: 20%;
      padding-top: 10px;
      padding-left: 15px;
      padding-right: 15px;
    }
  </style>
</head>
<body style="font-family:cursive;">
  <div style="background-color:lightblue; padding:50px;">
    <center>
      <h1 style="font-size:50px;">Welcome to my Page!</h1>
      <span style="font-size:20px;">Resize the browser window</span>
    </center>
  </div>
  <div>
    <div class="left_bar">
      <div class="left_bar_items">Home Page</div>
      <div class="left_bar_items">About Me</div>
      <div class="left_bar_items">My Blogs</div>
      <div class="left_bar_items">Projects</div>
      <div class="left_bar_items">Socials</div>
    </div>
  </div>
  <div class="contents">
    <h1>
      <u>My Blogs</u>
    </h1>
    <h2>Let's learn about responsive websites</h2>
    <p>Responsive web design is an approach to web design that makes web pages render well on a variety of devices and window or screen sizes from minimum to maximum display size.</p>
    <img src="https://www.maratopiadigitalmarketing.co.uk/wp-content/uploads/2019/08/responsive-design-blog-graphic.png" style="width:100%">
  </div>
  <div class="right_bar">
    <h2><u>How? </u></h2>
    <ol>
      <li>Add responsive meta tags in your HTML document</li>
      <li>Make sure to make the embedded images and videos responsive.</li>
      <li>Make sure the context is readable in different devices.</li>
    </ol>
    <h2><u>Advantage? </u></h2>
    <ul>
      <li>Creates a better user experience.</li>
      <li>Reaches to larger audience, and has smooth performance.</li>
    </ul>
  </div>
</body>

</html>
```

### Output

*(For better read, view at 0.5x is recommended)*

<iframe height="600" style="width: 100%;" scrolling="no" title="Responsive HTML Site" src="https://codepen.io/bhumikhokhani/embed/eYvXZNB?height=600&theme-id=dark&default-tab=result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/bhumikhokhani/pen/eYvXZNB'>Responsive HTML Site</a> by Bhumi Khokhani
  (<a href='https://codepen.io/bhumikhokhani'>@bhumikhokhani</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

<hr></hr>

# Wrapping Up

Hope this article gave you some practice and grip on working with HTML.
Feel free to put up any questions if you have/had. I will try my best to answer them.

Also, you can leave you suggestions in the comment section and give a reaction if you enjoyed reading it 💖 <br>
Feel free to connect with me on  [LinkedIn](https://www.linkedin.com/in/bhumikhokhani/)  |  [Twitter](https://twitter.com/bhumikhokhani) 
<br>
> 
If you like my work, you can extend your support by buying me a ☕. Thank you!

<a href="https://www.buymeacoffee.com/bhumikhokhani"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=bhumikhokhani&button_colour=FF5F5F&font_colour=ffffff&font_family=Cookie&outline_colour=000000&coffee_colour=FFDD00"></a>