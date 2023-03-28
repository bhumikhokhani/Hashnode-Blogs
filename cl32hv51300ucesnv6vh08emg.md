---
title: "How to start an online store in 7 simple steps - Medusa."
seoTitle: "How to start an online store in 7 simple steps - Medusa"
seoDescription: "Talking about shopping in online stores. Let's learn about Shopify's open-source alternative Medusa. And how to easily set up an online store in 7 steps."
datePublished: Thu May 12 2022 04:12:11 GMT+0000 (Coordinated Universal Time)
cuid: cl32hv51300ucesnv6vh08emg
slug: how-to-start-an-online-store-in-7-simple-steps-medusa
canonical: https://aviyel.com/post/3071/how-to-start-an-online-store-in-7-simple-steps-medusa
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1652195656831/78rkBceg1.png
tags: tools, opensource, ecommerce, thw-web-apps, thw-web3

---

> *The link to the original post is [here](https://aviyel.com/post/3071/how-to-start-an-online-store-in-7-simple-steps-medusa). *

## Introduction

When someone suggests going shopping, the first thing that comes to mind are those shopping apps and platforms that are absolutely packed with the newest fashion and trends. The epidemic had a tremendous economic impact, forcing many purchasers to shop online, which has now become the new normal in the fashion and retail industries.

When talking about eCommerce platforms, the most famous one that comes to our mind is Shopify. Shopify has established itself as one of the most popular platforms for building an eCommerce store for any type of company. However, it does have a lot of drawbacks, including the fact that it is not free and has limited customizability. This is where Medusa enters the picture.

You'll learn how to set up an eCommerce store with Medusa in this blog. This covers everything you'll need to get your Medusa eCommerce store up and running, including setting up your development environment, adding features and plugins to your backend, frontend, and admin panel, and everything else.

## What is a Medusa?

![1.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1652161191761/Ldv4Efoat.png align="center")

Medusa is a fast open-source headless commerce engine. You could use Medusa as a whole or just the components you need for your eCommerce site because it is separated into three key components: the headless commerce section that displays the REST APIs for your online store, the frontend of your online store, and the admin panel.

## Why Medusa?

You'll need a storefront to present the things you're prepared to offer, communicate with consumers, take online payments, and more if you want to get into the online selling market. Medusa helps you sell your items on the internet by acting as a mediator.

Medusa is an open-source headless commerce platform that lets you set up your own store in minutes. Medusa's extensibility is one of the features that makes it a fantastic fit for your eCommerce site. Medusa now can also be used to develop multi-vendor markets.

## Simple steps to set up your online store using Medusa

Now we'll use Medusa, an open-source alternative to Shopify, to build an online eCommerce store.

**1.Installing Prerequisites:**

We'll need to install some software on our system, so let's examine what those are.

- Node.js
We will need Nodejs installed on our machine because our backend server is written in Node.js, we'll need it to deploy it. Our frontend will be created with Next.js, which requires npm, so we'll need it there as well! So, go to the Node.js website and download the latest version.

- PostgreSQL
Medusa actually uses Postgres to store data from your e-commerce website. To install Postgres on your PC, browse the Postgres website!

- Redis
Another popular database for caching is Redis. It's available for download at the Redis website.

- Medusa CLI
Finally, the Medusa CLI will be required. We can easily install using the npm command because we already have Node.js installed on our system.

```
npm i -g @medusajs/medusa-cli
```
**2.Building the Backend for the store**

We'll need a backend for your e-commerce business, so let's look at how to make one in this section!

The Medusa CLI makes setting up a new server easy. So, execute the following command:

```
medusa new my-medusa-server --seed
```

This will construct a simple server for us to start with, as well as a Postgres database, and the --seed parameter will seed the database with some test data.

**3.Starting the Server**

Change the directory to the app and begin the server by running this command:

```
cd my-medusa-server

medusa develop
```

On http://localhost:9000, a server will be started.

**4.Building the Frontend of the store**

For the front end, let's go with going to select Next.js; Medusa also supports Gatsby and Create React apps. Let's start from scratch using a starter template.  execute the following command:

```
npx create-next-app -e https://github.com/medusajs/nextjs-starter-medusa my-medusa-storefront
```

So a new Next.js project is created.

Now, let’s rename .env.template to .env.local. Using this command:

```
mv .env.template .env.local
```

**5.Running the application**

Using the below command, you can run the app on the localhost.

```
npm run dev
```

Now, if you check on your browser by running localhost:8000, you can see the simple frontend design of your app.

**6.Customizing Logo**

Customizing is just adding some logo or color theme of your choice. You can do this by simply opening up your code editor.

Let’s first change the logo of the app, for that, first open, 
> components/layout/nav-bar.jsx

```
<a>
  <Image
    src="YOUR_IMAGE_LOCATION"
    height="25px"
    width="25px"
    alt="logo"
  />
</a>
```

In the given code, edit the src and add the location of your logo. You can also change the height and width accordingly. Done! The logo is also set.

**7.Customizing Theme**

Let’s now see how to change the colours. Inside: root in globals.css, you'll find a wide range of colours; replace those with your existing brand colours. This will modify the site's general theme; if you want to change the CSS for a specific component, simply go to that component and customize it. You'll have a fully customized and working store after a few modifications and changes!

```
export const theme = {
  colors: {
    link: "#5469D3",
    primary: "#3b77ff",
    secondary: "#79B28A",
    medusaGreen: "#454B54",
    medusa: "#454B54",
    danger: "#FF7675",
    muted: "#E3E8EE",
    gray: "#a3acb9",
    lightest: "#fefefe",
    light: "#f0f0f0",
    dark: "#454545",
    darkest: "#212121",
    placeholder: "#a3acb9",
    blue: "#5469d4",
  }
}
```
And that’s all, we have our app ready, and running.

## Closing

Medusa makes building and managing your online store simple! I hope you didn't have trouble setting up your online store with Medusa. Let me know if you have any queries in the comments section.

And would you be interested in building your next online store with an open-source tool like Medusa? Do let me know in the comment section below. I hope you enjoyed reading it! <br>


<hr></hr>

Feel free to connect with me on  [LinkedIn](https://www.linkedin.com/in/bhumikhokhani/)  |  [Twitter](https://twitter.com/bhumikhokhani) 
<br>
> 
If you like my work, you can extend your support by buying me a ☕. Thank you!

<a href="https://www.buymeacoffee.com/bhumikhokhani"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=bhumikhokhani&button_colour=FF5F5F&font_colour=ffffff&font_family=Cookie&outline_colour=000000&coffee_colour=FFDD00"></a>
