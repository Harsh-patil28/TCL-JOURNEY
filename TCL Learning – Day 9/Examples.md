## Example 1: Splitting a CSV string into a list
```tcl
set csv "red,green,blue"
set colors [split $csv ","]
puts $colors  ;# Output: red green blue
```

## Example 2: Joining list items with delimiter
```tcl
set fruits {apple banana cherry}
set line [join $fruits ","]
puts $line  ;# Output: apple,banana,cherry
```

## Example 3: Using string match with wildcards
```tcl
if {[string match "ver*" "verilog"]} {
    puts "Match found"
}
```

## Example 4: Using regexp to extract digits
```tcl
set line "Total = 1234 units"
regexp {\d+} $line match
puts $match  ;# Output: 1234
```

## Example 5: Using regsub to replace word
```tcl
set text "I love apple pie"
regsub "apple" $text "mango" newtext
puts $newtext  ;# Output: I love mango pie
```
