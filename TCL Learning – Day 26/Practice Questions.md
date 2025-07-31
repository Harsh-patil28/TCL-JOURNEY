# 💻 TCL Programming Exercises

### 1. Takes a string variable course = "RTL2GDS Flow 101".
```tcl
set course  "RTL2GDS Flow 101"
```

### 2. Converts it to uppercase and prints it.
```tcl
puts "[string toupper $course]"
```

### 3. Finds if it contains any digits using regex.
```tcl
if { [regexp  {\d+} $course]} {
  puts "contains digit"
}
```

### 4. Replaces all digits with underscores (_).
```tcl
puts "[regsub -all {\d}  $course _ ]"
```

### 5. Matches if the string starts with "RTL*" using string match.
```tcl
if { [string match "RTL*" $course]} {
  puts "String Match"
}
```

### 6. Extracts substring from 0 to 6.
```tcl
puts "[string range $course 0 6]"
```

### 7. Counts the number of characters.
```tcl
puts "[string length $course]"
```

### 8. If the string has “Flow” in it, print "Design Flow Detected".
```tcl
if {[string match "*Flow*" $course]} {
  puts "Design Flow Detected"
}
```
