# 💻 TCL Programming Exercises

### 1. Insert "orange" between "apple" and "banana" in list {apple banana cherry}.
```tcl
set fruit {apple banana cherry}
puts "$fruit"
set new [linsert $fruit 1 orange]
puts "$new"
```

### 2. Replace all occurrences of "bad" with "good" in a list of comments.
```tcl
set comments {
    "bad code"
    "not a bad idea"
    "bad day"
}
foreach c $comments { puts [string map {"bad" "good"} $c] }
```

### 3. Write a proc uniqueSort {list} that removes duplicates and returns sorted list.
```tcl
proc uniqueSort {list} {
    return [lsort -unique $list]
}
set mylist {3 5 1 2 3 2 4 1}
puts [uniqueSort $mylist]
```

### 4. Write a proc removeItem {list item} that deletes all occurrences of item.
```tcl
proc removeItem {list item} {
    return [lsearch -all -inline -not $list $item]
}
set mylist {a b c a d}
puts [removeItem $mylist a]
```

### 5. Given {10 5 20 1}, return the 2nd largest number.
```tcl
set numbers {10 5 20 1}
set sorted [lsort -integer -decreasing $numbers]
set secondLargest [lindex $sorted 1]
puts $secondLargest
```
