# 📘 TCL Learning – Day 10

Topic: Loop Control Statements & Error Handling in TCL

Date: July 10, 2025

# 🔹 Loop Control Keywords

| Keyword  | Use Case                                          |
|----------|---------------------------------------------------|
| `break`  | Immediately exits the innermost loop              |
| `continue` | Skips the current iteration and moves to the next |
| `return` | Exits a procedure and optionally returns a value  |


# 🔸 break and continue
```tcl
for {set i 1} {$i <= 10} {incr i} {
    if {$i == 5} {
        break
    }
    puts $i
}
```
```tcl
for {set i 1} {$i <= 5} {incr i} {
    if {$i == 3} {
        continue
    }
    puts $i
}
```


# 🔹 Error Handling Keywords

| Command | Description                                                |
|---------|------------------------------------------------------------|
| `catch` | Catches an error and prevents it from crashing the script |
| `error` | Generates a user-defined error message                    |


# 🔸 error Syntax
```tcl
error "Invalid input provided"
```

# 🔸 catch Syntax
```tcl
if {[catch {expr 10 / 0} result]} {
    puts "Error caught: $result"
} else {
    puts "Result: $result"
}
```

# 🔸 return in Procedure
```tcl
proc double {x} {
    return [expr {$x * 2}]
}
puts [double 6]  ;# Output: 12
```




