---
title: "Learning about the 3 CSS Properties"
seoTitle: "Learning Perspective 3D"
seoDescription: "Under this we learn about the CSS properties perspective, transform and transition."
datePublished: Mon May 02 2022 10:24:17 GMT+0000 (Coordinated Universal Time)
cuid: ckqhsjlc90f8p7ks1bsdnf3g8
slug: learning-about-the-3-css-properties
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1624890885316/GlkYc-BYk.png
tags: web-development, hashnode, 2articles1week, thw-web-apps, thw-mobile-apps

---

<head><meta name="monetization" content="$ilp.uphold.com/fXgYL9dgXzHk"></head>
<!-- Google Tag Manager -->
<script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
})(window,document,'script','dataLayer','GTM-ND3TDD2');</script>
<!-- End Google Tag Manager -->
<!-- Google Tag Manager (noscript) -->
<noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-ND3TDD2"
height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript>
<!-- End Google Tag Manager (noscript) -->

# Introduction
The other day, when I put up my blog on  [Building simple CSS projects](https://bhumikhokhani.hashnode.dev/building-simple-css-projects) , there was a request by @[Favourite Jome](@Favourite) to explain perspective property. So, this article focuses on the css property, perspective. I will be starting with the basics of perspective property and then go in-depth on learning more about it with the help of examples.

## What is perspective?
As the name says, this property says from which position will the user looks at the given 3D object. This won't affect how the element is rendered and is only applied to the child elements only.

## Use of perspective?
As the definition said, this property gives the 3D object a position to be viewed from. This will also define from how far the user will be looking at the object. This means **lower the perspective value, more subtle the 3D effect**.

## Do the child elements require any different property?
Yes, the child property uses the transform property.
So, basically perspective property is the main property. It's function is to create some 3D space for the child elements. The child elements use the transform property to give depth to the child elements.

## Syntax
```
.parent{
   perspective: space_size;
}
.child{
   transform: rotate_axis(value deg);
}
```

## Example

```
.scene {
  perspective: 500px;
}

.elements {
  transform: rotateY(60deg); 
  //Also can be written specifying two values, as given below.
  transform: rotateX(60deg) rotateY(60deg);
}
```

## What is perspective-origin?
It basically is the view from where the user is looking at the 3D object.

## Syntax
```
perspective-origin: x-axis y-axis| initial| inherit;
```
*Perspective origin values can possibly be: %, left, center, right, size.*

## Example
```
perspective-origin: 60%; //Percentage
perspective-origin: right; //Side view
perspective-origin: bottom right; //Corner view
perspective-origin: inherit; //Inherits from parent element
perspective-origin: initial; //Sets to default value which is 50%
```

## Perspective & Views

> 
I found one of the codepen which describes the perspective from different views.

<iframe height="700" style="width: 100%;" scrolling="no" title="Perspective cube" src="https://codepen.io/desandro/embed/bMqZmr?defaultTab=result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
</iframe>


## Flip-Flip 
> 
Now, I will explain the perspective, transform and transition part of the **Flip-Flip** project I had presented in my previous blog. Hope this helps in understanding the application of the same. (Explanation in the comments.)

```
.flip-card {
  width: 500px;
  height: 500px;
  perspective: 1000px; //Creating the 3D space for the Card
}
.flip-card-inner { //This is where the content is written at the back of Card.
  position: relative; //Setting the position of the Card
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 0.6s; //Total duration for the Card to flip
  transform-style: preserve-3d;
}
.flip-card:hover .flip-card-inner { //When hovered over any side of the Card,
  transform: rotateY(180deg); // Adding rotation along Y-axis.
}
.flip-card-front,
.flip-card-back { //This applies to both sides of the Card.
  position: absolute;
  width: 100%;
  height: 100%;
  -webkit-backface-visibility: hidden;
  backface-visibility: hidden; //The opposite face to the display is hidden.
}
.flip-card-back { //Adding styling attributes to the content side of the Card.
  background-color: #ffe8f5;
  transform: rotateY(180deg); 
  color: #323738;
  border: 2px solid black;
  outline: 3.5px dashed #de97c0;
}
```
## Output
<iframe height="700" style="width: 100%;" scrolling="no" title="Task 3- Flip Flip" src="https://codepen.io/bhumikhokhani/embed/OJpyvXq?defaultTab=result" frameborder="no" loading="lazy" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href="https://codepen.io/bhumikhokhani/pen/OJpyvXq">
  Task 3- Flip Flip</a> by Bhumi Khokhani (<a href="https://codepen.io/bhumikhokhani">@bhumikhokhani</a>)
  on <a href="https://codepen.io">CodePen</a>.
</iframe>

<hr></hr>

# Wrapping Up

Hope this article gave you some practice and grip on working with the CSS property perspective.
Feel free to put up any questions if you have/had. I will try my best to answer them.

Also, you can leave you suggestions in the comment section and give a reaction if you enjoyed reading it 💖 <br>
Feel free to connect with me on  [LinkedIn](https://www.linkedin.com/in/bhumikhokhani/)  |  [Twitter](https://twitter.com/bhumikhokhani) 
<br>
> 
If you like my work, you can extend your support by buying me a ☕. Thank you!

<a href="https://www.buymeacoffee.com/bhumikhokhani"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=bhumikhokhani&button_colour=FF5F5F&font_colour=ffffff&font_family=Cookie&outline_colour=000000&coffee_colour=FFDD00"></a>