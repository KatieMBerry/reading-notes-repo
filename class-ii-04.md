/// URL Search Params ///
- URL Search Params() - returns an object
- methods:
    - append - a k/v pair as new search param
    - delete
    - entries - iterates through all k/v pairs
    - forEach() - iterates via a callback function
    - get()/getAll()- returns 1st val/all
    - has() - boolean for existence
    - keys()/values()
    - set() - to given value
    - sort() - by keys
    - toString() - returns a string containing a query string suitable for use in a URL

        /*searchParams.has("topic") === true; // true
        searchParams.get("topic") === "api"; // true
        searchParams.getAll("topic"); // ["api"]
        searchParams.get("foo") === null; // true
        searchParams.append("topic", "webdev");
        searchParams.toString(); // "q=URLUtils.searchParams&topic=api&topic=webdev"
        searchParams.set("topic", "More webdev");
        searchParams.toString(); // "q=URLUtils.searchParams&topic=More+webdev"
        searchParams.delete("topic");
        searchParams.toString(); // "q=URLUtils.searchParams"/*

/// toString() ///
- no parameters
- returns a DOMString

/// Location Object ///
- represents the location (URL) of the object it is linked to
- methods:
    - assign() = loads the resource at the URL provided in parameter
    - reload()
    - replace() = difference from assign() is that after using,the current page will not be saved in session History
    - toString() = returns a USVString containing the whole URL

/// HashChange Event ///
- happens when the part of url staring with # has changed
    - can use on EventListeners of onhashchange event handler