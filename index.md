---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
# The Basic Components of a Regular Expression
A Regular expression (usually abbreviated as regex) is a distinct collection of characters that establish a search pattern. This guide will help you get started with regular expressions by going over the essential components that can be used to define them.

### The Basic Syntax
Regular expressions are of the format `/pattern/`, where 'pattern' describes an exact arrangement of characters that the regex will search for within a given text.

**Example** (JavaScript):
```
var input = "Look for abc";
var num =  input.search( /abc/ );
console.log(num);
// Output will be 10, since 10 is the location of abc in the string.
```
In the above example, `/abc/` is the regular expression, while `abc` is the pattern of characters to search for.
### Square Brackets
In a regular expression pattern, square brackets are used to define a scope of possible characters. The regex will search for any character between the two brackets. For example, the expression `/[_*]/` will match any occurrences of underscores or asterisks.

Additionally, you can use a hyphen between two characters within a bracket to include the entire range between them. For example, the expression `/[0-9]/` will search for any digit between 0 and 9. Similarly, `/[A-Z]/` will search for any capital letter, and `[a-f]` will search for any lowercase letter between a and f.

**Example:**
```
var str = "x9F, 10100010b x85, 1011100b x5C";
var reg = /x[0-9][0-9A-Z]/;

str = str.replace(reg, ''); // Delete any regex matches
console.log(str);
// The output is ", 10100010b , 1011100b "
```

### Shorthand Characters
Rather than typing out common ranges such as alphanumerics each time, regular expressions provide shorthands that you can use to denote them instead. The most common shorthand symbols are as follows;
* `\w` matches a letter, digit, or underscore.
* `\d` matches a single digit character.
* `\s` matches a whitespace character (including tabs and line breaks).

**Example:**
```
var str = "m:12 d:10 y:1997 John Smith";

var regW = /\w/;
str2 = str.replace(regW, '');
console.log(str2); // The output is ":12 :10 :1997  ";

var regD = /\d/;
str1 = str.replace(regD, ''); // Delete any regex matches
console.log(str1); // The output is "m: d: y: John Smith"

var regS = /\s/;
str3 = str.replace(regS, '');
console.log(str3); // The output is "m:12d:10y:1997JohnSmith";
```

[A list of other shorthand characters can be found here.](https://www.rexegg.com/regex-quickstart.html#chars)

### Conclusion
Regular expressions are a powerful tool for searching text or formatting input, and these are just a few primary components. If you want to bring the strength and customizability of your regular expressions to the next level, I recommend you [visit this website](https://www.rexegg.com/regex-disambiguation.html) to learn about additional regex elements.

---

#### Appendix

*Audience:* other COMP 3040 students

*Venue:* a website like Geeks for Geeks

*Purpose:* Instruct the audience on how to use the basic components of Regular Expressions.

*Additional Purpose:* Encourage the student to learn more about regular expressions, or try their own.

*Desired Reaction:* Understanding of the basic componments of regular expressions, confident that they can apply the regular expression elements outlined.

*Vocabulary:* General programming jargon, JavaScript syntax for code examples. Vocabulary that a college-level student should have no trouble understanding.

*Tone:* Brief, concise, to-the-point.

*Examples:* A code or regex example of syntax or expected regex matches for every topic introduced.
---

# The Basic Components of a Regular Expression
A Regular expression (usually abbreviated as regex) is a distinct collection of characters that establish a search pattern. This guide will help you get started with regular expressions by going over the essential components that can be used to define them.

### The Basic Syntax
Regular expressions are of the format `/pattern/`, where 'pattern' describes an exact arrangement of characters that the regex will search for within a given text.

**Example** (JavaScript):
```
var input = "Look for abc";
var num =  input.search( /abc/ );
console.log(num);
// Output will be 10, since 10 is the location of abc in the string.
```
In the above example, `/abc/` is the regular expression, while `abc` is the pattern of characters to search for.
### Square Brackets
In a regular expression pattern, square brackets are used to define a scope of possible characters. The regex will search for any character between the two brackets. For example, the expression `/[_*]/` will match any occurrences of underscores or asterisks.

Additionally, you can use a hyphen between two characters within a bracket to include the entire range between them. For example, the expression `/[0-9]/` will search for any digit between 0 and 9. Similarly, `/[A-Z]/` will search for any capital letter, and `[a-f]` will search for any lowercase letter between a and f.

**Example:**
```
var str = "x9F, 10100010b x85, 1011100b x5C";
var reg = /x[0-9][0-9A-Z]/;

str = str.replace(reg, ''); // Delete any regex matches
console.log(str);
// The output is ", 10100010b , 1011100b "
```

### Shorthand Characters
Rather than typing out common ranges such as alphanumerics each time, regular expressions provide shorthands that you can use to denote them instead. The most common shorthand symbols are as follows;
* `\w` matches a letter, digit, or underscore.
* `\d` matches a single digit character.
* `\s` matches a whitespace character (including tabs and line breaks).

**Example:**
```
var str = "m:12 d:10 y:1997 John Smith";

var regW = /\w/;
str2 = str.replace(regW, '');
console.log(str2); // The output is ":12 :10 :1997  ";

var regD = /\d/;
str1 = str.replace(regD, ''); // Delete any regex matches
console.log(str1); // The output is "m: d: y: John Smith"

var regS = /\s/;
str3 = str.replace(regS, '');
console.log(str3); // The output is "m:12d:10y:1997JohnSmith";
```

[A list of other shorthand characters can be found here.](https://www.rexegg.com/regex-quickstart.html#chars)

### Conclusion
Regular expressions are a powerful tool for searching text or formatting input, and these are just a few primary components. If you want to bring the strength and customizability of your regular expressions to the next level, I recommend you [visit this website](https://www.rexegg.com/regex-disambiguation.html) to learn about additional regex elements.

---

#### Appendix

*Audience:* other COMP 3040 students

*Venue:* a website like Geeks for Geeks

*Purpose:* Instruct the audience on how to use the basic components of Regular Expressions.

*Additional Purpose:* Encourage the student to learn more about regular expressions, or try their own.

*Desired Reaction:* Understanding of the basic componments of regular expressions, confident that they can apply the regular expression elements outlined.

*Vocabulary:* General programming jargon, JavaScript syntax for code examples. Vocabulary that a college-level student should have no trouble understanding.

*Tone:* Brief, concise, to-the-point.

*Examples:* A code or regex example of syntax or expected regex matches for every topic introduced.
---
