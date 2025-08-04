# 💻 TCL Programming Exercises

### 1. Creates a procedure cube that returns the cube of a number.
```tcl
proc cube {num} {
  return "[expr $num ** 3]"
}
puts "[cube 5]"
```

### 2. Creates a procedure is_even that returns "true" if a number is even, else "false".
```tcl
proc iseven {num1} {
  if {$num1 % 2 == 0} {
    return "True"
  } else {
    return "False"
  }
}
puts "[iseven 7]"
```

### 3. Creates a procedure power with 2 arguments (base, exponent) and returns base^exponent.
```tcl
proc power {base exponent} {
  return [expr $base ** $exponent]
}
puts "[power 2 10]"
```

### 4. Creates a procedure greet_user with an optional name argument (default: "guest") and prints a greeting.
#### Explanation:
`{{name "guest"}}`: The double braces allow defining an optional argument with a default value (`"guest"`).
```tcl
proc greet_user {{name "guest"}} {
  return "Hello, $name"
}
puts "[greet_user]"
```

### 5. Creates a global variable calls, and defines a procedure track_calls that increments it every time it's called. Call it 3 times and print calls. 
```tcl
set calls 0 
proc track_calls {} {
  global calls
  incr calls
}
track_calls
track_calls
track_calls
track_calls
track_calls
track_calls
puts "$calls"
```
