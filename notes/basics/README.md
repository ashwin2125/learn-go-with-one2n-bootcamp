# Tour of Go

Notes:
- Variables declared inside an `if short` statement will also be available in `else` blocks.
- Order of Evaluation in Function Arguments:
    - In Go, function arguments are evaluated before the function is called.
    - Go determines the order of evaluation of function arguments by evaluating them from **left to right** before the function call, as specified in the language specification.
    - In languages like C, C++, Java there is no definite specification that mentions on the order of evaluation of function arguments.
    - In Python, the order of evaluation of function arguments is similar to Go.
- In `switch` statement, Go runs only the first successful case and inserts the `break` automatically, unlike C, C++, Java & JS.
- `defer` calls are evaluated immediately but the function call is not executed until the surrounding function returns.
- Deferred function calls are pushed onto a stack. When a function returns, its deferred calls are executed in **last-in-first-out** order.
