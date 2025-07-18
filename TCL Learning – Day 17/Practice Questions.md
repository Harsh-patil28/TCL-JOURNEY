# 💻 TCL Programming Exercises

### 1. `factorial {n}` – Recursively compute factorial of a number.
```tcl
proc factorial {n} {
set res 1
  for {set i 1} {$i <= $n} {incr i} {
   set res [expr $res * $i]
  }
  return $res
}
puts "[factorial 5]"
```

### 2. `reverseString {str}` – Return the reversed version of the string.
```tcl
proc reverseString {str} {
  return [join [lreverse [split $str ""]] ""]
}
puts "[reverseString Hello]"
```

### 3. `fibonacci {n}` – Return nth Fibonacci number.
```tcl
proc fibonacci {n} {
    set a 0
    set b 1
    for {set i 0} {$i < $n} {incr i} {
        set b [expr {$a + $b}]
        set a [expr {$b - $a}]
    }
    return $a
}
puts "[fibonacci 6]"
```

### 4. `showArgs` – Create a procedure that prints all received arguments using args.
```tcl
proc showArgs {args} {
    puts "Arguments received:"
    foreach arg $args {
        puts $arg
    }
}
puts "[showArgs apple watermelon]"
```
