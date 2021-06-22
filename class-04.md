# HTML Links, JS Functions, and Intro to CSS Layout

### HTML Links:

One of most important things to do when making a Website, is to have the ability to switch between its pages, just like when you are switching book pages, and links exactly allow us to do that, aswell as being able to link to other websites, email links and more.

To write a link in html, you simply need to put it between *Anchor Tag* with a name of the link.

Example:
```
<a href="https://www.google.jo/">Go To Google</a>  
```

Also you can add "target" attribute to the Anchor tag so that the link opens in a window.

### CSS Layout:

It is essential to understand how layout works in HTML and CSS as it helps us have an easier time designing and making our websites, pages etc..., and since browsers display pages in normal flow which is somewhat boring, we should manually work on specify relative, absolute, or fixed positions by using properties like **float** to move elements around.

One of the common practices that designers do, is keeping pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels as it helps with consistancy.

### Javascript Functions:

Having an interactive webpage/website or web application requires hundreds if not thousands of code, but is it really optimal to run code all at once ?, no, thats why there are tools that we can uitilize to help us make better and more organized code such as Functions, use of Objects and built-in Objects.


##### Functions

Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of st atements).   

_Definitation taken from Duckett book about Js and JQuery_


Example code:
```
let usersCount = 225;

function WelcomeNewUser()
{
    console.log("Hello new user!")
    usersCount += 1;
}
```

Which would basically welcome a new user and add this user to the users count, its called each time a new user joins!

[Go Back](https://musaabshalaldeh.github.io/reading-notes/)