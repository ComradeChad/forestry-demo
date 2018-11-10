---
layout: home

---
This is a **bold** word

* option
* Option

`This is a code snippet`

***

### New Heading

    

***

# The Basic Components of a Regular Expression

A Regular expression (usually abbreviated as regex) is a distinct collection of characters that establish a search pattern. This guide will help you get started with regular expressions by going over the essential components that can be used to define them.

### The Basic Syntax

Regular expressions are of the format `/pattern/`, where 'pattern' describes an exact arrangement of characters that the regex will search for within a given text.

**Example** (JavaScript):

    var input = "Look for abc";
    var num =  input.search( /abc/ );
    console.log(num);
    // Output will be 10, since 10 is the location of abc in the string.

In the above example, `/abc/` is the regular expression, while `abc` is the pattern of characters to search for.

### Square Brackets

In a regular expression pattern, square brackets are used to define a scope of possible characters. The regex will search for any character between the two brackets. For example, the expression `/[_*]/` will match any occurrences of underscores or asterisks.

Additionally, you can use a hyphen between two characters within a bracket to include the entire range between them. For example, the expression `/[0-9]/` will search for any digit between 0 and 9. Similarly, `/[A-Z]/` will search for any capital letter, and `[a-f]` will search for any lowercase letter between a and f.

**Example:**

    var str = "x9F, 10100010b x85, 1011100b x5C";
    var reg = /x[0-9][0-9A-Z]/;
    
    str = str.replace(reg, ''); // Delete any regex matches
    console.log(str);
    // The output is ", 10100010b , 1011100b "