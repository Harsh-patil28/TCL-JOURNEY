## Example 1: Procedure Without Arguments
```tcl
proc sayHello {} {
    puts "Hello from TCL!"
}
sayHello
```

## Example 2: Procedure with Arguments
```tcl
proc add {a b} {
    set sum [expr $a + $b]
    return $sum
}
puts "Sum: [add 5 10]"
```

## Example 3: Procedure to Check Even or Odd
```tcl
proc checkEvenOdd {num} {
    if {[expr $num % 2] == 0} {
        return "Even"
    } else {
        return "Odd"
    }
}
puts [checkEvenOdd 7]
```

## Example 4: Procedure to Find Maximum of Two Numbers
```tcl
proc findMax {a b} {
    if {$a > $b} {
        return $a
    } else {
        return $b
    }
}
puts "Max: [findMax 12 9]"
```

## Example 5: Procedure Returning a List
```tcl
proc makeList {x y} {
    return [list $x $y]
}
puts [makeList "EDA" "TCL"]
```
