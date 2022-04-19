# HTML Interview Questions & Answers

> Click :star:if you like the project. Pull Requests are highly appreciated. Follow me [@Bhushan-Jangle](https://www.instagram.com/bhu5hanpatil/) .

Go to [Coding Exercise](#coding-exercise) for coding specific questions

### Table of Contents

| No. | Questions |
|---- | ---------
|1  | [What is <!Doctype html> in Html5](#What is <!Doctype html> in Html5) |
|2  | [What is difference between div and span in Html](#What is difference between div and span in Html)|
|3  | [What is semantic tags and non semantic tags in Html](#What is semantic tags and non semantic tags in Html)|
|4  | [What is difference between html and html5](#What is difference between html and html5)|
|5  | [What is Iframe tag in Html5](#what-is-the-purpose-of-the-array-slice-method)|
|6  | [What are the formatting tags in html](#what-is-the-purpose-of-the-array-splice-method)|
|7  | [What is difference <b> and <Strong> in html](#what-is-the-difference-between-slice-and-splice)|
|8  | [What is view port attribute in html](#how-do-you-compare-object-and-map)|
|9  | [What is attribute in html](#what-is-the-difference-between--and--operators)|
|10 | [What is block level element and inline element in html](#what-are-lambda-or-arrow-functions)|
|11 | [What is difference between Html and Html5](#what-is-a-first-class-function)|


1. ### What is <!Doctype html> in Html5

      All HTML documents must start with a <!DOCTYPE> declaration.

      The declaration is not an HTML tag. **It is an "information" to the browser about what document type to expect.**

      In HTML 5, the declaration is simple:

      ```<!DOCTYPE html>```

      **Tip: The <!DOCTYPE> declaration is NOT case sensitive.**
   
      ```<!DOCTYPE html>```
   
      ```<!DocType html>```
   
      ```<!Doctype html>```
   
      ```<!doctype html>```

      
      **[⬆ Back to Top](#table-of-contents)**

2. ### What is difference between div and span in Html

    **Span and div** are both generic HTML elements that group together related parts of a web page. 
    
    **However, they serve different functions.**.
    A div element is used for block-level organization and styling of page elements,
    whereas a span element is used for inline organization and styling.

    **[⬆ Back to Top](#table-of-contents)**

3. ### What is semantic tags and non semantic tags in Html

    **semantic tags**
    A semantic element clearly describes its meaning to both the browser and the developer.

    Examples of semantic elements: <form>, <table>, and <article> - Clearly defines its content.
      
    Examples of non-semantic elements: <div> and <span> - Tells nothing about its content.

    **[⬆ Back to Top](#table-of-contents)**

4. ### What is difference between html and html5

    **HTML** 
    A hypertext markup language (HTML) is the primary language for developing web pages.
    Language in HTML does not have support for video and audio.
      
     1. Easy and simple to use.
     2. Widely supported by almost all the web browsers.
     3. Standard language for making the structure of the web pages.
     4. Code is very lightweight, thus providing better speed online.
     5. Free to use. And it can be run on browsers only, so there is no need to buy any external software.
    
    **HTML5:** 
    HTML5 is a new version of HTML with new functionalities with markup language with Internet technologies.
    HTML5 supports both video and audio.
      
     1. There are many attributes present in HTML5 that were not present in HTML. E.g., data-, offline, onabort, onblur etc.
     2. It provides support for audio, video and other multimedia contents by using tags like <audio>,<video>,<canvas> etc.
        There are many page layouts options available in HTML5. In HTML, you can only find page layouts tags like div, span, etc. But in HTML5, there are many more tag         options available like header, footer, article, section, etc.
     3. HTML5 supports Search Engine Optimisation(SEO). Search engine optimization helps the websites to know about the popularity of their content and also provides           insights on how to improve the content to increase the traffic on the websites.
     4. HTML5 provides more flexible storage options. HTML used the concept of cookies to store temporary data, but HTML5 is capable of using a user-side database like         SQL. It also allows the user to view previously visited page data in offline mode.
     5. HTML5 eliminates the need to write multiple codes for multiple platforms. The code written in HTML5 supports mobile or tablet layout also. Thus it provides             multi-platform compatibility.

    **[⬆ Back to Top](#table-of-contents)**

5. ### What is the purpose of the array slice method

    The **slice()** method returns the selected elements in an array as a new array object. It selects the elements starting at the given start argument, and ends at the given optional end argument without including the last element. If you omit the second argument then it selects till the end.
    
    Some of the examples of this method are,

    ```javascript
    let arrayIntegers = [1, 2, 3, 4, 5];
    let arrayIntegers1 = arrayIntegers.slice(0,2); // returns [1,2]
    let arrayIntegers2 = arrayIntegers.slice(2,3); // returns [3]
    let arrayIntegers3 = arrayIntegers.slice(4); //returns [5]
    ```

    **Note:** Slice method won't mutate the original array but it returns the subset as a new array.

    **[⬆ Back to Top](#table-of-contents)**

6. ### What is the purpose of the array splice method

    The **splice()** method is used either adds/removes items to/from an array, and then returns the removed item. The first argument specifies the array position for insertion or deletion whereas the optional second argument indicates the number of elements to be deleted. Each additional argument is added to the array. 
    
    Some of the examples of this method are,

    ```javascript
    let arrayIntegersOriginal1 = [1, 2, 3, 4, 5];
    let arrayIntegersOriginal2 = [1, 2, 3, 4, 5];
    let arrayIntegersOriginal3 = [1, 2, 3, 4, 5];

    let arrayIntegers1 = arrayIntegersOriginal1.splice(0,2); // returns [1, 2]; original array: [3, 4, 5]
    let arrayIntegers2 = arrayIntegersOriginal2.splice(3); // returns [4, 5]; original array: [1, 2, 3]
    let arrayIntegers3 = arrayIntegersOriginal3.splice(3, 1, "a", "b", "c"); //returns [4]; original array: [1, 2, 3, "a", "b", "c", 5]
    ```

    **Note:** Splice method modifies the original array and returns the deleted array.

    **[⬆ Back to Top](#table-of-contents)**

7. ### What is the difference between slice and splice

    Some of the major difference in a tabular form

    | Slice | Splice |
    |---- | ---------
    | Doesn't modify the original array(immutable)  | Modifies the original array(mutable) |
    | Returns the subset of original array | Returns the deleted elements as array  |
    | Used to pick the elements from array | Used to insert or delete elements to/from array|

    **[⬆ Back to Top](#table-of-contents)**

8. ### How do you compare Object and Map

    **Objects** are similar to **Maps** in that both let you set keys to values, retrieve those values, delete keys, and detect whether something is stored at a key. Due to this reason, Objects have been used as Maps historically. But there are important differences that make using a Map preferable in certain cases.

    1. The keys of an Object are Strings and Symbols, whereas they can be any value for a Map, including functions, objects, and any primitive.
    2. The keys in Map are ordered while keys added to Object are not. Thus, when iterating over it, a Map object returns keys in order of insertion.
    3. You can get the size of a Map easily with the size property, while the number of properties in an Object must be determined manually.
    4. A Map is an iterable and can thus be directly iterated, whereas iterating over an Object requires obtaining its keys in some fashion and iterating over them.
    5. An Object has a prototype, so there are default keys in the map that could collide with your keys if you're not careful. As of ES5 this can be bypassed by using map = Object.create(null), but this is seldom done.
    6. A Map may perform better in scenarios involving frequent addition and removal of key pairs.

    **[⬆ Back to Top](#table-of-contents)**

9. ### What is the difference between == and === operators

    JavaScript provides both strict(===, !==) and type-converting(==, !=) equality comparison. The strict operators take type of variable in consideration, while non-strict operators make type correction/conversion based upon values of variables. The strict operators follow the below conditions for different types,
    1. Two strings are strictly equal when they have the same sequence of characters, same length, and same characters in corresponding positions.
    2. Two numbers are strictly equal when they are numerically equal. i.e, Having the same number value.
       There are two special cases in this,
       1. NaN is not equal to anything, including NaN.
       2. Positive and negative zeros are equal to one another.
    3. Two Boolean operands are strictly equal if both are true or both are false.
    4. Two objects are strictly equal if they refer to the same Object.
    5. Null and Undefined types are not equal with ===, but equal with ==. i.e,
        null===undefined --> false but null==undefined --> true

    Some of the example which covers the above cases,

    ```javascript
    0 == false   // true
    0 === false  // false
    1 == "1"     // true
    1 === "1"    // false
    null == undefined // true
    null === undefined // false
    '0' == false // true
    '0' === false // false
    []==[] or []===[] //false, refer different objects in memory
    {}=={} or {}==={} //false, refer different objects in memory
    ```

    **[⬆ Back to Top](#table-of-contents)**

10. ### What are lambda or arrow functions

    An arrow function is a shorter syntax for a function expression and does not have its own **this, arguments, super, or new.target**. These functions are best suited for non-method functions, and they cannot be used as constructors.

    **[⬆ Back to Top](#table-of-contents)**

11. ### What is a first class function

    In Javascript, functions are first class objects. First-class functions means when functions in that language are treated like any other variable.

    For example, in such a language, a function can be passed as an argument to other functions, can be returned by another function and can be assigned as a value to a variable. For example, in the below example, handler functions assigned to a listener

    ```javascript
    const handler = () => console.log ('This is a click handler function');
    document.addEventListener ('click', handler);
    ```

    **[⬆ Back to Top](#table-of-contents)**

12. ### What is a first order function

    First-order function is a function that doesn’t accept another function as an argument and doesn’t return a function as its return value.

    ```javascript
    const firstOrder = () => console.log ('I am a first order function!');
    ```

    **[⬆ Back to Top](#table-of-contents)**
