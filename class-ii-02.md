/// Components, Classes & Callbacks ///
- components = breaking down the UI into pieces; can also mean a specific technical approach
- atomic design methodology = breaking UI designs down into code, building blocks for site creation
    - benefits:
        - can see what can be reused or matched to create new components
        - can serve as a style guide
        - layout is easy to understand
        - consistent code, less duplicate code
        - quicker prototyping
        - easy to update/remove parts
        - more modular file structure
        - fewer components
- Pages
    -Templates
        - Organisms = large sections that we can easily extract from the page (can include other organisms)
            - molecules = sections that we can easily extract from an Organism; usually repeated in several places on the page
                - atoms = include basic HTML elements like form labels, inputs, buttons, and others that can’t be broken down any further 
- when code, start with atoms and work way upwards & make folders foe each
- for components to be reusable and composable, you have to make them as small and as independent as possible
- spearate UI into components where each component matches one piece of data model

/// Callbacks ///
= a function that is to be executed after another function has finished executing
    - real-world examples include needing to wait for an API response to your request before acting on that response
        - once response is given, callback function is invoked
        - synchronous = executed immediately (vs asynchronous)
- first-class functions = when functions are treated as variables

/// JS Classes ///

/* class User {
  constructor(name) { this.name = name; }
  sayHi() { alert(this.name); }
}

// proof: User is a function
alert(typeof User); // function /*

    - Creates a function named User, that becomes the result of the class declaration. The function code is taken from the constructor method
    - Stores class methods, such as sayHi, in User.prototype.