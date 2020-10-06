//// Article: The Problem of the Domain... ////

- majority of the problem is you cant see what you are trying to build very clearly 
- as programmers, many problem domains are difficult and look differently depending on POV
    - may not be given complete info
    - understanding the problem is critical
    - cut out cases and narrow focus, one part at a time

//// JS ////
- Objects group sets of variables and functions to create models
    - variables become properties
    - functions become methods/tasks
    - object can't have 2 keys with same names b/c keys are used to access their values
- DOM specifies how browsers should create a model of an HTML page & how JS can access and update the contents
    - DOM defines methods and properties to access/update each object in the model (which updates whats seen in the browser)
    - DOM is an API (Application Programming Interface) = let programs talk to eachother
    - as browser loads a page  it makes a model ('DOM tree')
        - consists of nodes (that represent the ele):
            1. document node = represents the entire page
            2. element nodes = identify then can go on to access attributes
            3. attribute nodes = part of their host ele; methods & props
            4. text nodes = text within host ele
        - to work with the tree: 
            a. locate the node that represents the ele you want to work with:
                - getEleByID() - uses ele's ID attribute
                - querySelector() - uses CSS selector (class ir ID) & returns first matching ele
            b. work with those eles
                - access/update text nodes
                - work with html content (textContent, innerHTML, createEles(), appendChild(), removeChild())
                - access/update attribute values (className/id)
    - DOM Queries = methods that find elements in DOM tree
        - can use a variable to store the results/location of eles = 'caching'
        - will return a NodeList if more than 1 result, then access the ele by index
            - getElementsByClassName('class'); getElementsByTagName('tagname'), querySelectorAll('css selector')
            - to choose item from NodeList use item(index) or array syntax
            - can loop thru nodelists:
                - find out how many items so can set a counter to loop
    - whitespace betw eles is treated as a text node
    - get/update ele content: 
        - text nodes w/ nodeValue prop, textContent
        - containing eles
        - use it's textContent, child elements & attributes