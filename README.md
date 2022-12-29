#Javascript-notes

# Javascript-notes-JavaScript is Everywhere. Millions of web pages are built on JavaScript and it’s not going anywhere at least for now. On one side HTML and CSS give styling to the web pages but on the other side, it’s the magic of JavaScript that makes your web page alive. Today this language is not just limited to your web browser. You can also use it for server-side applications. Isn’t it cool to use a single language for both client-side and server-side applications? A single language fulfills both of the purposes and this is the main reason TON of job posting is there for javascript developers in the tech industry. 
According to Stack Overflow Developer Survey 2019, JavaScript is the #1 programming language. The language is widely used by 95% of all the websites Whether it’s a small startup or a big company, most of them are working on some kind of website or an app that requires a good knowledge of this language. A lot of frameworks and libraries are there for javascript. These frameworks and libraries can be easily learned if your javascript fundamentals are clear. A lot of concepts are confusing and overwhelming for developers but a good knowledge of these concepts will help you in the long run. Frameworks and libraries come and go but the fundamentals always remain the same. It’s easy to build any kind of application and learn any framework and libraries if the fundamentals are clear. Also, it will help you in interviews as well. Let’s discuss some of the basic concepts of javascript which are important to learn for any JavaScript developer. Become a good front-end developer with Geeksforgeeks JavaScript Foundation – Self Paced and learn all the aspects of web development with ease. 
Variables
Most of the time, a JavaScript application needs to work with information. Here are two examples:
1.	An online shop – the information might include goods being sold and a shopping cart.
2.	A chat application – the information might include users, messages, and much more.
Variables are used to store this information.
A variable
A variable is a “named storage” for data. We can use variables to store goodies, visitors, and other data.
To create a variable in JavaScript, use the let keyword.
The statement below creates (in other words: declares) a variable with the name “message”:
let message;
Now, we can put some data into it by using the assignment operator =:
let message;

message = 'Hello'; // store the string 'Hello' in the variable named message
The string is now saved into the memory area associated with the variable. We can access it using the variable name:
let message;
message = 'Hello!';

alert(message); // shows the variable content
To be concise, we can combine the variable declaration and assignment into a single line:
let message = 'Hello!'; // define the variable and assign the value

alert(message); // Hello!
We can also declare multiple variables in one line:
let user = 'John', age = 25, message = 'Hello';
That might seem shorter, but we don’t recommend it. For the sake of better readability, please use a single line per variable.
The multiline variant is a bit longer, but easier to read:
let user = 'John';
let age = 25;
let message = 'Hello';
Some people also define multiple variables in this multiline style:
let user = 'John',
  age = 25,
  message = 'Hello';
…Or even in the “comma-first” style:
let user = 'John'
  , age = 25
  , message = 'Hello';
Technically, all these variants do the same thing. So, it’s a matter of personal taste and aesthetics.
var instead of let
In older scripts, you may also find another keyword: var instead of let:
var message = 'Hello';
The var keyword is almost the same as let. It also declares a variable, but in a slightly different, “old-school” way.
There are subtle differences between let and var, but they do not matter for us yet. We’ll cover them in detail in the chapter The old "var".
Javascript Data Types
JavaScript provides different data types to hold different types of values. There are two types of data types in JavaScript.
1.	Primitive data type
2.	Non-primitive (reference) data type
JavaScript is a dynamic type language, means you don't need to specify type of the variable because it is dynamically used by JavaScript engine. You need to use var here to specify the data type. It can hold any type of values such as numbers, strings etc. For example:
1.	var a=40;//holding number  
2.	var b="Rahul";//holding string  
JavaScript primitive data types
There are five types of primitive data types in JavaScript. They are as follows:
Data Type	Description
String	represents sequence of characters e.g. "hello"
Number	represents numeric values e.g. 100
Boolean	represents boolean value either false or true
Undefined	represents undefined value
Null	represents null i.e. no value at all
JavaScript non-primitive data types
The non-primitive data types are as follows:
Data Type	Description
Object	represents instance through which we can access members
Array	represents group of similar values
RegExp	represents regular expression


Loops in JavaScript

Looping in programming languages is a feature that facilitates the execution of a set of instructions/functions repeatedly while some condition evaluates to true. For example, suppose we want to print “Hello World” 10 times. This can be done in two ways as shown below:
Iterative Method: The iterative method to do this is to write the document.write() statement 10 times. 
<script type="text/javascript">
	document.write("Hello World<br>");
	document.write("Hello World<br>");
	document.write("Hello World<br>");
	document.write("Hello World<br>");
	document.write("Hello World<br>");
	document.write("Hello World<br>");
	document.write("Hello World<br>");
	document.write("Hello World<br>");
	document.write("Hello World<br>");
	document.write("Hello World<br>");
</script>
Using Loops: In Loop, the statement needs to be written only once and the loop will be executed 10 times as shown below: 
•	JavaScript
    for (let i = 0; i < 10; i++)
    {
         document.write("Hello World!<br>");
    }
Many things may seem confusing to you in the above program at this point of time but do not worry you will be able to understand everything about loops in JavaScript by the end of this tutorial. You can observe that in the above program using loops we have used the document.write statement only once but still, the output of the program will be the same as that of the iterative program where we have used the document.write statement 10 times. In computer programming, a loop is a sequence of instructions that is repeated until a certain condition is reached.
•	An operation is done, such as getting an item of data and changing it, and then some condition is checked such as whether a counter has reached a prescribed number.
•	Counter not Reached: If the counter has not reached the desired number, the next instruction in the sequence returns to the first instruction in the sequence and repeats it.
•	Counter reached: If the condition has been reached, the next instruction “falls through” to the next sequential instruction or branches outside the loop.
There are mainly two types of loops:
1.	Entry Controlled loops: In these types of loops, the test condition is tested before entering the loop body. For Loops and While Loops are entry-controlled loops.
2.	Exit Controlled loops: In these types of loops the test condition is tested or evaluated at the end of the loop body. Therefore, the loop body will execute at least once, irrespective of whether the test condition is true or false. The do-while loop is exit controlled loop.
JavaScript mainly provides three ways for executing the loops. While all the ways provide similar basic functionality, they differ in their syntax and condition checking time. Let us learn about each one of these in detail.
while loop: A while loop is a control flow statement that allows code to be executed repeatedly based on a given Boolean condition. The while loop can be thought of as a repeating if statement. 
Syntax :
while (boolean condition)
{
   loop statements...
}
•	While loop starts with checking the condition. If it is evaluated to be true, then the loop body statements are executed otherwise first statement following the loop is executed. For this reason, it is also called the Entry control loop
•	Once the condition is evaluated to be true, the statements in the loop body are executed. Normally the statements contain an update value for the variable being processed for the next iteration.
•	When the condition becomes false, the loop terminates which marks the end of its life cycle.
for loop: for loop provides a concise way of writing the loop structure. Unlike a while loop, a for statement consumes the initialization, condition, and increment/decrement in one line thereby providing a shorter, easy-to-debug structure of looping. Syntax:
for (initialization condition; testing condition; 
                              increment/decrement)
{
    statement(s)
}
1.	Initialization condition: Here, we initialize the variable in use. It marks the start of a for loop. An already declared variable can be used or a variable can be declared, local to loop only.
2.	Testing Condition: It is used for testing the exit condition for a loop. It must return a boolean value. It is also an Entry Control Loop as the condition is checked prior to the execution of the loop statements.
3.	Statement execution: Once the condition is evaluated to be true, the statements in the loop body are executed.
4.	Increment/ Decrement: It is used for updating the variable for the next iteration.
5.	Loop termination: When the condition becomes false, the loop terminates marking the end of its life cycle.
do-while: The do-while loop is similar to the while loop with the only difference that it checks for the condition after executing the statements, and therefore is an example of an Exit Control Loop. 
Syntax:
do
{
    statements..
}
while (condition);
1.	The do-while loop starts with the execution of the statement(s). There is no checking of any condition for the first time.
2.	After the execution of the statements, and update of the variable value, the condition is checked for a true or false value. If it is evaluated to be true, the next iteration of the loop starts.
3.	When the condition becomes false, the loop terminates which marks the end of its life cycle.
4.	It is important to note that the do-while loop will execute its statements at least once before any condition is checked, and therefore is an example of the exit control loop.
Infinite loop: One of the most common mistakes while implementing any sort of looping is that it may not ever exit, that is the loop runs for infinite times. This happens when the condition fails for some reason. 
Example: 
•	JavaScript
// JavaScript program to illustrate infinite loop
 
    // infinite loop because condition is not apt
    // condition should have been i>0.
    for (var i = 5; i != 0; i -= 2)
    {
        document.write(i);
    }
     
    var x = 5;
 
    // infinite loop because update statement
    // is not provided.
    while (x == 5)
    {
        document.write("In the loop");
    }
 
Here are some more loops used in Javascript these days:
For-in: For-in loop in JavaScript is used to iterate over the properties of an object. The for-in loop iterates only over those keys of an object which have their enumerable property set to “true”.
JavaScript - Functions
A function is a group of reusable code which can be called anywhere in your program. This eliminates the need of writing the same code again and again. It helps programmers in writing modular codes. Functions allow a programmer to divide a big program into a number of small and manageable functions.
Like any other advanced programming language, JavaScript also supports all the features necessary to write modular code using functions. You must have seen functions like alert() and write() in the earlier chapters. We were using these functions again and again, but they had been written in core JavaScript only once.
JavaScript allows us to write our own functions as well. This section explains how to write your own functions in JavaScript.
Function Definition
Before we use a function, we need to define it. The most common way to define a function in JavaScript is by using the function keyword, followed by a unique function name, a list of parameters (that might be empty), and a statement block surrounded by curly braces.
Syntax
The basic syntax is shown here.
<script type = "text/javascript">
   <!--
      function functionname(parameter-list) {
         statements
      }
   //-->
</script>
Example
Try the following example. It defines a function called sayHello that takes no parameters −
<script type = "text/javascript">
   <!--
      function sayHello() {
         alert("Hello there");
      }
   //-->
</script>
Calling a Function
To invoke a function somewhere later in the script, you would simply need to write the name of that function as shown in the following code.
 Live Demo
<html>
   <head>   
      <script type = "text/javascript">
         function sayHello() {
            document.write ("Hello there!");
         }
      </script>
      
   </head>
   
   <body>
      <p>Click the following button to call the function</p>      
      <form>
         <input type = "button" onclick = "sayHello()" value = "Say Hello">
      </form>      
      <p>Use different text in write method and then try...</p>
   </body>
</html>
Function Parameters
Till now, we have seen functions without parameters. But there is a facility to pass different parameters while calling a function. These passed parameters can be captured inside the function and any manipulation can be done over those parameters. A function can take multiple parameters separated by comma.
Example
Try the following example. We have modified our sayHello function here. Now it takes two parameters.
 Live Demo
<html>
   <head>   
      <script type = "text/javascript">
         function sayHello(name, age) {
            document.write (name + " is " + age + " years old.");
         }
      </script>      
   </head>
   
   <body>
      <p>Click the following button to call the function</p>      
      <form>
         <input type = "button" onclick = "sayHello('Zara', 7)" value = "Say Hello">
      </form>      
      <p>Use different parameters inside the function and then try...</p>
   </body>
</html>
Output
The return Statement
A JavaScript function can have an optional return statement. This is required if you want to return a value from a function. This statement should be the last statement in a function.
For example, you can pass two numbers in a function and then you can expect the function to return their multiplication in your calling program.
Example
Try the following example. It defines a function that takes two parameters and concatenates them before returning the resultant in the calling program.
 Live Demo
<html>
   <head>  
      <script type = "text/javascript">
         function concatenate(first, last) {
            var full;
            full = first + last;
            return full;
         }
         function secondFunction() {
            var result;
            result = concatenate('Zara', 'Ali');
            document.write (result );
         }
      </script>      
   </head>
   
   <body>
      <p>Click the following button to call the function</p>      
      <form>
         <input type = "button" onclick = "secondFunction()" value = "Call Function">
      </form>      
      <p>Use different parameters inside the function and then try...</p>  
  </body>
</html>
JavaScript - Events
What is an Event ?
JavaScript's interaction with HTML is handled through events that occur when the user or the browser manipulates a page.
When the page loads, it is called an event. When the user clicks a button, that click too is an event. Other examples include events like pressing any key, closing a window, resizing a window, etc.
Developers can use these events to execute JavaScript coded responses, which cause buttons to close windows, messages to be displayed to users, data to be validated, and virtually any other type of response imaginable.
Events are a part of the Document Object Model (DOM) Level 3 and every HTML element contains a set of events which can trigger JavaScript Code.
Please go through this small tutorial for a better understanding HTML Event Reference. Here we will see a few examples to understand a relation between Event and JavaScript −
onclick Event Type
This is the most frequently used event type which occurs when a user clicks the left button of his mouse. You can put your validation, warning etc., against this event type.
Example
Try the following example.
 Live Demo
<html>
   <head>   
      <script type = "text/javascript">
         <!--
            function sayHello() {
               alert("Hello World")
            }
         //-->
      </script>      
   </head>
   
   <body>
      <p>Click the following button and see result</p>      
      <form>
         <input type = "button" onclick = "sayHello()" value = "Say Hello" />
      </form>      
   </body>
</html>
Output
onsubmit Event Type
onsubmit is an event that occurs when you try to submit a form. You can put your form validation against this event type.
Example
The following example shows how to use onsubmit. Here we are calling a validate() function before submitting a form data to the webserver. If validate() function returns true, the form will be submitted, otherwise it will not submit the data.
Try the following example.
<html>
   <head>   
      <script type = "text/javascript">
         <!--
            function validation() {
               all validation goes here
               .........
               return either true or false
            }
         //-->
      </script>      
   </head>
   
   <body>   
      <form method = "POST" action = "t.cgi" onsubmit = "return validate()">
         .......
         <input type = "submit" value = "Submit" />
      </form>      
   </body>
</html>
onmouseover and onmouseout
These two event types will help you create nice effects with images or even with text as well. The onmouseover event triggers when you bring your mouse over any element and the onmouseout triggers when you move your mouse out from that element. Try the following example.
 Live Demo
<html>
   <head>   
      <script type = "text/javascript">
         <!--
            function over() {
               document.write ("Mouse Over");
            }            
            function out() {
               document.write ("Mouse Out");
            }            
         //-->
      </script>      
   </head>
   
   <body>
      <p>Bring your mouse inside the division to see the result:</p>      
      <div onmouseover = "over()" onmouseout = "out()">
         <h2> This is inside the division </h2>
      </div>         
   </body>
</html>


