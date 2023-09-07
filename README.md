# hoisting
Hoisting is a concept in JavaScript where variable and function declarations are moved to the top of their containing scope during the compilation phase. This means that, while the actual code appears to have variable and function declarations in a specific order, JavaScript interpreters will treat them as if they were declared at the top of their containing scope. Hoisting applies only to declarations, not initializations or assignments.
Here's a step-by-step explanation of each line and the thought process behind it:

    sayHello();:
        This line is attempting to call the sayHello function before it's actually declared in the code.
        The reason this works is due to hoisting. During the compilation phase, the JavaScript engine recognizes that there is a sayHello function declaration in the code, and it "hoists" this declaration to the top of the current scope.
        So, when this line is executed, the sayHello function is already declared (even though it appears later in the code), and it can be called without any errors.

    function sayHello() { ... }:
        This line is where the sayHello function is defined.
        Despite its position in the code, the JavaScript engine treats it as if it were declared at the top of the current scope.
        When the code execution reaches this point, it assigns the function definition to the sayHello identifier, allowing it to be called or used later in the code.
In summary, hoisting is a JavaScript behavior where function declarations (not expressions) are "lifted" to the top of their containing scope during the compilation phase. This allows you to call functions before they appear in the code, but it's important to note that this behavior applies to function declarations, not variable declarations or initializations. For clarity and best coding practices, it's recommended to declare your variables and functions at the top of their respective scopes.
