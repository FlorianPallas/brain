# Pure Javascript
## Variables
- let for normal variables
- const for constants
- Javascript is weakly typed, so variables can change their type
- Primitive types (stored in the stack) :: Strings, Numbers, Booleans, null, undefined, Symbol
	- Variables stores the actual value
- Reference types (stored in the heap) :: All objects
	- Variables store a reference
- Converting string to int: let inputNumber = parseInt(inputString);
	- Note if the inputString can't be converted the inputNumber is assigned to NaN. You can check of NaN with the function isNaN(inputNumber)
- Converting variables to string: number.toString();
- Default value for uninitialised variables = undefined
- The **null** can be set by the user to variables.
- The type of a variable can be checked with the **typeof** operator
### Strings
- It does't matter if you use ' or " but it needs to be the same for one string. E.g. "Hello World", 'Hello World'
- \\ escapes ' or " 
#### Template literals
- Special kind of strings in which variables can be embedded. It is opened and closed with this char: \`
- E.g. const calculationDescription =  \`The result is: ${currentResult}\`; 
 ### Numbers
 - Either integer or float
 ### Booleans
-  true or false
- Special cases
	- 0 is false and any other number is true
	- '' is false and any other string is true
	- any initialised object or array is true
	- null, undefined and NaN are false
 ### Objects
- An object is a key value pair
- Creation of an object: const myObject = { name: 'Lukas', age: 20 };
- Retrieving data: const name = myObject.name; or const name = myObject['name'];
### Arrays
- Type of object that represents a list of data. E.g. const myList = [1,2,3];
- Retrieving an element: nameOfArray[index];
- Retrieving the number stored in the array :: const length = myArray.length;

## Operators
- Assignment operators: +, -, \*, \*\*, /, %, +=, -=, \*=, /=, ++, -- 
- Boolean Value equality: == and !=
	- Ignores the type e.g. 2 == '2' = true
- Boolean Value and Type equality: === and !==
- Greater and Less than operators: <, <=, =>, >
	- Note they can compare two numbers normally or two strings after their lexicographical order
- Ternary Operator (if the given condition is true it assignees the first option and if it is false it assignees the second option) :: const userName = isLogin ? 'Max' : null;
- Spread operator (spreads out an array or an object - used for object and list creation to bypass the reference type nature) :: ...
- Rest operator (collects function arguments and puts them in a list, needs to be the last parameter) :: function sum(a, b, ...numbers){} sum(1,2,3,4,5);

## Control structures
- if(){}, else if(){}, else{}
- Classic switch statement :: switch(input){ case 'start': runSth(); break; case 'quit' runSthElse(); break; default: break;}
	- Short way of writing if(input === 'start'){} else if(input === 'quit'){}
- Classic for loop :: for(let i = 0; i < 5; i++){}
- for-of loop - loops over every element in an array myArray:: for(const myElement of myArray){}
- for-in loop - loops over every key in an object myObject :: for(const myKey in myObject){}
- classic while loop :: while(condition){}
- classic do-while loop :: do{} while(condition);
- break and continue can be used in every control structure
- Classic try catch :: try{} catch(error){}

 ## Functions
 - Functions are objects
 - Method :: is a function that an object has as a property
 - Parameters are the defined variables a function takes as input and arguments are the concrete values that are passed into the function
 - Defining a function: function greetUser(name){ alert('Hello' + name); }
 - Calling a function: greetUser('Lukas');
 - Storing a functions into a variable. E.g. const greeting = function greet(){}; or simply const greeting = () => {};
	 - If the body of the arrow function only has one line the curly braces can be omitted. Note: The return keyword also has to be removed. E.g. (a,b) => a+b; is the same as (a,b) => {return a+b};
 - You can call a function with less arguments than parameters are defined. JS then just treats the missing arguments as undefined if no default value is defined or uses the default argument if present. Defining default arguments: function(a, b=0){return a+b}
 - myFunction.bind(this, firstArgument) preloads the myFunction with the first argument but does not call the function yet

## Exceptions
- Throwing an error (technically everything can be thrown but the following is the convention) :: throw { message: 'Error message'};
- It is best practice to log errors using console.error() instead of console.log()

## Comments
- Single line comments: //
- Multiline comment: /\* \*/


 # JS with HTML
 ## Document Object Model (DOM)
 - The browser parses and renders the html file and provides an API for JS to manipulate the DOM and the window object.
 ## Importing Scripts
 - Use the HTML Script Tag in the header, so the scripts are loaded at the beginning 
	 - use the *defer* keyword to execute them only when the HTML is done being parsed
	 - use the *async* keyword to execute them as soon as the browser has capacity
 - E.g.  \<script src="assets/scripts/app.js" defer>\</script>
 ## Messages
 - alert(stringMessage) shows an alert box with the string message
 - prompt(stringMessage, initValue) shows a box with the string message and an input box with the initValue 
 ## Input Boxes
 - Input is always a string and needs to be parsed to a number if calculations should be performed. 
 ## Event Listener
 - Either create the attribute onClick="functionName()" in HTML tag or add it through JS with document.getElementById('buttonId').addEventListener('click', functionName);