#  Intro To HTML and Programming with Javascript

### HTML.

**HTML** stands for **Hyper Text Markup Language** and it is the standard markup language for documents designed to be displayed in a web browser. There are many topics about html to talk about, but we are gonna start with few ones which are *Structure*, *Extra Markup*, *HTML5 Layout* and *Process & Design*.


#### Structure:

To start off, its recommended to understand how the structure of HTML web pages work at first, because the structure of the Web Page helps the readers to understand the messages you are trying to convey and help users navigate through your Web Page.

Web Pages are mainly constructed like **News Papers**, mainly including *Headers*, *Sections*, *Paragraphs*, *images* and the list goes on.

A code example of a simple strucutre would look like this:
```
<html>
<body>
<h1>This is the Main Heading</h1>
<p>This text might be an introduction to the rest of
the page. And if the page is a long one it might
be split up into several sub-headings.<p>
<h2>This is a Sub-Heading</h2>
<p>Many long articles have sub-headings so to help
you follow the structure of what is being written.
There may even be sub-sub-headings (or lower-level
headings).</p>
<h2>Another Sub-Heading</h2>
<p>Here you can see another sub-heading.</p>
</body>
</html>
```


#### The Evolution of HTML:

There have been multiple versions of HTML Since the first ever Web Page was created which are *HTML4*, *XHTML 1.0* and *HTML5*, but the latter is what is being used to this date due to the advantages and new features it offers.


#### HTML5 Layout:

*HTML5* introduces many elements that help define the structre of a Web Page, they allow you to divide up the parts of a page with clear indication what goes where.

Also, what mostly helps people memorize these elements, is that The names of these elements indicate the kind of content you will fill in them, for example:

1. *<header>*(the main header of a page or a section) 
2. *<footer>* (the main footer of a page, where usually copyrights are present at)
3. *<nav>* (links to other sites/ navigation to other pages of the same web app)
4. *<section>* (sections of a web page)

#### Process & Design:

The design of a web page is one of the most important elements about creating a Web Site, but lets talk about the process of designing a web page.

Alot of questions should be asked whenever you are deciding to create a web site, such as: 

1. **Who is this site for ?**

2. **How Often People Will Visit Your Site ?** 

3. **What Your Visitors are Trying to Achieve ?**

as they are going to help you decide what is the design and Wire Frame of the page should be, and how to deliver the message you are trying to send through the webpage properly.

### Programming with Javascript.

Programming is writing computer code to create a program or in other words, telling it what to do, in order to solve a problem or preform a specific task wethere its saving information or calculating an outcome. Programs consist of a series of instructions to tell a computer exactly what to do and how to do it.

There are three main concepts about programming that you need to to know which are

1. **_What is a script and how to write one_**

A script is a series of commands and instructions to tell the computer to do specific tasks and to write a script you need to follow the proper syntax, for example a script to print to the console *Hello*:

```
function SayHello()
{
  console.log("Hello!");
}
```

2. **_How computers fit in the world around them_**

To summorize how computers fit in the world around them, computers create models of the world using data and objects to represent physical things, which allows programmers to code when specific events happen and how to handle them,

3. **_How to write a script for a web page_**

To write a script for a web page, you need to know how to the HTML, CSS and Javascript fit together, HTML is for structring content, CSS is for making that content look beautiful and Javascript is for giving functionality to the Web Page.

Also, its best keep each language in its own file and link them with proper code to help keep code clean.

Code Example of a function that takes in the name of the user and says Hi back:

```
function SayHiToUser(userName)
{
  console.log("Hello "+username+"!")
}
```


[Go Back](https://musaabshalaldeh.github.io/reading-notes/)