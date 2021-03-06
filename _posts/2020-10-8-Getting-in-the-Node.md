---
layout: post
title: Getting in the Node — Node.js, Express, and Template Engines
---
#### What they are, when they are used, and who uses them


You've been busy out DOMinating the front-end of JavaScript. But you might be surprised on how well you can be served by adding a little back-end to your repertoire. This quick little guide will help you get in the node, express yourself, pretty up your ugly data fast. All with no fewer than 2.3 terrible puns per section.

## Serving you Right: What Node.js is, when you use it

Image your website is a stage play. 

![empty stage](/images/stage.jpg)
###### *Photo by [Barry Weatherall](https://unsplash.com/@dgmke_06?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText){:target="_blank"} on [Unsplash](https://unsplash.com/s/photos/stage-play?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText){:target="_blank"}. He obviously goes to fancier playhouses than me.*

Every play on the stage has at least two sides: the side facing the audience, where actors, props, and lights unfold the play; and a backstage, where people in black lurk with checklists, light and audio boards, queues, and currently unused props. Backstage people are just as important, just as passionate as the those who enjoy basking in the limelight, but if they do their job right, you'll never know they were there besides a few vague forms whisking passed in the darkness of a scene change.

Vanilla JavaScript and its frameworks are the front stage. JS moves objects in the Document Object Model, or DOM, where the user can see: telling it where to go, how to look, when to appear and disappear, and what to do when a set number of events happen.  

[Node.js](https://nodejs.org/){:target="_blank"}, on the other hand, is the backstage. While it's a platform built on JavaScript, and executes that code, it's purpose is to transmit requests, receive data in response, and make that data accessible so that the variables and function that are "actors on stage" can intake content to display. Node.js apps are servers: data-focused, logic-driven, and not intended for display.

![back stage](/images/backstage.jpg)

###### *Photo by [Adi Goldstein](https://unsplash.com/@adigold1?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText){:target="_blank"} on [Unsplash](https://unsplash.com/s/photos/backstage?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText){:target="_blank"}. Could be backstage for anything, anywhere, but one thing's for sure: they have budget for nice cases.*

Node.js is about input and output. Its modules can be made as servers, used to develop APIs, and/or act as a conduit to deliver static site information. They work great for data streaming apps, where you have a constant flow of information, things like chatbots for customer support, and single-page applications that can take and give a lot of information asynchronously.

Apps for video streaming (Netflix), social networks (LinkedIn), payment transactions (eBay and PayPal), and browser games have all been built with Node.js.


## Express.js: Node, but... faster

[Express](https://expressjs.com/){:target="_blank"} is a web framework for Node.js. It supports the development of web applications, and is particularly great for easing the creation and use of APIs. It simplifies some of the verbiage of Node.js to make the commands of getting and sending data to APIs more simple. And more simple/less verbose means less typing, and less time.

Using HTTP request methods like GET, POST, PUT, DELETE, and PATCH, and routing those requests to easily-accessed endpoints in an API, are a couple of the most common uses of Express.

## Templating Engines and Why Lazy is Good

Yet another constructive use for Node.js is it allows you to take advantage of Templating Engines. They provide a simplified way to take the data your Node is feeding, and display it flexibly on a static site. Rending this display happens as the template engine runs instead of pre-rendering a site completely for a server to request, so it displays the updated data every time its refreshed. Basically, you shove in data and the templates in, and static web pages in HTML pop out. 

TEs are relatively simple to employ, and provide consistent front-end templates into which you can feed your data for display. They aren't ideal for user interaction, but they often used simplified syntax that, once again, cuts down on typing time. Yay for less typing and more making things that make money!

For my own experiment, I chose [pug](https://www.npmjs.com/package/pug){:target="_blank"}. While its mascot animal is uglier than sin (a massive downgrade from its earler name 'Jade'), its clean, almost Pythonic syntax won me over almost immediately. It doesn't hurt that Pug is Express.js's preferred template engine out of the box, and installation was mostly a breeze. 

![pug dog](/images/pug.jpg)
###### *Photo by [Toshi](https://unsplash.com/@toshilepug?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText){:target="_blank"} on [Unsplash](https://unsplash.com/s/photos/pug?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText){:target="_blank"}. Some people find this variety of dog cute. Those people like tiny little bug-eyed, lip-faced rolls of fat with paws. I'll admit the ears aren't bad.*

In actual use, Pug does an admiral job of communicating in the similar ways of HTML, but cut down in a way that you crunch out a template in minutes. Add in a few mixins, and feel your way through some of the CSS idiosyncrasies of how it handles styling, and you are good to go. Data displayed.

Until next time...