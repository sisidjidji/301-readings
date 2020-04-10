# READ10

- A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.

- The JavaScript engine (which is found in a hosting environment like the browser), is a single-threaded interpreter comprising of a heap and a single call stack. The browser provides web APIs like the DOM, AJAX, and Timers.

- The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

- When the code is run, we get an error. A stack is printed showing how the functions are stack on top each other.

- The first thing that indicates you that something is wrong with your code is the (in)famous error message that the one we saw just moments ago, it usually appears on your console (being developer tools of the browser, terminal or whatever else you are using).

- Whatever you are using (var, let or const) the fix is as simple has declaring the variable before any declaration is made.

- Some syntax errors like sending a trailing comma when calling a function are handled without error by most recent browsers, but older ones you have to be careful.