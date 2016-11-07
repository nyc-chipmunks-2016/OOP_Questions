### Classes and Methods:

1. What is a class?
 * A class is a first-class object that holds state. Classes can be passed as objects.
2. How do you create a class?
 * class ClassName ... {methods} ... end
3. What is an instance of a class?
 * An instance is the object that is created when the class is instantiated.
4. What is the difference between the CamelCase and snake_case styles of naming?
  * Classes and Modules use CamelCase, the word has no spaces but each of the first word is capitalized
  * Methods use snake_case, all words are lowercase and spaces are represented by underscores
5. How do you instantiate a class?
  * ClassName.new(args)
6. How do you set the state of your new instance?
  * Creating a initialize method with all the needed states
7. What should be done in the #initialize method?
  * Set the state of the object when a new instance is created
8. What is a class method?
  * They are the methods inside of the class
9. How is a class method different from an instance method?
  * Class methods does not deal with individual instance of a class.
  * Instance methods only work during an instance. You have to create a new instance to use them again.
10. How are methods you already know like #count or #sort etc instance methods?
  * They can be used anytime without instantiating a class
11. What's the difference between how you declare a class method vs an instance method?
  * Class method you would have to state the class instance then the method, ClassName.new.method
  * You could also set the new instance as a variable and call the method, variable.method
  * Instance method is used after a hash/string/array, array.instance_variable
12. What's the difference between how you call a class method vs an instance method?
  * For class method you have to instantiate then call the method, instance methods you just call the method
13. What is an instance variable?
  * Variables that can be used during an instance, and can be used anywhere inside the class
14. What's the difference between an instance variable and a 'regular' variable?
  * Regular variables can only be used within a method where the variable is located
  * Instance variable could be used anywhere in the class they are stored
15. What are "getter" and "setter" methods used for?
  * getters methods are used to read variables but cannot be written over
  * setters methods are used to rewrite variables
16. What is the difference between a "getter" and a "setter" method?
  * getters are reader only method
  * setters are writeable method
17. How do you make instance variables readable outside your class? Writeable? Both at the same time?
  * Readable outside - Use attr_reader; Writeable - attr_writer; Both - attr_accessor
18. What's the difference between a class and a module?
  * Class has state, modules are behaviors. You cannot initialize in a module.
19. When would you use a class but not a module?
  * You would use a class when you need it to save state or initialize a method.
20. How does inheritance work?
  * It takes methods/states from parent classes. These methods/states could be used in the children class.
21. What does #super do? Why use it?
  * It brings down all states depending where super is called from in the children class.
