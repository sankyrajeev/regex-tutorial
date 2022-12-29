# Regex Tutorial (Matching an Email)

In this tutorial we will try to understand the use of of regex to match emails with the following expression :
```
 /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```
 We use the expression to validate emails in our applications.

# Summary

A regular expression is a sequence of characters that defines a search pattern. This is commonly used to find patterns within a string, find/replace characters within a string or validate input. This tutortial will go walk through the components of a regex and how it applies to matching an email.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

# Regex Components


## **Anchors**



There are different kinds of anchors used in this pattern. The one's we have used are  ```  ^  ``` , which describes beginnening of a string value.
``` $ ``` is to indicate the end of a string.

## **Quantifiers**

We use th ``` + ``` operator which connects the name of the email , the service and  ```.com```. The ```{1,6}```allows range of 1-6 characters to match with a set of [a-z\.].



## **Character Classes**

This expression has a class ``` \d ``` which matches a individual characters of digits from 0-9. It matches individual numbers only.



## **Grouping and Capturing**

Capturing group in this expression is ([a-z0-9_\.-]+) that matches the user email name. The second capturing group is ([\da-z\.-]+) which will match the email service. Then lastly, capture group #3 is ([a-z\.]{2,6}) to capture the .com.

## **Bracket Expressions**

Bracked expressions for email validation includes the character sets of [a-z0-9_\.-], which is matching any letter a-z and is case senstive. It also matches a character 0-9 and matches the characters "_" , "-" , and "."; [\da-z\.-], which is matching a single digit from 0-9, any character a-z (case senstive), and the characters "." and "-".; [a-z\.] matches any character a-z(case senstive) and the character ".".

##  **Greedy and Lazy Match**

The following regex uses Greedy and Lazy match. Since it incldues  ```+ ``` it will match as many times as possible as needed. 
 Another greedy Quantifier used in this regex is ``` {} ``` when matching ```{2,6}``` for the last capture group.



## Author

Find my projects at https://github.com/sankyrajeev?tab=repositories
