# 🔹 Conditional Statements in Tcl

Use `if`, `if-else`, and logical operators (`&&`, `||`) to control flow based on conditions.

## Example 1: Basic `if` condition
Use `if` to check a condition and execute a block if it's true.

```tcl
set age 18
if {$age >= 18} {
    puts "You are eligible to vote."
}
```

## Example 2: if-else condition
Use if-else to handle both true and false conditions.
```tcl
set temperature 28
if {$temperature > 30} {
    puts "It's hot."
} else {
    puts "It's not hot."
}
```

## Example 3: if-elseif-else ladder
Use this structure to check multiple conditions in sequence.
```tcl
set score 82
if {$score >= 90} {
    puts "Grade A"
} elseif {$score >= 75} {
    puts "Grade B"
} else {
    puts "Grade C"
}
```

## Example 4: Using logical AND (&&)
Logical AND ensures both conditions must be true.

```tcl
set a 10
set b 20
if {$a < 15 && $b > 15} {
    puts "Both conditions are true."
}
```

## Example 5: Using logical OR (||)
Logical OR passes if at least one condition is true.
```tcl
set a 5
if {$a < 3 || $a > 2} {
    puts "At least one condition is true."
}
```
