# Object-Oriented Programming, HTML Tables


### Object-Oriented Programming (Domain Modelling)

Domain Modelling is the process of creating models in code for a specific problem which describes the behaviors and attributes in a method, which helps us have a better understanding of the problem that we want to solve, this prcoess is commonly used when we want to have single entity that'll have many instances, and that allows us to build self-contained objects with the same attributes and behaviors at ease.


Lets have an example code in which we demonstrate a case where its best to use Domain Modelling so that we save time and effort istead of writing different info for each new video manually:

```
var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail);
console.log(corgiFail);
```
and its going to log:
```
EpicFailVideo {epicRating: 7, hasAnimals: false}
epicRating: 7
hasAnimals: false
__proto__: Object
VM138:10 
EpicFailVideo {epicRating: 4, hasAnimals: true}
epicRating: 4
hasAnimals: true
__proto__: Object
```
Also, we can have inside those constructer functions all types of data, update them at run time, even methods which we can call for each different instance that was made using a model.


### HTML Tables


There are many cases where you want to have data on your website as **Grid** to show the user an easily understandable and organized table of information, and in those cases where HTML Tables come in use, they allow us to do exactly that.

There are 2 types of Tables which are Basic Tables and Long Tables, each have their own use.

To add an HTML Table to your webpage, you simply have to write the following code:

```
<table>
    <tr>
        <td>15</td>
        <td>15</td>
        <td>30</td>
    </tr>
    <tr>
        <td>45</td>
        <td>60</td>
        <td>45</td>
    </tr>
    <tr>
        <td>60</td>
        <td>90</td>
        <td>90</td>
    </tr>
</table>
```

This is a very basic table structure, which contains Table Tag, Table Row Tag and Table Data Tag, but you can even more customize how this table looks by adding Table Heading Tag, adding **colspan** attribute in table data to break the table into 2 sections and more...

__Full documentation can be found in the Duckett Book about HTML__


[Go Back](https://musaabshalaldeh.github.io/reading-notes/)