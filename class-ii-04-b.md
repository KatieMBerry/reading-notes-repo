/// JavaScript Asynchronous Programming and Callbacks ///
- Asynchronous means that things can happen independently of the main program flow
    - JavaScript is synchronous by default, and single threaded (one thing happens ata time)
    - browser provides a way for JS to look like it's working on things simultaneously by using a set of APIs 
    - function w/in a function that is called when an event is triggered = callback
        - error-first callbacks = the first parameter in any callback function is the error object
            - if no error, object = null
    - alternatives : Promises & Async/Await

/// Promises ///
= a proxy for a value that will eventually become available; object that represents an intermediate state of an operation
- once called, starts in pending state
    - function continues to execute while awaiting response
    - will return in resolved or rejected state
    - Async functions use the promises API as their building block
- new Promise((resolve, reject))
- can chain promises
- when rejects => nearest catch() down the chain
- promise callbacks are always called in the strict order they are placed in the event queue