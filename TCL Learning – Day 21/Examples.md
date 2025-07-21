## Example 1: Creating and printing a list
```tcl
set myList [list "apple" "banana" "cherry"]
puts $myList
```

## Example 2: Accessing an element with lindex
```tcl
set item [lindex $myList 1]
puts "Second item is: $item"
```

## Example 3: Iterating with foreach
```tcl
foreach fruit $myList {
    puts "Fruit: $fruit"
}
```

## Example 4: Adding elements using lappend
```tcl
lappend myList "date"
puts $myList
```

## Example 5: Replacing a value with lset
```tcl
lset myList 0 "apricot"
puts $myList
```

## Example 6: Inserting at a specific position
```tcl
set newList [linsert $myList 1 "blueberry"]
puts $newList
```

## Example 7: Sorting and searching
```tcl
set sortedList [lsort $myList]
puts "Sorted list: $sortedList"

set index [lsearch $myList "banana"]
puts "Index of banana: $index"
```
