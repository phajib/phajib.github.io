---
layout: post
title:      "'Irasshaimase! One request response cycle!'"
date:       2019-09-21 09:22:00 +0000
permalink:  irasshaimase_one_request_response_cycle
---

# 1つの要求応答サイクルを取得できますか

You walk in to a restaurant. Sit down and open up the menu. The unagi bento box looks appetizing and you place your order. The waiter rings up your order as the chef and the staff go to work in creating your order of unagi bento box. When the apprentice chef places the final garnish, the bell is rung and waiter picks it up and presents it to you. Before you a perfect unagi bento box ready for it's instagram photoshoot, really?

If you are using something connected to the internet, you've most likely interacted with the Request Response Cycle and didn't even know it. You log in to check your email or jump on to view your social media or just wanted to check if the iPhone still looks the same from the previous model, no matter what it is the Request Response Cycle is operating in the background.

How it works:

1. You type in a URL (**U**niform **R**esource **L**ocator) in the browser.
2. A *request* is made by the browser.
3. The server receives the *request* and collects all the data to fulfill the request.
4. Often the data is loaded in to a  HTML (**H**yper **T**ext **M**arkup **L**anguage) page.
5. This HTML text is returned to to you the body of the HTTP (**H**yper **T**ext **T**ransfer **P**rotocol) *response*.
6. Once the *response* is received, the browser will then render the data in to a web page for the you to view.

So there are a couple of things that we need to know, client, the HTTP request, server response and client receiving the server response.

Anything that speaks HTTP are clients, our web browsers are perfect examples. The client makes the request/s via the HTTP request utilizing Uniform Resource Identifiers. Often it is a string that the server receives, a URL, eg. http://learn.co . The request contains some actions you want the server to carry out such as GET, POST, PATCH and DELETE.

GET - Retrieves a representation of a resource
POST - Submits data to be processed in the body of the request.
PATCH - Apply a partial modification of a resource.
DELETE - Deletes a specific resource.

The server will then run some code (code your wrote eg. your Sinatra Project) and send a response back. The server sends a status code of 200, a successful response. There are other status codes for example the 404 code, file not found. Our browser then renders the body of the response, often a web page.

![](http://curriculum-content.s3.amazonaws.com/how-the-web-works/Image_17_ComputerServer.png)


In regards to your project, the reques response cycle looks like this:

![](http://images.thoughtbot.com/ember-rails-terminology-differences/rails.png)



