# Classes-in-Python

# Classes

According to Google A class is a code template for creating objects.
Objects have member variables and have behaviour associated with them.
In python a class is created by the keyword class . An object is created using the constructor of the class.

# Basics (in easy words)

A class mainly contains methods, attributes, instances and a prefix 

* methods are simply like python fucntions
* one such method is _init_ method which is also considered as a constructor of a class
* attributes are declared inside a class (more in detail in file classes.py)
* instances are basically the names which we use to call a particular class.
* prefix basically works with _init_ method(define as self) 

# How to define a class: 
(just write class put a space and mention name you like to assign as a class, but make sure the first letter of your class is capitalised.

# format:


    class Introduction():                         (1)  

    def __init__(self,name,age):                  (2)
        self.name = name                          (3)
        self.age = age 
    def describe(self):                           (4)
        print('My name is ' + self.name +         (5)
        ' and i am ' + str(self.age)              (6)
        + ' years old')
        
    intro = Introduction('yash', 23)              (7)
    intro.describe()                              (8)     
     

At 1, i defined a class and named it as Introduction (keep first letter in capitals).

At 2, i defined a method by def and the method name is __init__(), having 3 parameters self, age, name

At 3, i mentioned attributes by using self.(anything you like to print) = the same parameter,
      in this case our attributes are name and age

At 4, i defined another method describe(), which will take care in what manner the output will be printed.

At 5, i gave the print command which basically gives us the output when describe method is called via instance.

At 6, i used str() function (use to define strings) with age.self, as python will only take strings not integers.

At 7, i mentioned an instance 'intro' which is use to call the class Introduction,
      also the values of parameters (name, age) are defined here (that is 'yash', 23)

At 8, i used the instance (intro) and method (describe) together in order to get the output that particulat method only

* Note: You can define as many as methods you like and to get all of them printed you need to mention the method name with the instance name. As shown above (8).






* Brief Explanation:

The __init__() method at is a special method that Python runs automatically whenever 
we create a new instance based on the Dog class.
This method has two leading underscores and two trail-ing underscores, 
a convention that helps prevent Python’s default method names from conflicting with your method names. 
Make sure to use two underscores on each side of __init__(). 
If you use just one on each side, the method won’t be called automatically when you use your class,
which can result in errors that are difficult to identify.
We define the __init__() method to have three parameters: self, name, and age. 
The self parameter is required in the method definition, and it must come first before the other parameters. 
It must be included in the def-inition because when Python calls this method later (to create an instance of Dog),
the method call will automatically pass the self argument. Every method call associated with an instance 
automatically passes self, which is a reference to the instance itself; it gives the individual instance access
to the attributes and methods in the class.

* more in Classes.py file :)

IDE Used: Jupyter Notebook
Book Reference: Python Crash Course (by Eric Matthes)

