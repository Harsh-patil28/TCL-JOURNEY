# 💻 TCL Programming Exercises

### 1. Creates a list components = {mux alu reg file}
```tcl
set components {mux alu reg file}
```

### 2. Adds a new item "decoder" using lappend
```tcl
lappend components decoder 
```

### 3. Sorts the list and prints the sorted result
```tcl
puts "[lsort $components]"
```

### 4. Replaces the second item with "adder"
```tcl
set new_comp "[lreplace [lsort $components]  1 1 adder]"
puts "$new_comp"
```

### 5. Loops through and prints each component with its index
```tcl
set idx 0
foreach i $new_comp {
    puts "$idx - $i"
    incr idx
}
```
### 6. Extracts and prints only the first three elements
```tcl
set final "[lrange $new_comp 0 2]"
puts "$final"
```

### 7. Checks the length of the final list
```tcl
puts "[llength $final]"
```
