# 💻 TCL Programming Exercises

### 1. Print numbers from 10 to 1 using a for loop.
```tcl
for {set i 10} { $i >= 1 } {incr i -1} {
  puts "$i"
}
```

### 2. Use a while loop to print squares of numbers from 1 to 5.
```tcl
set i 0 
while { $i <= 5 } {
  puts "[expr $i * $i]"
  incr i 1
}
```

### 3. Print the first 10 even numbers using for loop.
```tcl
for { set i 1 } { $i <=10 } { incr i } {
  puts "[expr $i * 2]"
}
```

### 4. Iterate through a list {apple orange banana} and print each element.
```tcl
set fruits { apple orange banana}
foreach i $fruits {
  puts "$i"
}
```

### 5. Use foreach to iterate over {1 2 3} and print its square.
```tcl
set sq { 1 2 3 }
foreach i $sq {
  puts "[expr $i * $i]"
}
```

### 6. Write a while loop that keeps doubling a number starting from 1 until it exceeds 100.
```tcl
set i 1 
while { $i <= 100 } {
  puts "$i"
  set i [expr $i * 2]
}
```

### 7. Use foreach with two lists {1 2 3} and {a b c} to print pairs like 1-a, 2-b.
```tcl
set num {1 2 3}
set alp {a b c}
foreach i $num j $alp {
  puts "$i-$j"
}
```

### 8. Use a while loop to calculate factorial of a number n = 5.
```tcl
set n 5
set n1 1
while { $n > 1 } {
set n1 [expr $n1 * $n]
incr n -1
}
puts "$n1"
```

### 9. Create a list of words and print only those with more than 4 characters.
```tcl
set str {abcdefg hello had mad trips}
foreach i $str {
if {[string length $i] > 4} {
  puts "$i"
}
}
```
