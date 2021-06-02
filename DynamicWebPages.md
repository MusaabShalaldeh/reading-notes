# Dynamic Web Pages with Js

### Javascript

**Javascript** or **Js** is a well known programing language which is mainly used to create functionality for web pages, it gives you the ability to do many cool stuff, such as creating a dynamic web pages that react _realtime_ with the user.

Also, it is a powerful programming language that has many advantages like:

1. Simplicity.
2. Popularity(you are most likely to stumble upon a problem thats been already solved, just gotta search up for the solution).
3. Gives the ability to create rich interfaces.

### Dynamic Usage of Js with HTML:
```
<html>
<head>
  <title>Hello World</title>
</head>
<body>
 
First name: <input id="first_name">
Last name: <input id="last_name">
<button id="say">Say hi!</button>
 
<hr>
<div id="result"></div>
 
<script>
function say_hi() {
    var fname = document.getElementById('first_name').value;
    var lname = document.getElementById('last_name').value;
 
    var html = 'Hello <b>' + fname + '</b> ' + lname;
 
    document.getElementById('result').innerHTML = html;
}
 
document.getElementById('say').addEventListener('click', say_hi);
</script>
 
</body>
</html>
```
In the example above, the user inputs their first name and last name, then the user would click "Say Hi Button" and then it would add a new line to the web page at the bottom which says Hi back to the user with their own first name and last name. 




[Go Back](https://musaabshalaldeh.github.io/reading-notes/)