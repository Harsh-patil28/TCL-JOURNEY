## Example 1: Using switch for decision making
```tcl
set choice "B"

switch $choice {
    "A" {
        puts "Option A selected"
    }
    "B" {
        puts "Option B selected"
    }
    "C" {
        puts "Option C selected"
    }
    default {
        puts "Invalid option"
    }
}
```
### 📝 Note: You can also use -exact, -glob, or -regexp switch modes.

## Example 2: switch with pattern matching
```tcl
set status "error:123"

switch -glob $status {
    "error:*" { puts "An error occurred." }
    "success" { puts "Operation successful." }
    default   { puts "Unknown status." }
}
```

## Example 3: Using break in a loop
```tcl
for {set i 0} {$i < 10} {incr i} {
    if {$i == 5} {
        break
    }
    puts "i = $i"
}
```

## Example 4: Using continue in a loop
```tcl
for {set i 0} {$i < 5} {incr i} {
    if {$i == 2} {
        continue
    }
    puts "i = $i"
}
```

## Example 5: Using return inside a proc (label-like behavior)
```tcl
proc checkValue {x} {
    if {$x < 0} {
        puts "Negative number"
        return
    }
    puts "Positive number"
}

checkValue -5
checkValue 10
```

