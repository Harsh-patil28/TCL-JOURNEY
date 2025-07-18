## Example 1: Basic Procedure with Parameters
```tcl
proc greet {name} {
    puts "Hello, $name!"
}
greet "Harsh"
```

## Example 2: Procedure with Return Value
```tcl
proc square {x} {
    return [expr {$x * $x}]
}
puts "Square: [square 5]"
```

## Example 3: Default Arguments (Manual Handling)
```tcl
proc welcome {name {greeting "Hi"}} {
    puts "$greeting, $name!"
}
welcome "Engineering Enigma"
welcome "Engineering Enigma" "Welcome"
```

## Example 4: Using args for Variable Arguments
```tcl
proc printAll args {
    foreach val $args {
        puts $val
    }
}
printAll "Apple" "Banana" "Cherry"
```

## Example 5: Returning Status with catch
```tcl
proc divide {a b} {
    if {$b == 0} {
        return "Error: Division by zero"
    }
    return [expr {$a / $b}]
}
puts [divide 10 0]
puts [divide 10 2]
```

## Example 6: Using catch to Handle Procedure Errors
```tcl
proc riskyOp {x} {
    return [expr {10 / $x}]
}

if {[catch {riskyOp 0} result]} {
    puts "Caught error: $result"
} else {
    puts "Result: $result"
}
```

