# 📘 TCL Learning – Day 6

Topic: Procedures and Return Values in TCL

Date: July 6, 2025

# 🔹 What is a Procedure?
In TCL, a procedure (also called a proc) is a reusable block of code defined once and called multiple times. It promotes code modularity and readability.

# 🔹 Why Use Procedures?
Avoid code repetition

Encapsulate logic

Make code reusable and maintainable

# 🔹 Syntax of a Procedure
```tcl
proc procedureName {arg1 arg2 ...} {
    # code block
    return $result
}
```
proc defines the procedure.

{arg1 arg2 ...} is the list of input arguments.

Code inside the body gets executed when the procedure is called.

return is used to send back a result.
