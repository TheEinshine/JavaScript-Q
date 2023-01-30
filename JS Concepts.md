1.  What are the primitive data types in JS?
    => 1. string 2. number 3. bigint 4.boolean 5.undefined 6.symbol 7.null
    these are 7 types of different types of primitive datatype out there.
    A primitive (primitive value, primitive data type) is data that is not an object and has no methods or properties.

2.  What's the difference between a variable that is: null, undefined or undeclared?
    => 1. so firstly let's take undeclared, if some variable is undeclared means it's not declared or initialized. it means the variable does not exist because it has never been created. 2. undefined is one of JavaScript primitive type. A variable is undefined when the variable has been declared but not assign a value. it does not mean that variable does not exist. it means that the variable exist because it's been created. but does not have a value. 3. null, null is one of JavaScript's primitive types. The value null is used for purposefully setting something to empty, the absence of a value. When null is used, it means a variable is declared and has a value of a null.

3.  What is the difference between while and do-while loops in JavaScript?
    => the while statement creates a loop that executes a specified statement as long as the test condition evaluates to true. the condition is evaluated before executing the statement.
    do while loop. the do while statement creates a loop that executes a specified statement until the test condition evaluates to false. The condition is evaluated after executing the statement, resulting in the specified statement executing at least once.

4.  What language constructions do you use for iterating over object properties and array items?
    => for loops - for (let i in obj) (log(i)); However, this will also iterate through it's inherited properties, and you will add an obj.jasOwnProperty(i) check before using it.
    Object.keys() - Object.keys(obj).forEach(function (i)) {...}).Object.keys() is a static method that will lists all enumerable and non-enumerable properties of the object that you pass it.

5.  What are the promises and how do they work?
    => A promises is an asynchronous action that may complete at some point in the future and produce a value. This value is not necessarily known at the time of its creation. Once the value is produced, it notifies the user.
    Promise provide a robust way to wrap the result of asynchronous work, overcoming the problem of deeply nested callbacks.
    The Promises object takes a callback function as a parameter, resolve and reject. The promise is either fulfilled or reject. The promise is either fulfilled or rejected.

6.  What are IIFEs and explain with an example where they can be used?
    => Uses of IIDE An IIFE (immediately invoked function expression) can be used for avoiding the variable hoisting from within the blocks. it allows the public access to methods while retaining the privacy for variables defined in the function. IIFE is a design pattern that is also known as the Self-Executing Anonymous Functions.

7.  Explain event delegation.
    => Event Delegation is basically a pattern to handle events efficiently. instead of adding an event listener to each and every similar element, we can add an event listener to each and every similar element, we can add an event listener to a parent element and call an event on a particular target using the. target property of the event object.

8.  Explain how this works in JavaScript.
    a.Can you give an example of one of the ways that working with this has changed in ES6?
    => JavaScript ES6 brings new syntax and new awesome features to make your code more modern and more readable. it allows you write less code and do more. ES6 introduce us too many great features like arrow functions, template strings, class destruction, module and more.

9.  Explain how prototypal inheritance works.
    => The Prototypal Inheritance is a feature in javascript used to add methods and properties in objects. it is a method by which an object can inherit the properties and methods of another object. Traditionally, in order to get and set the [[Prototype]] of an object, we use Object. getPrototypeOf and Object.

10. What is a closure, and how/why would you use one?
    => A closure is the combination of a function bundled together (enclosed) with references to its surrounding state (the lexical environment). In other words, a closure gives you access to an outer function's scope from inner function.

11. Can you describe the main difference between the Array.forEach() loop and Array.map() methods and why you would pick one versus the other?
    => the forEach() method does not return a new array, wheres the map() method returns a new array. the map() method is used to transform the elements of an array, wheres the forEach() method is used to loop through the elements of an array.
    the normal loop is just to iterate over array or any other element till specific condition reaches, it also does not return any new array.

12. What's a typical use case for anonymous functions?
    => A typical use of anonymous function is used when we have urgency on the return value or certain piece of code to get execute inline.

13. What's the difference between host objects and native objects?
    => native object in ECMAScript implementation whose semantics are fully defined by this specification rather than by the host environment.
    host object supplied by the host environment to complete the execution environment of ECMAScript.

14. Explain the difference between: function Person(){}, var person = Person(), and var person = new Person()?
    => so function Person(){} is a function declaration
    code above declares a function statement (statements perform an action) but does not execute, however, it does get registered into the global namespace.

    var person = person() is a function expression
    a variable 'var person' has defined and contains a value reference to a Person function. Any JavaScript Expressions (including Function Expressions) always returns a value.
    This may also be an Anonymous function if no name has been assign to a function to a function but wrapped in parenthesis to be interpreted as an expression.

    var person = new Person() is function Constructor
    By adding the keyword 'new'. We are instantiating a new object of the Person class constructor. A function declaration is just a regular function unless it has been instantiated, it then becomes a class constructor.

15. Explain the differences on the usage of foo between function foo() {} and var foo = function() {}
    => function foo(){} is a Normal Function or traditional general way of Function Declaration which every developer finds it simpler to declare and use it every ever required and var foo = function() {} is a Anonymous Function Declaration syntax or Expression Function wrapped in via a variable or a in simple words.

16. Can you explain what Function.call and Function.apply do? What's the notable difference between the two?
    => The difference is: The call() method takes arguments separately . The apply() method takes arguments as an array. the apply() method is very handy if you want to use an array instead of argument list.

17. Explain Function.prototype.bind.
    => prototype blind() The blind() method creates a new function thatm when called, has its this keyword set to the provided value, with a given sequence of arguments preceding any provided when the new function is called

18. What's the difference between feature detection, feature inference, and using the UA string?
    => Feature Detection
    Feature detection is just a way of determining if a feature exists in certain browsers. A good example is a modern HTML5 feature ‘Location’
    Feature Inference
    Feature Inference is when you have determined a feature exists and assumed the next web technology feature you are implementing unto your app exists as well. Its usually bad practice to assume, so its better to explicitly specify features you want to detect and plan a fallback action.
    UA String
    UA String or User Agent String is a string text of data that each browsers send and can be access via navigator.userAgent. These “string text of data” contains information of the browser environment you are targeting.
    If you open your console and run

19. Explain "hoisting".
    => JavaScript Hoisting refers to the process whereby the interpreter appears to move the declaration of functions, variables or classes to the top of their scope, prior to the execution of the code. Hoisting is not a term normatively defined in the ECMASCript specification.

20. Describe event bubbling.
    => Event Bubbling is a concept in the DOM (Document Object Model) it happens when an element receives an event, and that event bubbles up (or you can say is transmitted ot propagated) to its parent and ancestor elements in the DOM free until it gets to the root element

21. Describe event capturing.
    => Event capturing is one of the two wats to do event propagation in the HTML DOM in event capturing, an event propagates from the outermost elements to the target element. it is the opposite of event bubbling, where events propagate outwards from the target to the outer elements. Capturing happens before bubbling.

22. What's the difference between an "attribute" and a "property"?
    => A property is a single attribute-like name that wraps a collection of setter, getter (and deleter) functions. An attribute is usually a single object within another object.

23. What are the pros and cons of extending built-in JavaScript objects?
    => The main argument against doing this is: if, in future, a browser decides to implement its own version of your method, your method might get overridden (silently) and the browser's implementation (which is probably different from yours) would take over. So not extending in the first place is future proofing your code.

24. What is the difference between == and ===?
    =>The == operator checks if two values are equal. The != operator checks if two values are not equal. It is also known as the loose equality operator because it checks abstract equality, i.e., it tends to convert the data types of operands in order to carry the comparison when two operands aren't of the same data type

25. Explain the same-origin policy with regards to JavaScript.
    => The same-origin policy is a critical security mechanism that restricts how a document or script loaded by one origin can interact with a resource from another origin. It helps isolate potentially malicious documents, reducing possible attack vectors.

26. Why is it called a Ternary operator, what does the word "Ternary" indicate?
    =>The name ternary refers to the fact that the operator takes three operands. The condition is a boolean expression that evaluates to either true or false

27. What is strict mode? What are some of the advantages/disadvantages of using it?
    => The statement “use strict”; instructs the browser to use the Strict mode, which is a reduced and safer feature set of JavaScript. Benefits of using 'use strict': Strict mode makes several changes to normal JavaScript semantics. Strict mode eliminates some JavaScript silent errors by changing them to throw errors.

28. What are some of the advantages/disadvantages of writing JavaScript code in a language that compiles to JavaScript?
    => Advantages of JavaScript Development. Inherently Fast. Simplicity. Interoperability. Popularity. Reduced Server Load. ...
    Disadvantages of JavaScript Development. Permissive Nature. Client-side Security. Debugging on the web can be Inherently Tricky. Browser Inconsistency.
    Weighing Up JavaScript Development.

29. What tools and techniques do you use debugging JavaScript code?
    => Developer tools in modern web browsers. Every modern browser has tools available within it to debug code, the best is inbuilt tool

30. Explain the difference between mutable and immutable objects.
    a. What is an example of an immutable object in JavaScript?
    b. What are the pros and cons of immutability?
    c. How can you achieve immutability in your own code?

    a.immutable object : The object being frozen is said to be immutable because the entire object state (values and references to other objects) within the whole object is fixed. Note that strings, numbers, and booleans are always immutable and that Functions and Arrays are objects

    b.immutability : With all the benefits mentioned in the above section, immutable objects have only one disadvantage: When you need to change the state of an object, you have to create a new object which is an overhead and causes frequent garbage collection. Moreover, if these objects are large, they can be costly.

    c: how to achieve immutability : You can freeze (make immutable) an object using the function Object. freeze(obj) . The object passed to the freeze method will become immutable. The freeze() method also returns the same object.

31. Explain the difference between synchronous and asynchronous functions.
    => Asynchronous is a non-blocking architecture, so the execution of one task isn't dependent on another. Tasks can run simultaneously. Synchronous is a blocking architecture, so the execution of each operation is dependent on the completion of the one before it.

32. What is an event loop?
    => Event loop: An event loop is something that pulls stuff out of the queue and places it onto the function execution stack whenever the function stack becomes empty.

        a. What is the difference between call stack and task queue?

    => Call stack -->Every time a script or function calls a function, it's added to the top of the call stack. Task queue---> A task is any JavaScript code which is scheduled to be run by the standard mechanisms such as initially starting to run a program, an event callback being run, or an interval or timeout being fired

33. What are the differences between variables created using let, var or const?
    => var variables can be updated and re-declared within its scope; let variables can be updated but not re-declared; const variables can neither be updated nor re-declared. They are all hoisted to the top of their scope. But while var variables are initialized with undefined , let and const variables are not initialized.

34. What are the differences between ES6 class and ES5 function constructors?
    => In the ES5 version, constructor functions are declared using the function keyword, with the body of the code initializing the object properties upon its creation. The ES6 version, on the other hand, uses the constructor keyword to declare the constructor function which runs on object creation.

35. Can you offer a use case for the new arrow => function syntax? How does this new syntax differ from other functions?
    => How does the arrow function differ from other functions?
    Unlike regular functions, arrow functions do not allow duplicate parameters, whether in strict or non-strict mode. Duplicate parameters will cause a Syntax Error to be thrown. In this article, I have discussed some significant differences between regular functions and arrow functions in JavaScript.
    it can shorten and make your function quicker.

36. What advantage is there for using the arrow syntax for a method in a constructor?
    =>This arrow function reduces lots of code and makes the code more readable. Arrow function syntax automatically binds “this” to the surrounding code's context. Writing the arrow => is more flexible as compared with the writing function keyword.

37. What is the definition of a higher-order function?
    => A higher order function is a function that takes a function as an argument, or returns a function . Higher order function is in contrast to first order functions, which don't take a function as an argument or return a function as output.

38. Can you give an example for destructuring an object or an array?
    => Destructuring is used to more easily assign values taken directly from an object or an array. Let's start by taking a look at an example of an object and the process required to extract its values prior to ES6: var obj = {first: 'Rick', last: 'Sanchez', age: 70}; var first = obj.

39. Can you give an example of generating a string with ES6 Template Literals?
    => ```
var name = 'World';  
var cname = 'Abhi';  
console.log(`Hello, ${name}!  
     Welcome to ${cname}`);  
     Output
    Hello, World!
    Welcome to Abhi

```

40. Can you give an example of a curry function and why this syntax offers an advantage?
=> function multiply(a, b, c) {

    return a * b * c;
}

function multiply_curried(a) {

    return function (b) {
        return function (c)  {
            return a * b * c
        }
    }
}

let res = multiply(1, 2, 3);
console.log(res);

let mc1 = multiply_curried(1);
let mc2 = mc1(2);
let res2 = mc2(3);
console.log(res2);

let res3 = multiply_curried(1)(2)(3);
console.log(res3);
We have normal multiply function, which multiplies its three arguments. The code multiply_curried uses currying to get the multiplication done.

let res = multiply(1, 2, 3);
This is the classic function call; all its parameters are passed between the round brackets.

let mc1 = multiply_curried(1);
let mc2 = mc1(2);
let res2 = mc2(3);
console.log(res2);
In currying, the function takes one argument and returns another function, which takes the next argument, until all arguments are exhausted.

let res3 = multiply_curried(1)(2)(3);
This is the shorthand notation of the previous code.

41. What are the benefits of using spread syntax and how is it different from rest syntax?
=>Spread syntax looks exactly like rest syntax. In a way, spread syntax is the opposite of rest syntax. Spread syntax "expands" an array into its elements, while rest syntax collects multiple elements and "condenses" them into a single element.

42. How can you share code between files?
=> To share code between components, create an ES6 module in a service component and export the variables or functions that you want to share using standard JavaScript syntax. An ES6 module is a JavaScript file that explicitly exports variables or functions that other modules can use.

43. Why you might want to create static class members?
=> => Public static fields are useful when you want a field to exist only once per class, not on every class instance you create. This is useful for caches, fixed-configuration, or any other data you don't need to be replicated across instances.
```
