# 💻 TCL Programming Exercises

### 1. Check if a number is even or odd.
```tcl
set x 35; set y 50;
if {[expr $x % 2]==0} {
  puts "even"
} else {
  puts "odd"
}
```

### 2. Determine if a number is positive, negative, or zero.
```tcl
set x 35; set y 50; set z -4; set a 0;
if { $z > 0 } {
  puts "positive"
} elseif { $z < 0 } {
  puts "negative"
} else {
  puts "zero"
}
```

### 3. Take two numbers x = 35, y = 50. Print which one is greater.
```tcl
set x 35; set y 50;
if { $x > $y } {
  puts "$x is greater then $y"
} else {
  puts "$y is greater then $x"
}
```

### 4. Check if a number is divisible by both 2 and 3.
```tcl
set num1 6
if { [expr $num1 % 2] == 0 && [expr $num1 % 3] == 0 } {
puts "Divisible" 
} else {
  puts "Not Divisible"
}
```

### 5. Assign a temperature value and print:
- "Cold" if less than 20  
- "Moderate" if between 20–30  
- "Hot" otherwise
```tcl
set temp 25
if { $temp < 20 } {
  puts "Cold"
} elseif { 20 <= $temp && $temp < 30 } {
  puts "Moderate"
} else {
  puts "High"
}
```

### 6. Create a variable user_role. If it’s "admin", print "Full Access"; if "guest", print "Read Only"; else print "Unknown Role".
```tcl
set user_role guest
if { $user_role == "admin" } {
  puts "Full Access"
} elseif { $user_role == "guest" } {
  puts "Read-Only"
} else {
  puts "Unknown User"
}
```

### 7. Use logical OR to check if a number is less than 10 or greater than 100.
```tcl
set num2 600
if { $num2 > 100 || $num2 < 10 } {
  puts "Greater then 100 or less then 10"
} else { 
puts "In between"
}
```

### 8. Use `if` to compare two strings "EDA" and "eda". Print "Match" if equal, else "Not Match".
```tcl
if { [string compare "EDA" "eda"] } {
  puts "Not Match"
} else {
  puts "Match"
}
```

### 9. Evaluate if a number lies between 10 and 20 (inclusive).
```tcl
set num3 20
if { $num3 <=20 && $num3 >= 10} {
  puts "In between"
} else {
  puts "Not"
}
```

### 10. Write a condition to check if a string contains the word "test".
```tcl
set str testmatch
if { [string match "*test*" $str] } {
  puts "Yes"
} else {
  puts "No"
}
```

### 11. Check if a string starts with "T" using `string index`.
```tcl
set str2 Tempus
if { [string index $str2 0] eq "T"} {
puts "Yes" 
} else {
puts "No" }
```

### 12. Compare lengths of two strings and print which one is longer.
```tcl
if {[string length $str] > [string length $str2] } {
  puts "Lenght of String 1 is larger"
} else {
  puts "Length of String 2 is larger"
}
```
