//// HTML & CSS ////
- CSS Positioning:
    - normal flow (default) - each block level ele on a new line, vertically going down the page (position: static)
    - relative positioning - shifts block eles relative to others
    - absolute positioning - in relation to container ele (moves as you scroll up/down) & doesn't affect position of surrounding eles
    - fixed positioing - in relation to browser window
    - floating eles - out of normal flow and moves to far left/right of container ele; uses width prop
        - can be used to set eles side by side
        - clear class - no ele in containing ele should touch on left/right/both sides
        - floats can create multi-column layouts
    - z-index prop - controls which ele is ontop (higher the number, closer to top)
    - liquid layouts - use %; 90% width rule for body
    - fixed layouts - use px; 960px width rule for body w/ auto l/r margins
    - 960px grid system - composition/stylesheet 

    //// JS ////
    - execution contexts - 1 global and each function creates one
    - when statement needs data from another function, it stacks the newer function ontop of current task
        1. prepare - variables and functions hoisted to top
        2. execute - each execution context has its own variables object
    - scope p457
    - console methods: 
        - info
        - warn
        - error
        - group
        - table
        - assert (conditional)
    - breakpoints can check values stored as variables at a given moment in time
    - try, catch, finally p 458