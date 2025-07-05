# 💻 TCL Programming Exercises

### 1. Create a list of three colors and print it.
```tcl
set colours { orange yellow blue }
puts "$colours"
```

### 2. Get the number of elements in `{10 20 30 40}`.
```tcl
set num { 10 20 30 40 }
puts "[llength $num]"
```

### 3. Access and print the second element from the list `{math physics chemistry}`.
```tcl
set sub {math physics chemistry}
puts "[lindex $sub 1]"
```

### 4. Create a list `{A B C D}` and print the first two elements using `lrange`.
```tcl
set alp { A B C D}
puts "[lrange $alp 0 1]"
```

### 5. Append `"green"` and `"blue"` to an existing list `{red yellow}`.
```tcl
set clr {red yellow}
lappend clr green blue
puts "$clr"
```

### 6. Insert `"orange"` between `"red"` and `"yellow"` in the list `{red yellow}`.
```tcl
set clr {red yellow}
set clr [linsert $clr 1 orange]
puts "$clr"
```

### 7. Replace `"physics"` with `"biology"` in `{math physics chemistry}`.
```tcl
set sub {math physics chemistry}
puts "[lreplace $sub 1 1 bio]"
```

### 8. Search for `"dog"` in `{cat dog bird}` and print the index.
```tcl
set src {cat dog bird}
puts "[lsearch $src dog]"
```

### 9. Sort the list `{45 12 89 33}` and print the result.
```tcl
set unsrt {45 12 89 33}
puts "[lsort $unsrt]"
```

### 10. Sort `{zebra apple mango}` in ascending order.
```tcl
set asc {zebra apple mango}
puts "[lsort $asc]"
```

### 11. Check if `"math"` exists in `{math physics}` using `lsearch`.
```tcl
set sub {math physics chemistry}
puts "[lsearch $sub math]"
```

### 12. Write a procedure to return the last item of any list.
```tcl
set alp { A B C D}
set sub {math physics chemistry}
puts "[lindex $alp end]"
puts "[lindex $sub end]"
```

### 13. Insert multiple elements `{E F}` at index 2 in `{A B C D}`.
```tcl
set alp { A B C D}
set alp [linsert $alp 2 E F]
puts "$alp"
```

### 14. Replace elements at index 1 to 3 in `{1 2 3 4 5}` with `"X"`.
```tcl
set num1 {1 2 3 4 5}
puts "[lreplace $num1 1 3 X]"
```

### 15. Combine two lists `{1 2}` and `{a b}` into one flat list.
```tcl
set lst1 { 1 2 }
set lst2 { a b }
puts "[concat $lst1 $lst2]"
```
