//// Domain Modeling ////
- " A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model."
- Constructor Functions = defines the same properties between various objects
    - Storing data within properties ensures any newly created object can access that data later

- "Here's some tips to follow when building your own domain models:

    - When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
    - Model its attributes with a constructor function that defines and initializes properties.
    - Model its behaviors with small methods that focus on doing one job well.
    - Create instances using the new keyword followed by a call to a constructor function.
    - Store the newly created object in a variable so you can access its properties and methods from outside.
    - Use the this variable within methods so you can access the object's properties and methods from inside."

//// JS ////
- update an object property by declaring as if new (hotel.name = 'Park')
    - to delete or clear the value => delete.hotel.name or hotel.name = '';
    - Object constructors = template for creating objects with props and methods
        - uses this keyword instead of object name to indicate belongs to this function
        - new keyword followed by a call to the contructor function creates a new object & props of each object are given as arguments to the function