# 💻 TCL Programming Exercises

### 1. Declare an array studentMarks with subject names as keys and marks as values.
```tcl
array set  studentMarks { Math 68 Physics 88 Bio 55 Chem 30 }
```

### 2. Access and print the marks in Math and Physics.
```tcl
puts " $studentMarks(Math)"
puts " $studentMarks(Physics)"
```

### 3. Print all subjects the student has.
```tcl
puts "[array names studentMarks]"
```

### 4. Add a new subject Computer with marks.
```tcl
set studentMarks(Computer) 52
```

### 5. Remove the subject Chemistry.
```tcl
unset studentMarks(Chem)
```

### 6. Iterate through the array and print subject:marks.
```tcl
foreach i [array names studentMarks] {
  puts "$i - $studentMarks($i)"
}
```

### 7. Count the number of subjects stored.
```tcl
set count 0 
foreach i [array names studentMarks] {
  incr count
}
puts "$count"
```

### 8. Delete the array.
```tcl
unset studentMarks
```

### 9. Try to access a key after deletion and observe the output.
```tcl

puts "$studentMarks(Computer)"
```
Ouptut 
```tcl
can't read "studentMarks(Computer)": no such variable
    while executing
"puts "$studentMarks(Computer)""
```
