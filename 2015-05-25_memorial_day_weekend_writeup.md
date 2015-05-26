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

The CSS Box model is the visual box model, or interpretation, of any HTML element. The inside of the box is the content. So, for example, if you have HTML of `<p>This is a little box!</p>` the content inside of the box is the text "This is a little box!", the element is the \<p> and the height and width can be set to a size. Immediately surrounding the content inside is the padding. Immediately surrounding the padding is the border. Immediately surrounding the border is the margin. 

Think of the margin as the piece that touches other elements' margins on the page. The padding is the space between the content and the border. The border is invisible by default but it can be shown by adding a size and color to it.

The 5 properties that affect the box model are:

- padding
- border
- margin
- height
- width

**What is the difference between relative and absolute positions in CSS?**

The relative position means "relative to itself." If you do not set any of the positioning attributes (top, left, bottom, right), then you will see no change. If you set `top: 10px;` for example, then the element will shift 10px down from where it would originally have been positioned. Giving an element `postion: relative` will also set it on top of any elements that are `position: static`. Also, any element that is a child of the relatively positioned element can be absolutely positioned within that block.

The absolute position means you can set the element to an exact location on the page, relatice to the next parent element, by giving it coordinates to use for the positioning attributes (top, left, bottom, right). These elements are taken out of the normal flow of elements (which is from top to bottom as they are found in the HTML document).

**What is the difference between block and inline elements?**

A block element takes up the full width of its container by defualt and inline elements sit next to each other, so multiple inline lemenets can be on the same line.

Examples of block elements are \<p>, \<div>, and \<span> and examples of inline elements are \<a>, \<em>, and \<h1>.

**What does each git command do? git add ., git commit -m “”, git push origin master**

- `git add .` adds all of the files in the current directory (or folder) to the git staging area.
- `git commit -m ""` is typed after files are added to the staging area and -m stands for message. We write a short description of the changes made to the files since the last commit was made inside of the qoutes.
- `git push origin master` pushes all changes that are in our staging area up to our repo. If we are using GitHub to hold our repo, these are pushed to GitHub and we can then see our files that we just added to staging on the branch called "master" on our repo. Master is the default, or main, branch.

**Git Branches: What are they? What are they used for?**

The are versions of our files. We can create a new branch, move to it, and alter our files, then when we go back to the old branch, our files are in the state that we last saved them on that old branch. Our new branch has our files in a different state.

Typically people use branches when they are collaborating on the same files with other people. Each person creates their own branch to work on, makes all of the changes they want to, then merges their branch back onto the master branch. Any conflicts need to be edited by hand before the new branch can be merged to the master branch. The master branch is like the production branch, or the "always the most current working version" that other people will copy from before they start editing files.

**What's the difference between git and github?**

git is version control. We use it to keep copies of our files every time we commit the files using the `git commit <file name>` command. It's like saving a snapshot of our file at that point in time. We can keep track of as many versions of our file as we want.

GitHub is a website where we can view our file version and provides a visual way to see what the differences are between versions. We use it to collaborate with other people on repositories. Each person uses git on their local machine to save, stage, and push changes up to the repository on GitHub.

**Identify all of the truthy and falsy values in JS and explain what it means to be “truthy” and “falsy”.**

Falsy values are:

- 0 (zero)
- "" (empty string)
- false
- null
- undefined
- NaN

All other values are truthy. Examples of truthy are:

- true
- {}
- []
- any number that is not zero
- a string

To be "truthy" something "exists". When it is evaluated in a Boolean context, as whether or not it is something that exists, it returns "true".

Falsy values are empty values or are values that do not exist. They return as false when evaluated in a Boolean context.

**How do you access elements inside of an array?**

There are a few ways to do this. To access just a single item, we would use the built-in method indexOf followed by a number, to get the element at the index with the corresponding number. 

Additionally, ee could use a for loop to iterate through each item in the array and use the variable to correspond to the index of the array item. We could also use the built-in method forEach to loop through each item, simliar to the for loop.

**What's the difference between arrays and objects?**

An array is like a list, but with brackets [ ]. The items in the array can be accessed by their spot (index) in the array, moved around, added to or subtracted from the array.

An object is like an array, but with keys (names) instead of indexes, to access specific values in the object. Anything can be put inside of an object and and object is usually designated by curly braces { }.

**How do you create arrays and objects?**

Syntax:

- array is shown using [ ]
- object is shown using { }

Items inside of both are separated with a comma. We can initialize them like so:

	var myArr = [1,3,"third element in array"];

	var myObj = { key1 : "value 1", key2 : "value2" };


**How do you access values inside an object?**

With the name of the key. Items inside of objects are in pairs of key(name):value. Calling the object name followed by the key name would give us the value of the item at that key.

**Describe the three components of a for loop.**

First we set a variable equal to a starting value (initialize it), then we give an ending value, that the variable will be true until it reaches this ending value (conditional or test statement), and thirdly we change the variable so that it moves towards the ending value (iteration). An example would be to start at zero, end at 10, and add 1 to the value until the variable value is equal to 10.

**Name three types of HTML mouse events.**

Click, dbclick (double click), and mouseover are all mouse events.

**What is event propagation?**

When an eventListener is added to an element on a page, and the eventListener is called, it is also called on any element that is either a parent of that element or a child of that element. The direction of the propagation is determined by an argument of 'true' or 'false' passed in as the third argument to the eventListener. 

The default behavior of eventListeners is to "bubble upwards" and the corresponding argument for this is 'false'. If this is set, then the element and all parent elements, including the and the document, will all have the eventListener applied to them. For example, clicking on a \<p> inside of a \<div> causes the action inside of the event handler to be applied to the \<p>, then the \<div>, then the \<body>, then the document.

If the third eventListener argument is set to 'true' then the element and all children elements inside of it, get the eventListener applied to them.

**What is npm?**

npm is a package manager for code, or a way to share modules of code with other people. It is sort of like version control for smaller pieces of code that people share via the npm registry.

**What are npm modules? How do you install an npm module?**

npm module are files with code that are created to be modular. This means that they can be re-used for different purposes and modified. Instead of having one gigantic program, we break the program apart into modules that do very specific things, and then we can re-use those modules in other programs or repeatedly inside of the same program.

You can install an npm module from the command line with the command `npm install <package name>`.

**Describe the execution of a while loop and the potential for infinite loops.**

A while loop runs repeatedly while a certain condition is true. We need to include a way to alter the value that the condition is testing in order for the while loop to stop at some point. If the contition is always true, then it will run infinitely and then our program is stuck in a loop, or our browser running the program will not be able to continue doing other things on that tab.

