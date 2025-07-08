## Example 1: Basic List and Array Creation
```tcl
set colors {red green blue}
array set codes {R 1 G 2 B 3}
```

## Example 2: Accessing List and Array Elements
```tcl
puts [lindex $colors 0]         ;# Output: red
puts $codes(G)                  ;# Output: 2
```

## Example 3: Iterating Through a List
```tcl
foreach color $colors {
    puts "Color: $color"
}
```

## Example 4: Iterating Through an Array
```tcl
foreach key [array names codes] {
    puts "$key => $codes($key)"
}
```

## Example 5: Array Size and Existence Check
```tcl
puts "Size: [array size codes]"
if {[info exists codes(R)]} {
    puts "Key R exists"
}
```

