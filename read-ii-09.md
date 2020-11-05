/// DB Normalization ///
- hone in on one topic/purpose
- les prone to dups and anomalies and simplifies queries
- 3 progressive forms:
    - 1NF (normal form)
        = no repeating groups of columns 
    - 2NF
        = + all columns depend on primary key
    - 3NF
        = + all columns not transitively dependent on primary key

/// Visual Representation ///
Returning Data from 2 relational tables:

1. INNER JOIN: returns left (a) table records match right (b) table 
    SELECT <select_list> 
    FROM Table_A A
    INNER JOIN Table_B B
    ON A.Key = B.Key

2 LEFT: returns all left table plus matches to right table
    SELECT <select_list>
    FROM Table_A A
    LEFT JOIN Table_B B
    ON A.Key = B.Key

3. RIGHT: returns all right table plus matches to left table
    SELECT <select_list>
    FROM Table_A A
    RIGHT JOIN Table_B B
    ON A.Key = B.Key
    Outer JOIN

4. OUTER: returns all records from both, joining matching
    SELECT <select_list>
    FROM Table_A A
    FULL OUTER JOIN Table_B B
    ON A.Key = B.Key

5. LEFT Excluding: left table records that do not match right table
    SELECT <select_list> 
    FROM Table_A A
    LEFT JOIN Table_B B
    ON A.Key = B.Key
    WHERE B.Key IS NULL

6. RIGHT Excluding: right table records that do not match left table
    SELECT <select_list>
    FROM Table_A A
    RIGHT JOIN Table_B B
    ON A.Key = B.Key
    WHERE A.Key IS NULL

7. OUTER Excluding: all from each that do not match
    SELECT <select_list>
    FROM Table_A A
    FULL OUTER JOIN Table_B B
    ON A.Key = B.Key
    WHERE A.Key IS NULL OR B.Key IS NULL

