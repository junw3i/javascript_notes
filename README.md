# javascript_notes

### Understanding Scope

**LHS** 

*look-up is done when a variable appears on the left-hand side of an assignment operation*

If the Engine is performing an LHS look-up and arrives at the top floor (global Scope) without finding it, and if the program is not running in "Strict Mode" [^note-strictmode], then the global Scope will create a new variable of that name in the global scope, and hand it back to Engine.

**RHS** 

*means "go get the value of..."*

If an RHS look-up fails to ever find a variable, anywhere in the nested Scopes, this results in a `ReferenceError` being thrown by the Engine. It's important to note that the error is of the type `ReferenceError`.


Avoiding using `eval(..)` and `with`

https://github.com/getify/You-Dont-Know-JS/blob/master/scope%20%26%20closures/ch3.md
