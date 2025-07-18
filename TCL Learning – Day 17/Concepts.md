# 📘 TCL Learning – Day 17

Topic: Procedures in TCL – Parameters, Return, and Error Handling

Date: July 17, 2025

In TCL, procedures (also known as procs) are used to group reusable logic. A procedure can take parameters, return values, and include default arguments. Proper use of procedures leads to more modular and maintainable code.

# 🔹 Syntax: `proc`
```tcl
proc proc_name {param1 param2 ...} {
    # body
    return value
}
```

# 🔹 Key Concepts
| Concept           | Description                                                  |
|-------------------|--------------------------------------------------------------|
| Parameters        | Input variables passed to the procedure                      |
| Default Parameters| Use `args` or assign defaults inside the body                |
| Return Value      | The `return` command exits the proc and passes back a value  |
| Error Handling    | `catch` is used to wrap potentially error-prone code         |
| Recursion         | Procedures can call themselves                               |
