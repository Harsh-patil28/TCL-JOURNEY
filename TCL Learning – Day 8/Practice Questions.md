# 💻 TCL Programming Exercises

### Part A: List-Based

### 1. Create a list `{one two three}` and print the second element.
```tcl
set lst { one two three}
puts "[lindex $lst 1]"
```

### 2. Add `"four"` to that list using `lappend`.
```tcl
puts "[lappend lst four]"
```

### 3. Replace `"two"` with `"TWO"` using `lreplace`.
```tcl
puts "[lreplace $lst 1 1 "TWO"]"
```

### 4. Print all list elements whose length is greater than 3.
```tcl
foreach i $lst {
  if { [string length $i] > 3 } {
    puts "$i"
  }
}
```

### 5. Sort a list of numbers `{4 2 9 1}`.
```tcl
set num { 4 2 9 1}
puts "[lsort $num]"
```
---
### Part B: Array-Based

### 6. Create an array `capitals` with the following key-value pairs:
- India: Delhi  
- France: Paris  
- USA: Washington
```tcl
array set capitals {India Delhi France Paris USA Washington}
```

### 7. Access and print the capital of France.
```tcl
puts "$capitals(France)"
```

### 8. Add a new pair `Japan: Tokyo` to the array.
```tcl
set capitals(Japan) Tokyo
```

### 9. Use `array names` to print all countries in the array.
```tcl
foreach i [array names capitals] {
  puts "$i"
}
```

### 10. Use a loop to print `Country - Capital` pairs.
```tcl
foreach i [array names capitals] {
  puts "$i - $capitals($i)"
}
```

### 11. Check if `"USA"` exists as a key and print the capital.
```tcl
if { [info exist capitals(USA)]} {
  puts "$capitals(USA)" 
}
```

### 12. Count and print the number of key-value pairs in the array.
```tcl
puts "[array size capitals]"
```

### 13. Write a procedure `getCapital` that takes a country and returns its capital.
```tcl
proc getCapital { cap } {
 global capitals
  puts "$capitals($cap)"
}
getCapital USA
```

### 14. Write a procedure `printAllKeys` that prints all keys in any array.
```tcl
proc all {key} {
  global capitals
  foreach i [array names capitals] {
    puts "$i"
  }
}
all capitals
```

### 15. Write a procedure `removeKey` that removes a key from an array and returns the updated size.
```tcl

proc removeKey {key} {
    global capitals
   unset capitals($key)
  puts " [array size capitals] "
}
removeKey India
```
