//// THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS http://diveinto.html5doctor.com/storage.html ////
- Unlike web apps that are written primarily in Javascript, native apps are applications written in languages that the platform they are being built for accepts
    - native apps can create their own local storage and databases, etc to store info beyond k-v pairs
    - web apps deal with cookies, which have downsides:
        - they slow down the app by sending the same data multiple times
        - they send unencrypted data
        - limited to 4 KB 
    - needs for data storage incl:
        - a lot of storage space
        - on the client
        - that persists beyond a page refresh
        - and isn’t transmitted to the server
    - HTML5 took care of all this but before that attempted solutions had same issues: specific to a single browser or reliant on thid-party plugins
        - HTML5 was created to provide a standard API, native and consistent implementation, no reliance to 3rd-party plugins
    
    - HTML storage = local storage
    - “QUOTA_EXCEEDED_ERR” is the exception that will get thrown if you exceed your storage quota of 5 megabytes
    - SQL is a local storage competitor to HTML5