# Local Storage


Storing Data is one of the main components in having interactive Web Applications, Games and more. though tot directly making them interactable, but in indirect way, for example saving important values such as passwords and emails to compare them later whenever the user wants to log back in, or saving data such as user preferences for a web site.


Although in HTMl5 we have Web Storage, or as many would like to call it DOM Storage or Local Storage due to uninteresting political reasons, and Local Storage is a way for web pages to store named key or value pairs locally within the client web browser and this data persists even after you navigate away from the web site like cookies.

It is very easy to store data using Local storage, we mainly use **localStorage.setItem("name", name);** to create a value that we store locally and to get the value that we made we just have to get it by **localStorage.getItem("name");** which will return the value we saved eariler and from there we can use it in whatever way we like.


Here is an very simple example in which a function is called whenever a user opens the webpage/website and it would greet them if they are new with "Hi Stranger" and ask the user to enter their name, and if the function is called again it is going to say "Hi Username"(keep in mind its generally a good practice to check if the value we want exists in the first place, if not we just create it right after):

```
function greet(){
    name = localStorage.getItem("name");
    if (name == null || name == "null"){
      alert("Hi, Stranger!");
      name = prompt("What is your name?");
      localStorage.setItem("name", name);
    } else {
      alert ("Hi, " + name + "!");
    } 
}
```




[Go Back](https://musaabshalaldeh.github.io/reading-notes/)