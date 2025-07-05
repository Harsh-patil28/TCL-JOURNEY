## Example 1: Creating and Printing a List
```tcl
set fruits [list apple banana mango]
puts "$fruits"
```

## Example 2: Getting the Length of a List
```tcl
puts [llength $fruits]  ;# Output: 3
```

##  Example 3: Accessing List Elements
```tcl
puts [lindex $fruits 1] ;# Output: banana
```

## Example 4: Extracting a Sublist
```tcl
puts [lrange $fruits 0 1] ;# Output: apple banana
```

## Example 5: Appending Elements to a List
```tcl
lappend fruits papaya
puts $fruits ;# Output: apple banana mango papaya
```

## Example 6: Inserting into a List
```tcl
set numbers {1 2 4 5}
set updated [linsert $numbers 2 3]
puts $updated ;# Output: 1 2 3 4 5
```

## Example 7: Replacing Elements in a List
```tcl
set items {pen pencil marker}
set newlist [lreplace $items 1 2 eraser]
puts $newlist ;# Output: pen eraser
```

## Example 8: Searching in a List
```tcl
set tools {hammer wrench pliers}
puts [lsearch $tools wrench] ;# Output: 1
```

## Example 9: Sorting a List
```tcl
set unsorted {5 1 9 3}
puts [lsort $unsorted] ;# Output: 1 3 5 9
```

## Example 10: Splitting a String into a List
```tcl
set items [split "a,b,c" ","]
puts "$items"   ;# Output: a b c
```

## Example 11: Joining List Elements into a String
```tcl
set colors {red green blue}
set result [join $colors ","]
puts "$result"   ;# Output: red,green,blue
```

## Example 12: Merging Two Lists into One Flat List
```tcl
set list1 {1 2}
set list2 {a b}
set combined [concat $list1 $list2]
puts "$combined"   ;# Output: 1 2 a b
```

## Example 13: Getting the Last Element of a List
```tcl
set alp { A B C D}
puts "[lindex $alp end]"
```

