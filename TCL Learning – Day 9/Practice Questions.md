# 💻 TCL Programming Exercises

### 1. Split `"name:age:gender"` into a list using `:` as the delimiter.
```tcl
set data {name:age:gender}
puts "[split $data :]"
```

### 2. Join `{EDA VLSI TCL}` using `-` as a separator.
```tcl
set d {EDA VLSI TCL}
puts "[join $d -]"
```

### 3. Check if the word `"script"` matches the pattern `"scrip*"` using `string match`.
```tcl
set s script
puts "[string match "scri*" $s]"
```

### 4. Extract the number from `"Marks: 87/100"` using `regexp`.
```tcl
set num "Marks: 87/100"
regexp {\d+} $num nums
puts "$nums"
```

### 5. Replace `"error"` with `"warning"` in `"Syntax error at line 4"`.
```tcl
set str "Syntax error at line 4"
regsub "error" $str "warning" new
puts "$new"
```

### 6. Use `split` on `"one two three"` and print the second word.
```tcl
set num {one two three}
set num1 [split $num " "]
puts "[lindex $num1 1]"
```

### 7. Use `regexp` to check if the string `"TCL123"` contains a number.
```tcl
set str1 "TCL123"
if { [regexp {\d+} $str1] } {
  puts "Yes"
} else {
  puts "No"
}
```

### 8. Replace only the first occurrence of `"hello"` with `"hi"` in `"hello world, hello again"`.
```tcl
set str2 "hello world, hello again"
regsub "hello" $str2 "hi" newstr2
puts "$newstr2"
```


