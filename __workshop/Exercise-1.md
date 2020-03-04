# Questions

**With a partner**, answer these questions as completely as possible. Feel free to look at past lecture notes, the web, anything. 

Take the time to explain it to each other. 

The power of this exercise is in the act of _formulating_ and _explaining_ the concepts to someone else (your teammate).

## One

Run the app. Write out the steps, the _pseudo code_, required to create this app. It doesn't have to be totally accurate, or in the right order.

Only move on to the next question when you have enough detail that you would be able to start coding it yourself.

```
// Answer here
html
header
create an (form) input and submit
unordered list

Javascript
form submit pushes value to array (global variable)
page has forEach with array to make li with each value

CSS
pretty


```

## Two - `server.js`

Take a look at the `server.js` file.

We have a new module in there, `body-parser` that is required on line `4`. What is it for? What is its use-case? What other lines are related to this module?

_The NPM site might be a good place to start. Feel free to provide links as relevant._

```
// Answer here
Body-parser allows us to read client-side sent forms using req.body after method POST. In this caseit was used to push the value of input to an array
https://scotch.io/tutorials/use-expressjs-to-get-url-and-post-parameters

```

## Three - `server.js`

Look at lines `23` and `24`. Explain the methods used. How are they different? What are the usecases for each?

```
// Answer here
.get and .post are similar, in that they use url parameters to get to functions. Post is more powerful in that it can read data from the client(forms?) using req.body
```

## Four - `server.js`

Line `6`. That's new. What do you think it's for?

```
// Answer here
It is the function handlers which are imported from a different page. That page is accessed much like modules with a require(...)
those functions can now be called by their handlers
```

## Five - `handlers.js`

Explain line `1`. Where, why and how is `items` being used?

```
// Answer here
it is used as an array to push data in the ul. it gets its info by getting pushed by the data from post method
```

## Six - `handlers.js`

Why is there `redirect` on line `11`;

```
// Answer here
to provide an endpoint for the .get
Also, this refreshes the page so that items can go through the forEach with the latest entered info
``` 

## Seven - `handlers.js`

The `handle404` function is a more complex than we've seen thus far, what is the extra functionality for?

```
// Answer here
breaking down which type of error, if it is with the front end or during the data manipulation that goes on within body-parser (json)
```

## Eight - `ejs`

Take a look at `homepage.ejs` and `todoInput.ejs`. What is happening in there? Explain line-by-line...

```
// Answer here
homepage
1 - header
2- css container
3 - includes todo partial (explaines later, form)

5- css container
6- shoppinglist for css
7- for each to read the items array
8- read items data to populate the list
12- footer

todoinput
1- post method and action to trigger .post in server
2- label
3- input with placeholder. name='item' allows us to refer to it in the formdata function
4-submit button to trigger the action
```

## Nine - `styles.scss`

What are lines `2` to `7` for this file? Where are these values being used? Take a look at `_homepage.scss` as well? What do you notice?

```
// Answer here
they are scss global variables to be referenced for styling as keys: values
```

## Ten - `_homepage.scss`

Line `16`. See if by searching the Sass documentation, you can determine what _exactly_ is going on here. That `#{}` notation very specific to this use-case. Why?

```
// Answer here
sass interpolation. equivalent to backticks in js.
```







