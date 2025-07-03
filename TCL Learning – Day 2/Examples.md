# 🔹 Variables in TCL
 Use `set` to assign values. Variables can store strings, numbers, or lists.
```tcl
set a 10
set b "Hello"
```

# 🔹 Arithmetic Expressions
 Use `expr` to evaluate expressions. Operators: +, -, *, /, %, **
```tcl
set sum [expr $a + 5]
set product [expr $a * 2]
set division [expr $a / 2]
set power [expr $a ** 2]
puts "Sum is: $sum"
puts "Product is: $product"
puts "Division is: $division"
puts "Power is: $power"
```

# 🔹 String Operations
 Concatenation happens automatically in `puts` or using `set`
```tcl
# 🔸 Concatenation
set s1 "Hello"
set s2 "World"
puts "$s1 $s2"
set combined "$s1, $s2!"
puts $combined
```

# 🔸 String Length
```tcl
puts "Length of s1: [string length $s1]"
```

# 🔸 To Lower / Upper
```tcl
puts "Lowercase: [string tolower $s1]"
puts "Uppercase: [string toupper $s2]"
```

# 🔸 Compare Strings
```tcl
puts "Compare s1 and s2: [string compare $s1 $s2]"
```

# 🔸 Equality Check
```tcl
if {[string equal $s1 "Hello"]} {
    puts "s1 is equal to 'Hello'"
}
```

# 🔸 Substring (Range)
```tcl
puts "First 3 letters of s1: [string range $s1 0 2]"
```

# 🔸 Trim Whitespace
```tcl
set padded "   some text   "
puts "Trimmed: '[string trim $padded]'"
```

# 🔸 Replace Text
```tcl
set sentence "I like apples"
puts [string map {apples oranges} $sentence]
```

# 🔸 Search Substring
```tcl
puts "Index of 'l' in s1: [string first "l" $s1]"
```

# 🔸 Last Index of Substring
```tcl
puts "Last index of 'l' in s1: [string last "l" $s1]"
```

# 🔸 String Match (Pattern)
```tcl
if {[string match "H*" $s1]} {
    puts "s1 starts with H"
}
```

# 🔸 String Index
```tcl
puts "Character at index 1 in s1: [string index $s1 1]"
```

# 🔸 String Replace (By Index)
 Replace index 0-1 in "Hello" with "Yo"
 ```tcl
puts [string replace $s1 0 1 "Yo"]
```
