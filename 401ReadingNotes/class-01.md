# Class 01 Read.

### Pain vs Suffering

Pain and Suffering are very different from each other, Pain is the result of working hard to achieve something in life while Suffering is the same feeling of pain, but without any purpose, ambition and aspiration.

-Also, to keep in mind these questions whenever you feel down or unsure about what you are doing:

* What’s your perspective?

* Why are you doing this?

* Do you want what comes at the end of this journey?

* Are you doing this for you?


### Big O notation

What is Big O notation ?

It is a Term used in Computer Science to describe the performance or complexity of an algorithm, mainly the worst case scenario and can be used to describe the execution time required or the space used.

Examples of Big O notation and their description:

* ### O(1)

-O(1) describes an algorithm that will always execute in the same time (or space) regardless of the size of the input data set.

Example Code:
```
bool IsFirstElementNull(IList<String> elements)
{
    return elements[0] == null;
}
```

* ### O(N)

-O(N) describes an algorithm whose performance will grow linearly and in direct proportion to the size of the input data set

Example Code:
```
bool ContainsValue(IEnumerable<string> elements, string value)
{
    foreach (var element in elements)
    {
        if (element == value) return true; 
    }     
    return false; 
}
```

* ### O(N²)

-O(N²) represents an algorithm whose performance is directly proportional to the square of the size of the input data set.

Example Code:
```
bool ContainsDuplicates(IList<string> elements)
{
    for (var outer = 0; outer < elements.Count; outer++) 
    {
        for (var inner = 0; inner < elements.Count; inner++) 
        { 
            // Don't compare with self 
            if (outer == inner) continue;             
            
            if (elements[outer] == elements[inner]) return true; 
        }
    }    
    return false;
}
```


* ### O(2^N)

-O(2^N) denotes an algorithm whose growth doubles with each addition to the input data set. 

```
int Fibonacci(int number)
{
    if (number <= 1) return number;
       
    return Fibonacci(number - 2) + Fibonacci(number - 1); 
}
```

# Facts About Python

* Python is simple(i.e x = 23, means x equals 23).
* Names are assigned differently.
* Assignments never copy data.
* Mutable Aliasing
* Immutable values can't alias.
* References can be more than just names.
* Function arguments are assignments.
* Names have no type.



# Bookmarks

### Great [Website](https://pymotw.com/3/index.html) for code examples of Python.

