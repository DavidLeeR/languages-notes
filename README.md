# languages-notes

## Popular Programming Paradigms
- object oriented programming (oop)
- functional programming
- procedural programming

### Object Oriented Programming
- uses classes and objects
- make re-usable components
- object refers to an instance or a real entity that follows a blueprint (class)
- objects have attributes and methods
- principles
  - polymorphism
    - objects can have same name but serve different purpose based on use context
    - function overloading (functions can have same name as long as they have different signatures) and overriding (inheritance)
  - inheritance
    - child classes, abstract classes
  - encapsulation
    - wrapping up contents of entity into one unit
    - objects can have private state not accessable by other objects
  - abstraction
    - classes can expose certain data attributes while keeping others private
    - done to make things less complex or more secure
- advantages
  - reusability
  - security
  - maintenance
    - easy to make changes to one obect without affecting other objects
  - inheritance
    - easy to import required functionality from libraries and customize them, thanks to inheritance
- disadvantages
  - programs usually larger
  - beforehand planning of entities that should be modeled as classes
  - steep learning curve
- examples
  - Python, C++, Java, Perl, JS

### Procedural Programming
- work with procedures, also known as routines, subroutines, or functions
- procedure is essentially a sequence of instructions or computational steps to be executed
- follows a linear, top-down approach where each program is designed as some combination of a series of code instructions
- all about the idea of getting things done in a sequence of steps
- code isn’t organized in any logical groups or object-like entities
- just think about the different operations that need to happen in succession and code them down.
- Unlike OOP, where data and methods were tied together (encapsulated) in a class or object, procedural programming uses data and methods as two different entities
- advantages
  - Offers a simple, intuitive, and straightforward way of writing sequential code – could be a godsend for people just starting out with programming
  - easier for compilers and interpreters
  - Easy to track program flow
- disadvantages
  - Procedural programming code is not reusable. You’ll have to replicate the code implementation across different programs or files.
  - Not easy to scale up or extend for larger applications.
  - Not secure, because of visibility of data across the whole program.
- examples
  - C

### Functional Programming
- all about organizing your code around the idea of using functions
- Each function should be set up to perform a clearly defined task and ideally be a pure one
- break down the functionality of your code into neat, single-responsibility, reusable functions, and then pass them the necessary data parameters that they need to work with, let them process data (locally, without affecting the global state), and return the required values, which can then be used in the program
- principles
  - pure functions
    - A pure function is one that returns the same output for a given set of inputs, without having any side effects
    - have Referential transparency
      - the invocation of a function (a function call) could be replaced by the value it returns, without affecting anything in your code
    - pure functions only use the parameters they are passed
  - should ideally only use immutable data
    - This means that every time you want to do an operation on a variable, you store the updated value in a new variable instead of modifying the initial one
  - avoid Shared State
  - First-class and Higher-Order Functions
    - A first-class function is one that can be used just like any other variable – it can be passed to another function as an argument, returned as a value from another function, stored in data structures, and even be assigned as a value to a variable
    - Similarly, a higher-order function is one that can take as an argument or return as a value another function
    - This is how functional programming languages allow you to create and work with functions flexibly.
  - Recursion
    - aimed at as an alternative for iteration through while and for loops
- advantages
  - reliable
    - Pure functions will always return the same output for a given set of inputs, and will not have any side effects on the rest of the program.
  - Easier debugging
    - Thanks to immutability, developers need not track the whole history of a variable’s state across the program, and can instead target variables at specific points in the code where they might be creating problems
  - Lazy evaluation
    - Functional programming allows for lazy evaluation, i.e. values of variables are calculated only when it is required.
- disadvantages
  - using recursion for every iteration operation is unintuitive, as compared to using while and for loops
  - Reduced performance because of immutability – especially when having to duplicate large data structures even for making small changes.
  - Difficult or inefficient to perform recursion without letting variables be updated (immutability)
- examples
  - haskell, scala
