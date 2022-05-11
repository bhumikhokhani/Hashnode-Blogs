## Getting started with HTML

<head> <meta name="monetization" content="$ilp.uphold.com/fXgYL9dgXzHk"> </head>
### What basically is HTML?

> 
HTML was invented back in 1991 by Tim Berners-Lee and today it's having a standard version and is supported by all browsers.
For every web developer, it's really necessary to be proficient in HTML. **Hyper Text MarkUp Language** is basically used to create web-pages/websites. Here, we use HTML tags to structure the web pages.

### What is it used for?

> 
**HTML tags** are used to add certain attributes, format texts, embed images, create various links to different pages and within it's directories or even create lists. Also, it's really important to make sure to not break the structure or use any incorrect tags as it would lead to web browser failing in understand the information and in turn result in breaking of the webpage.

### Basic structure of HTML

```
 <!DOCTYPE html>
 <html> 
   <head>
      <title>...</title>
   </head>
   <body>...</body>
 </html>

``` 
*Before any explanation, it's necessary to know that every opening tag < > has a compulsory closing tag </ > except a few, which we will come through in the later part of the blog.*
1. The first line shows that the **document** is of the type **HTML**.
2. **< html >< /html >** Its written at the start and end, as it is the **root element**. This tag also acts as the **parent tag** and all others are it's **descendants**. 
3. **< head >** It contains the general information of the document, known as the metadata. The **metadata** contains all the information about the publication, authors etc.
4. **< title >** Its the **descendant** of **< head >**. It contains the title of the webpage which will be displayed on the title bar of the browser tab.
5. **< link >** and **< style >** This again comes under the **< head >** tag. **< link >** tag is used to **link** an **external stylesheet** to the HTML web page. Whereas **< style >** tag is where all the **styling attributes** are mentioned **internally** in the HTML document itself with a closing **< /style > **tag.
6. **< script >** tag is also a **descendant** of **< head >** tag. It contains either a **link** to an **external JS** file or has **internal JS** code with an closing **< /script > **tag.
7. **< body >** This tag contains all the **content** of the web page. It's basically a **container** with all information and tags required to be displayed on the webpage.

### Now we will discuss different tags that's used under <br> < body >

### 1) Tags used for maintaining document structure.
**- Comments**
```
<body>
  <!-- This is a comment - - >
  <h1> You're awesome! </h1>
</body>
```
**- Heading Tags**

```
<h1> You're awesome! </h1>
<h2> You're awesome! </h2>
<h3> You're awesome! </h3>
<h4> You're awesome! </h4>
<h5> You're awesome! </h5>
<h6> You're awesome! </h6>
```
Try adding this to your file and check for the results.
These are** six **different variations of writing a heading. If you had checked it, **< h1 > **has the **largest font-size** were as when you come to** < h6 >** it has the **smallest font-size**.

**- Horizontal Ruler**
```
<hr/> 
```
This is used to draw a horizontal line on the webpage. Indicating end of the section and moving the control to the next line. It doesn't have a closing tag.

**- Line Break**
```
<br/> 
```
This is basically used to move to the next line on the web page. It doesn't have a closing tag either.

**- Division tag**
```
<div>
This tag divides the web content into different blocks .
</div> 
```
**- Span class**
```
<span> 
This tag, without messing with the styling of the page,
adds an inline image, element or even a emoticon to the web page.
</span>
```
**- Paragraph tag**
```
<p> 
Nothing special. Paragraph text / plain text is placed here.
</p>
```
### 2) Tags used for the formatting of texts.

**- Strong tag**
```
<strong>
 Used to emphasise the text and make it bolder.
</strong>
```
**- Emphasis tag**
```
<em> 
 Used to emphasise the text and make it italic. 
</em>
```
**- Bold tag**
```
<b> 
 Used to create text in bold.
</b>
```
**- Italics tag**
```
<i> 
 Used to create text in italics.
</i>
```
**- Strike tag**
```
<strike> 
 Used to strike the text at the center, marking it as not important.
</strike>
```
**- Subscript tag**
```
<sub> 
 Used to writing a smaller fonter under the normal font.
</sub>
```
**- Superscript tag
**
```
<i> 
 Used to writing a smaller fonter above the normal font.
</i>
```
**- Code Snippet tag**
```
<code> 
 Used to write code snippets.
</code>
```
**- Abbreviation tag**
```
<abbr> 
 Used to denote abbreviation with it's respective full form.
</abbr>
```
### 3)Styling Tags

> 
The HTML style attribute is mainly used to add styles to a particular element in the web page. This is basically inline styling. The styling includes many things like background-color, text-color, font-size etc.

## Basic Syntax
```
<element style="property:value;">
```
*In the above, an **element **can be a heading, paragraph or even the entire body.<br>**Property** is the **CSS properties** like font-style, font-size, background-color etc.<br>**Value** is the **CSS values** like 50px, 50%, blue, red, center, left, right etc.*

**- Background-Color**
```
<body style="background-color:red;">
  Here the background-color of the entire body is red. 
  i.e. the entire web page.
</body>
```
```
<body>
  <h1 style="background-color:yellow;">
    Only the color of this heading will be have the color yellow in the background.
  </h1>
  <p style="background-color:blue;">
    Only the color of this paragraph will be have the color blue in the background.
  </p>
</body>
```
**- Text-Color**
```
<body>
  <h1 style="color:yellow;">
     The text-color of the heading will be yellow.
  </h1>
  <p style="color:blue;">
     The text-color of this paragraph will be red.
   </p>
</body>
```
**- Text-Size**
```
<body>
  <h1 style="font-size:100px;">
      The font-size of this heading will be 100px.
  </h1>
  <p style="font-size:50px">
      The font size of this paragraph will be 50px.
   </p>
</body>
```
**- Fonts**
```
<body style="font-family:Verdana;">
  The font-family of entire body will be Verdana.
</body>
```
```
<body>
  <h1 style="font-family:Comic Sans;">
    The font-family this heading will be displayed is in Comic Sans.
  </h1>
  <p style="font-family:Verdana;">
    The font-family this paragraph will be displayed is in Verdana.
   </p>
</body>
```
**- Alignment**
```
<body>
  <h1 style="text-align:center;">
      This heading has the center alignment.
  </h1>
  <p style="text-align:right;">
      This paragraph will have the right alignment.
  </p>
  <p style="text-align:left;">
      This paragraph will have the left alignment.
   </p>
</body>
```
**-Borders**
```
<body>
  <h1 style="border:4px solid Yellow;">
     This heading will have a thick 4px border of yellow color.
  </h1>
  <h2 style="border:3px solid Violet;">
     This heading will have a thick 3px border of violet color.
  </h2>
  <p style="border:2px solid Red;">
     This paragraph will have a thick 2px border of red color.
  </p>
</body>
```

### 4) Lists
**- Ordered Listing**
```
<ol>
  Used for ordered listing of items., i.e a numbered list. 
</ol>
```
**- Unordered Listing**
```
<ul>
  Used for unordered method of listing items., i.e using bullets. 
</ul>
```
**- Individual Listing**
```
<li> 
 Used to list individual items as a part of a given list. 
</li>
```
**- Defined Lists**
```
<dl> 
 Used to list items along with its definitions. 
</dl>
```
```
<dt> 
 Written inside <dl></dl>. Used to express a single term. 
</dt>
```
```
<dd> 
 Written inside <dl></dl>. Used to express the definition of a particular term. 
</dd>
```
***For a better understanding on Lists, here's an example:***
```
<ol>
 Ordered days of week:
  <li>Mon</li>
  <li>Tues</li>
  <li>Wed</li>
  <li>Thurs</li>
  <li>Fri</li>
  <li>Sat</li>
  <li>Sun</li>
</ol>
<ul>
 Unordered list of fruits:
  <li>Apple</li>
  <li>Chikko</li>
  <li>Mango</li>
</ul>
<dl>
  <dt>Apple</dt>
  <dd>Apple a day keeps the doctor away.</dd>
  <dt>Mango</dt>
  <dd>Always stays the king of fruits.</dd>
</dl>
```
### 5) Table Tags

**- Main Tag**
```
<table>
  Used to draw a table in HTML.
</table>
```
**- Caption Tag**
```
<caption>
  Used to write the table description.
</caption>
```
**- Thead Tag**
```
<thead>
  Contains description about specific columns in a particular table.
</thead>
```
**- Table Body**
```
<tbody> 
  This tag holds the data of the entire table.
</tbody>
```
**- Table Footer**
```
<tfoot>
 This Contains the footer of the table.
</tfoot>
```
**- Table Row**
```
<tr>
  This marks a single row in a table.
</tr>
```
**- Column Heading**
```
<th>
  This contains heading of a column in a table.
</th>
```
**- Table Data**
```
<td>
  This contains data written in a particular cell.  
</td>
```
**- Column Groups**
```
<colgroup>
  This tag is used to group different columns together.
</colgroup>
```
**- Column**
```
<col>
  This tag denotes a column inside a particular table.
```
***For a better understanding on Tables, here's an example:*** <br>
Basically, we are displaying a table with a caption describing the data stored under it. It has two columns: **Name** and **State**. We are entering three user-data, with details of **Bhumi** staying in **Mumbai**, **Roy** staying in **Karnataka** and **Jaanvi **staying in **Delhi**.
```
<table>
  <caption>User Location Data</caption>
  <tr>
    <th>Name</th>
    <th>State</th>
  </tr>
  <tr>
    <td>Bhumi</td>
    <td>Mumbai</td>
  </tr>
  <tr>
    <td>Roy</td>
    <td>Karnataka</td>
  </tr>
  <tr>
    <td>Jaanvi</td>
    <td>Delhi</td>
  </tr>
</table>
```
### 6) Link Tags

> 
Here, links are nothing but hyperlinks which on hovered upon turns into a small hand like cursor. On a click, it will take you to a specific part in the document or will take to another document.

**Basic Syntax**
```
<a href="destination_url"  target=" ">Linked Text</a>
```
In the above, **< a >** is known as the **anchor tag**. It's the compulsory element.<br>
**href** is the necessary attribute which takes to the mentioned **destination_url**.<br>
**target** attribute is used to specify how the target link has to open. It is optional. By default, it will open in same window. <br>
**" "** Here, the **target value** is mentioned.
**Linked Text** is the text which on clicked takes to the **destination_url**. 

## Different Target Values.

**- _blank**
```
<a href="url" target="_blank">
  This target value is used to open the linked document in a new window or tab.
</a>
```
**- _self**
```
<a href="url" target="_self">
  This target value is used to open the linked document in the same window or tab.
</a>
```
**- _parent**
```
<a href="url" target="_parent">
  This target value is used to open the linked document in the parent frame.
</a>
```
**- _top**
```
<a href="url" target="_top">
  This target value is used to open the linked document in the full body of the window.
</a>
```
### Usage of links
**- Images**
```
<a href="url">
  <img src="image1.png" alt="Sample1" style="width: 60px; height: 60px;">
</a>
```
There is a **image** displayed with the given **width** and **height**. <br>
When **hovered** over the image, the text **"Sample1"** is **displayed**. <br>
When **clicked** on the image, it takes to the mentioned **url** in < a > tag.

**- Email **
```
<a href="mailto:bhumikhokhani@gmail.com">Send Email</a>
```
There is a text **"Send Email"** displayed. When clicked, it **redirects** to the person's **mailing website or program**, where the **To:** field is filled by the mentioned **mailto address**.

### 7) Important HTML5 Tags.

**- Header Tag**
```
<header>
  Used to specify the header of the webpage. <br> Also, can be used used for the 
  objects in the particular webpage.
</header>
```
**- Main Tag**
```
<main>
  Used to mark the maincontent in the webpage.
</main>
```
**- Footer Tag**
```
<footer>
  Used to specify the footer of the webpage. <br> Also, can be used used for the 
  objects in the particular webpage.
</footer>
```
**- Article Tag**
```
<article>
  Used to describe an article in a webpage.
</article>
```
**- Aside Tag**
```
<aside>
  Used to display content in the sidebar of the particular webpage.
</aside>
```
**- Section Tag**
```
<section>
  Use to specify a particular session in the web page.
</section>
```
**- Details Tag**
```
<details> 
 Used to add addition information of the user which can be hidden or viewed. </details>
```
**- Summary Tag**
```
<summary> 
  Used as heading for the details tag. 
</summary>
```
**- Dialog Box**
```
<dialog>
  As the name says, used to create a dialog box.
</dialog>
```
**- Mark Tag**
```
<mark>
  As the name says, it's used to mark or highlight a portion of text.
</mark>
```
**- Nav Tag**
```
<nav>
  Used for the navigation links in a webpage.
</nav>
```
**- Menu Item**
```
<menuitem>
  Used to display particular item from a list or a menu.
</menuitem>
```
**-Meter Tag**
```
<meter>
  Used to measure scalar data within a given range.
</meter>
```
**- Progress Tag**
```
<progress>
  Used to track progress using a progress bar.
</progress>
```
**- Time Tag**
```
<time>
  Used for date and time.
</time>
```
**-Content Line-Break**
```
<wbr>
  Used to have a line-break within the particular content.
```

**- Figure Tag**

```
<figure>
  As the name says, it's used for diagrams, charts or any other figures.
</figure>
```

*Yet, HTML consists of many different tags for forms, tables, options etc., which I will cover in the next blog where I will explain simple HTML projects.*

<hr></hr>
## Wrapping Up

Hope this article gave you some basic knowledge on HTML and it's working.
Feel free to put up any questions if you have/had. I will try my best to answer them.

Also, you can leave you suggestions in the comment section and give a reaction if you enjoyed reading it 💖 <br>
Feel free to connect with me on  [LinkedIn](https://www.linkedin.com/in/bhumikhokhani/)  |  [Twitter](https://twitter.com/bhumikhokhani) 
<br>
> 
If you like my work, you can extend your support by buying me a ☕. Thank you!

<a href="https://www.buymeacoffee.com/bhumikhokhani"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=bhumikhokhani&button_colour=FF5F5F&font_colour=ffffff&font_family=Cookie&outline_colour=000000&coffee_colour=FFDD00"></a>