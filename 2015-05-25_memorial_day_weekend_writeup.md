###Memorial Day Weekend Writeup
Date completed: 05/25/15

**List and describe each of the primitive data types (number, string, boolean, null, undefined). What do they each represent?**

A primitive type has a fixed size in the computer's memory. 

Primitive data types are:

ALWAYS

- Boolean - logical values, there are just two, `true` and `false`.
- Numbers - such as 0,1,2, 45, -44. These are any number that are positive or negative, have a decimal or not, and also includes `NaN` or Not a Number, and `infinity`.
- Null - is a value meaning equal to nothing, or an empty value.
- Undefined - is a value meaning that the item has not been defined or initialized.

SOMETIMES

- String - Any numbers or letters or characters contained inside of quotations, either double qoutes "" or single quotes''. In class we discussed how strings could be both primitive or relative data types. The MDN documentation lists strings as a primitive data type.

NEW

- Symbol - According the the MDN documentation, symbols are a primitive data type with the newest version of JavaScript (ECMAScript 6).

**Explain what a variable is.**

A variable is a placeholder. It is a word that acts as a placeholder or an identifier, to hold values. Variables need to be initialized in order for us to use them. They can be defined and redefined with new values at any time. 

A reason to use variables instead of the actual value is so that we can change the value in one place, where we first define and initialize it, for example, and then all of our other references to that variable in our program do not also need to be changed.

**Describe in precise terms what’s happening with variable assignment using “var keyword”, “identifier”, “value”, “assign” etc…**

..

**Evaluate the following expression: **

	!(typeof(9) === typeof(9.5) && (99 == "99" || !true))

...

**Use a for loop to iterate through an array.**

	var myArray = [56,43,22,19];

	for (var i = 0; i < myArray.length; i++){
		console.log(i);	 //will show the current item in the array in the console
	}


**Define functions using declarations and expressions.**

..

**Articulate the difference between defining and invoking a function.**

Defining a function is when we describe what the function should do.

Invoking a function is when we tell the function to run, or to do its thing. 

For example, a function `drive` would be an explanation of how to drive a car from point a to point b. And invoking the `drive` function would mean that we actually get into the car and drive it from the given parameters, point a to point b.

**Describe how data flows into a function (by passing in arguments).**

..

**Describe how data flows out of functions (by using the return keyword).**

..

**"Functions are just values" - explain.**

..

**Write functions that return values.**

..

**Write functions that have side effects, such as logging to the console or manipulating DOM.**

..

**Explain the difference between locally-scoped and globally scoped variables and write examples of each.**

..

**Define ‘type coercion’ and identify instances when it occurs.**

..

**Explain what the DOM is. Where does it live? What is it for? How does it get created?**

..

**Describe the CSS Box model. What 5 properties affect the box model?**

..
padding
border
margin
height
width

**What is the difference between relative and absolute poitions in CSS?**

..

**What is the difference between block and inline elements?**

A block element takes up the full width of its container by defualt and inline elements sit next to each other, so multiple inline lemenets can be on the same line.

Examples of block elements are \<p>, \<div>, and \<span> and examples of inline elements are \<a>, \<em>, and \<h1>.

**What does each git command do? git add ., git commit -m “”, git push origin master**

- `git add .` adds all of the files in the current directory (or folder) to the git staging area.
- `git commit -m ""` is typed after files are added to the staging area and -m stands for message. We write a short description of the changes made to the files since the last commit was made inside of the qoutes.
- `git push origin master` pushes all changes that are in our staging area up to our repo. If we are using GitHub to hold our repo, these are pushed to GitHub and we can then see our files that we just added to staging on the branch called "master" on our repo. Master is the default, or main, branch.

**Git Branches: What are they? What are they used for?**

..

**What's the difference between git and github?**

..

**Identify all of the truthy and falsy values in JS and explain what it means to be “truthy” and “falsy”.**

..

**How do you access elements inside of an array?**

..

**What's the difference between arrays and objects?**

..

**How do you create arrays and objects?**

..

**How do you access values inside an object?**

..

**Describe the three components of a for loop.**

..

**Name three types of HTML mouse events.**

..

**What is event propagation?**

..

**What is npm?**

..

**What are npm modules? How do you install an npm module?**

..

**Describe the execution of a while loop and the potential for infinite loops.**

..

