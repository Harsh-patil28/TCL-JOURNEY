## Example 1: for Loop for Counting 1 to 5
```tcl
for {set i 1} {$i <= 5} {incr i} {
    puts "Count: $i"
}
```

## Example 2: while Loop to Print Even Numbers Less Than 10
```tcl
set i 0
while {$i < 10} {
    puts "Even: $i"
    incr i 2
}
```

## Example 3: foreach Loop Over a List of Strings
```tcl
foreach name {TCL Verilog Python VHDL} {
    puts "Language: $name"
}
```

## Example 4: Nested for Loops for Multiplication Table (2 to 3)
```tcl
for {set i 2} {$i <= 3} {incr i} {
    for {set j 1} {$j <= 10} {incr j} {
        puts "$i x $j = [expr $i * $j]"
    }
}
```

## Example 5: Iterating with Two Lists Using foreach
```tcl
foreach {a b} {10 20 30 40 50 60} {
    puts "Pair: $a and $b"
}
```
