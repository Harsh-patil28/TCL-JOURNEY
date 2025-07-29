## Example 1: Declare and Assign
Title: Define and assign values to an array
```tcl
set fruits(apple) 10
set fruits(mango) 25
set fruits(banana) 12
```

##  Example 2: Access a Value by Key
Title: Read a value from the array
```tcl
puts "Mango count: $fruits(mango)"
```

## Example 3: Check All Keys
Title: List all array keys
```tcl
puts "Available fruits: [array names fruits]"
```

## Example 4: Iterating Over Array Elements
Title: Iterate and print all key-value pairs
```tcl
foreach key [array names fruits] {
    puts "$key -> $fruits($key)"
}
```

## Example 5: Delete Specific Entry
Title: Remove one key from array
```tcl
unset fruits(banana)
```

## Example 6: Delete Entire Array
Title: Remove the whole array
```tcl
unset fruits
```

## Example 7: Count Total Keys
Title: Determine the number of elements
```tcl
set count 0
foreach key [array names fruits] {
    incr count
}
puts "Total fruits: $count"
```
