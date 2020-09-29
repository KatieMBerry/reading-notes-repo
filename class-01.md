# reading-notes-repo: Class-01

////HTML & CSS - Structure & Markup ///////
- html comments use <!-- -->
- no two elements can have same id attribute value
- block elements always start on a new line (h1, p, ul, li)
- div: groups eles together in one block-level box
    - can wrap page
    - groups related content
    - can be helpful to add a comment at the end of the block to clearly mark it
- span : inline equivalent to div
- iframe element: window into another page (like Google Maps) - from anywhere on web
    -needs src, height, width
    -seamless attribute for non-scrolling
- meta element: within head & contains info about webpage for search engines 
    - empty ele, so no closing tag
    - uses name attributes (intention) and content attributes (specifications)
        - name attributes commonly used:
            1) description - for search engines
            1) keywords - for user searches
            1) robots - indicates if search engines should use in search results
                - noindex vs nofollow
    - http-equiv / content: 
        1) author / author
        1) pragma - prevents browser from caching / no-cache
        1) expires - should no longer be cached / Day, Date Month Time TZ
- escape characters page 194 - codes for symbols or characters reserved for html code
----Summary & Example page 196 -----   


////HTML & CSS - html5 Layout ///////
- article ele: containers content that could stand alone
- aside ele: 
    - if w/in article: should contain info related to but not essential to meaning of article (sidebar)
    - if outside an article: acts as a container for content related to whole page
- sections: groups related content, each with own heading 
    -don't use to wrap entire page unless only one piece of content
- hgroup: groups h1-h6 eles so treated as one single heading
- figure: images, videos, diagrams, graphs, code samples
    - figcaption: description
- anchor: can be used to link around block-level eles that contain child eles
- helping older browsers understand - page 442


////HTML & CSS - Process & Design ///////
- target audience: individuals vs companies
    - user personas
- user motivation & goals: reasons users visit
- what do your users need
- how often are users visiting
- site maps & user goals
- wireframes of key info - hierarchy and spacing
- design: 
        -content 
        - prioritizing (visual hierarchy/contrast) 
            - size
            - color
            - style
            -images
        - organizing (grouping)
            - proximity
            -closure
            - continuance
            - white space
            - color
            - borders
            - consistency
            - headings
- navigation: 
    - concise
    - clear - predictable
    - selective - only sections/content
    - context - where am I?
    - interactive - hover state, clicked-link color change
    - consistent


//// JavaScript - ABC's of Programming //////
- script = instructions for the computer to achieve a goal, step-by-step (like a recipe)
    - browser may use different parts depending on user interaction
    - scripts can run diff sections of code in response to sitution
- writing scripts: PB&J example
    1) define the goal 
    1) design series of tasks and sequence of steps to complete 
    - flowcharts: to show the path(s) between each step
- Objects: 
    - properties - name/value pairs
    - events - interactions that trigger functionality/methods
    - methods - what can be done with the object or it's properties (retrieve or update)
- DOM: Doc Object Model represents an html page pg 41
    - can access and change what content users see and respond to how they interact with it
    - nodes = objects within the DOM