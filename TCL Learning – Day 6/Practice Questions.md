# 💻 TCL Programming Exercises

### 1. Create a procedure `greet` that prints "Welcome to TCL Scripting".
```tcl
proc greet {} {
  puts "Welcome to TCl"
}
greet 
```

### 2. Define a procedure `multiply` that takes two inputs and returns their product.
```tcl
proc multiply { a b} {
  set pro [expr $a * $b]
  return $pro
}
puts "[multiply 10 2]"
```

### 3. Create a procedure `isPositive` that returns "Positive", "Negative", or "Zero" based on the input.
```tcl
proc ispositive {num} {
  if {$num > 0} {
    return "Positive"
  } elseif { $num < 0} {
    return "Negative" 
  } else {
    return "Zero"
  }
}
puts "[ispositive -9]"
```

### 4. Write a procedure to return the square of a number.
```tcl
proc sq {num1} {
  return "[expr $num1 ** 2]"
  
}
puts "[sq 6]"
```

### 5. Create a procedure `power` that takes base and exponent and returns the result.
```tcl
proc exp {base pwr} {
  return "[expr $base ** $pwr]"
}
puts "[exp 2 10]"
```

### 6. Write a procedure that takes a name and prints "Hello, <name>!".
```tcl
proc name {nm} {
  puts "Hello $nm"
}
puts "[name "Engineering Enigma"]"
```

### 7. Write a procedure to return the factorial of a number.
```tcl
proc fact {num2} {
  set r 1
  for {set i $num2} { $i > 0 } { incr i -1} {
    set r [expr $r * $i]
  }
  return $r
}
puts "[fact 5]"
```

### 8. Write a procedure that takes a list and returns its length.
```tcl
proc lst { list } {
  return "[llength $list]"
}
puts "[lst {a b c d}]"
```
### 9. Write a procedure that takes a string and returns it reversed.
```tcl
proc rev { list1 } {
  return "[join [lreverse [split $list1 " "]]]"
}
puts "[rev Hello]"
```

### 10. Create a procedure `countVowels` to count vowels in a given string.
```tcl
proc countVowels {str} {
    return [llength [regexp -all -inline {[aeiouAEIOU]} $str]]
}
puts "[countVowels {Hi Im Engineer}]"
```

### 11. Write a procedure to remove duplicates from a list.
```tcl
proc removeDuplicates {inputList} {
    set seen {}
    set result {}

    foreach item $inputList {
        if {[lsearch -exact $seen $item] == -1} {
            lappend seen $item
            lappend result $item
        }
    }
    return $result
}
puts "[removeDuplicates {a b c d abcd a a bcd}]"
```
