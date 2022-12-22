# Regex Tutorial: Email

With this tutorial we will dive deeper into regex to fully understand how email matching works.

## Summary

Through out the tutorial we are going to be going through a sample email regex. this will help us go thruoth the different symbols and characters to know they mean
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
In an email regex and our example we use ^ as our starteer anchor and $ as our end anchor. As we see in our sample there is an ^ and $, and we are use what is within those to match the email.

### Quantifiers
Quantifiers state of many of a certin string should be there in order to be considere as a match. It is determend for a group, We will talk about groups later. If a group is marked with +, it means that there needs to be atleast one character in that group to match. Another example would be {2,6}, this owuld indicated that a minimum of 2 and maximum of 6 characters could be in the group inorder to match

### Grouping and Capturing
Grouping helps us seperate string in out email regex. Each group is make with (). With grouping you are able to set parameters just for that specific group and not the entier string.

### Bracket Expressions
Brakets [] are used to specify the parameters that need to be followed inorder to match. 

### Character Class
Character class we are able to preset what we want used inorder to match. We can use only number or letters or both. [a-z] means only letters may be used in order to match, and it is case sensative. Inorder to use number you could use \d or [0-9].

### Sample
Our sample code has a couple groups within the string. We start of with a string thats greater then 1 and consists of letters and numbers, then we have to have an @ sign. After we another sting that consister of number/letters and needs to be greater then 1. Next there is a period and finished with a set of letters that add up to greater then 2 and less then 6.

## Author

My name is Artem Khomenko, I am currently enrolled in UW coding boothcamp. Checkout my github: https://github.com/Artemk2002