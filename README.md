### Classes and Methods:

1. What is a class?
- A class is the place / site / blueprint from which objects are created. I like to think of this as a petri dish.

2. How do you create a class?
 you make a class by typing class, space, then name of your class with camel case at the top of your file. Make sure to add end to the end of your file. everything // all info about your place goes inside of these parameters.

3. What is an instance of a class?
- to follow the petri dish analogy, an instance of your class is like a molecule inside of the petri dish. it is an object which gets created inside of your class via an initialize method.

4. What is the difference between the CamelCase and snake_case styles of naming?
CamelCase is used for the naming of classes and modules, whereas snake case is used for naming methods, instance variables, recalling a file ( ex. require_relative 'snake_man').

5. How do you instantiate a class?

- you instantiate a class by first creating an instance variable inside of the class via initialize. Then, you create an instance of the class by picking a variable name and setting it equal to the class name, then a dot, then the word new.


6. How do you set the state of your new instance?
you set the state of your new instance via instance variables in an initialize method in which you can set default values to them, as well as make them setter or getter methods.

7. What should be done in the #initialize method?

- I personally like making an empty hash and then setting keys  values for each instance variable. args = {} and then calling args.fetch on each instance and setting it to a default key / value pair.

8. What is a class method?
- A class method is a method a method defined on the class. we use .self for this kind of method ( before the method name)

9. How is a class method different from an instance method?

- An instance method is not tied to any particular instance. 


10. How are methods you already know like #count or #sort etc instance methods?

- These are instance methods because they are used on specific arrays, which is a type of object already in ruby.


11. What's the difference between how you declare a class method vs an instance method?

The .self goes infront of the name of a Class method. You do not use .self on an instance method.


12. What's the difference between how you call a class method vs an instance method?
You call a class method on an instance of the class. You call an instance method on an instance of the class. 

13. What is an instance variable?
- an instance variable is an object that was create inside of a class. "An instance variable has a name beginning with @ , and its scope is confined to whatever object self refers to."

14. What's the difference between an instance variable and a 'regular' variable?
- an instance variable can be used throughout a class, where as a regular variable has a limited scope inside of a method. 

15. What are "getter" and "setter" methods used for?
- making your instance variables writable and readable. They also help to cut down on lines of code. They are a type of syntactic sugar.

16. What is the difference between a "getter" and a "setter" method?

- getter methods make instance variables readable. It allows you to refer to an instance variable throughout your class. 
-setter methods allow instance variables to be readable and writable. These allow for you to update the value of the variable from outside of the program. 

17. How do you make instance variables readable outside your class? Writeable? Both at the same time?

attr_ reader = readable
attr_writer = writable   -> not really sure why we'd use these? never did in Phase 0
attr_accessor = writeable and readable

18. What's the difference between a class and a module?
-a class has instance variables. A module is basically like a holding place for a method or methods. You can insert it via "include ModuleName" inside of your class, and use the methods inside of it in your class. Again, I see this as a shortcut, so you don't have to keep writing the same methods over and over again in multiple classes.

19. When would you use a class but not a module?
- I would use a class if I need to make instance variables and perhaps I only have one method and I don't really need to use this method anywhere else but in this one class. I'd use a module if I need to use a method in several different classes, and I don't want to keep copy / pasting it into all of these classes.

20. How does inheritance work?
Parent -> child. children / the youngest can require all information from the older generation. I've written down shortcuts for using super as well as rewriting it. The animal exercise was great!

21. What does #super do? Why use it?
Super allows you to inheritance instance variables from a parent class. It's really nice, because then you don't have to re-instantiate these instance variables in your child class ( class inheriting IV's from parent). You can over write super, or add to it by writing new instance variables underneath it in your child's initialize method. I like it! 


Resources:

https://launchschool.com/books/oo_ruby/read/classes_and_objects_part1
