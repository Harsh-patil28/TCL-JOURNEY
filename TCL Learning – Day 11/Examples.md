## Example 1: Sorting Array Keys Alphabetically
```tcl
array set animals {zebra 1 ant 2 lion 3}
foreach key [lsort [array names animals]] {
    puts "$key => $animals($key)"
}
```

## Example 2: Pattern Matching in Keys
```tcl
array set data {val1 100 val2 200 temp 300}
foreach key [array names data val*] {
    puts "$key => $data($key)"
}
```

## Example 3: Using regexp to Filter Values
```tcl
array set studentGrades {A1 80 A2 92 B1 60 B2 55}
foreach key [array names studentGrades] {
    if {[regexp {^A} $key]} {
        puts "$key is from group A"
    }
}
```

##  Example 4: Conditional Filtering with if
```tcl
foreach key [array names studentGrades] {
    if {$studentGrades($key) >= 75} {
        puts "$key Passed"
    }
}
```

## Example 5: Key Existence Check
```tcl
if {[info exists studentGrades(B1)]} {
    puts "B1 exists"
}
```
