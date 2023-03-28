---
title: "What is Typesense?"
seoTitle: "What is Typesense? | Bhumi Khokhani"
seoDescription: "Typesense, an open-source, typo-tolerant search engine designed for “search as you type” experience. As it significantly boosts developer's productivity."
datePublished: Fri Apr 01 2022 21:52:22 GMT+0000 (Coordinated Universal Time)
cuid: cl1gyuvwf04rwkbnvcs85a3l3
slug: what-is-typesense
canonical: https://aviyel.com/post/2909/what-is-typesense
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1648848721925/mBudRBjCX.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1648850188696/ro9FZ3w5E.png
tags: software-development, tools, opensource

---

# Introduction

There was a time when it was extremely difficult to discover appropriate search results and to receive instant search results. It might be difficult to discover information on the project at times, and bookmarking everything doesn't help.

You could choose to add a search engine at this point, which maybe is a software application that specializes in indexing large amounts of data and giving user-friendly ways to search through it. Typesense is one such software application that comes to rescue, may it be for privacy, lightning-fast performance or efficiency. So, let's get into learning more about Typesense for a better understanding.

## What is Typesense?

<center>
![1.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648849262449/z-aoy0elM.png)
</center>

Typesense is an open-source, typo-tolerant search engine designed for “search as you type” experiences that are fast (usually under 50 milliseconds) and developer productivity.

If you're familiar with Elasticsearch or Algolia, a general way to think about Typesense is as follows:

It is an open source alternative to Algolia that has some critical flaws ironed out, as well as an easier to use, battery powered alternative to Elasticsearch.

## Why Typesense?

<center>
![2.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1648849271955/bdfAH8kFM.png)
</center>

Typesense's goal is to reduce "time to market" by developing a fantastic instant search experience that offers relevant results straight away.

Finally, Typesense built each feature from the bottom up with the intention of making it intuitive and straightforward to use. It also provided reasonable defaults for all configuration settings, ensuring that the engine is ready to use right out of the box for the vast majority of use cases. "Batteries included" is the term for this.

Typesense's main goal is to significantly boost developer productivity while creating search experiences, offering you with one less thing to worry about.

**Open Source:**

Typesense is completely open source with its entire source code available online. Find it here.

**Customizable word separators:**

During schema building, use the token separators parameter to provide a list of special characters. In addition to space and new-line characters, these characters are used as word separators.
For example: - (hyphen) to this list to make a word like non-stick to be split on hyphen and indexed as two separate words. 
<center>
![3.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1649065987107/g4FP7dJ5u.gif)
</center>

**Index and search special characters:**

During schema building, use the symbols to index parameters to specify a list of special characters that will be indexed as text.
For example: To search for a specific character in the query syntax which has a special purpose, you must escape it by putting a backslash before it, for example: To find the string "who?" start by escaping the question mark by typing "who\?"

**Filtering based on rules:**

Overrides now have a filter by clause that may dynamically apply filters to query rules provided in the override.
For example: When it comes to narrowing down a stream of documents to only those that deal with specific issues and highlighting sections of the texts that were used to choose the documents. This method necessitates the creation of a set of rules for each topic by the user.
<center>
![4.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1649065935352/PASBhL-Q-.gif)
</center>

**Server side Caching: **

Cache search requests on the server for a configurable length of time to reduce perceived latency on large searches. Caching is turned off by default.
For example: Web files and data are temporarily stored on the origin server for reuse. When a user requests a web page for the first time on their first visit, the website goes through the typical procedure of requesting information from the server.
<center>
![5.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1649065883123/oyLOXq0o_.gif)
</center>

**Community Engagement:**

The process of addressing challenges impacting people's well-being by collaborating and communicating via groups of individuals linked through special interests.
Therefore, get access to various channels like GitHub issues, Email, Public Slack Community, Phone, Private Slack and Paid Prioritized Support Groups.


## Features

**Typo Tolerance:**

Automatically corrects typographical errors present in the search and provides seamless experience. Therefore, there is no need to worry about typos anymore, and you still will get a smooth browsing experience.
<center>
![6.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1648849313038/YL-zZBRrt.gif)
</center>

**Simple and delightful:**

Setup, integration, operation, running, and scalability are all simple. All of these tasks are straightforward to carry out. There are no complex steps to go through, instead direct command operations to carry out tasks.

**Blazing Fast:**

Built-in C++ serves as a “lightning fast” performance. From the bottom up, the system is meticulously designed for low-latency (50 ms) quick searches.

<center>
![7.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1648849403408/kHUgm7srf.gif)
</center>

**Tunable Ranking:**

The search results may very well be fine-tuned quickly and easily. A search parameter is sent to the search engine via a user interface, and the search parameter is used to complete the search. Therefore, flexible and quick query-time sorting allows you to fine-tune your findings.
<center>
![Blazing Fast Search For 2 Million Recipes with Typesense.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1648849336607/tvtkfRvxK.gif)
</center>

**Sorting:**

At query time, dynamically sort results depending on a certain field. Therefore, the sorting method allows us to easily sort, arrange and view data in desired format.

For example: Any fields in your document can be used to sort records on the go. Sort by price, popularity, and other factors.

<center>
![9.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1648849432809/_zpCt3XyP.gif)
</center>

**Synonyms:**

Define terms as counterparts such that searching for a word returns results for the synonyms defined. So that when you search for a word, you will also get results for the synonyms you have specified.

For example: Suppose you search for trousers,  the synonym for trousers, that is pants will also be displayed in the search results.

**Geo Search:**

This shows the search results corresponding to the distance from a particular latitude/longitude region point.

For example: When you search for a general item, suppose a stationary kit, the search results will show the nearby shops that sell the product instead of a shop that’s in another country.

<center>
![11.gif](https://cdn.hashnode.com/res/hashnode/image/upload/v1648849485271/dIp-LX6w5.gif)
</center>

<hr></hr>

*** To continue reading more about how Typesense benefits the users and how it is better to it's other competitors , read my complete article [here](https://aviyel.com/post/2909/what-is-typesense) .***

<hr></hr>

Feel free to connect with me on  [LinkedIn](https://www.linkedin.com/in/bhumikhokhani/)  |  [Twitter](https://twitter.com/bhumikhokhani) 
<br>
> 
If you like my work, you can extend your support by buying me a ☕. Thank you!

<a href="https://www.buymeacoffee.com/bhumikhokhani"><img src="https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=bhumikhokhani&button_colour=FF5F5F&font_colour=ffffff&font_family=Cookie&outline_colour=000000&coffee_colour=FFDD00"></a>