# 💻 TCL Programming Exercises

### 1. Declare two variables `x = 12`, `y = 8` and print their sum.

```tcl
set x 12
set y 8
puts "[expr $x + $y]"
```

---

### 2. Calculate the remainder of `23 ÷ 5` and print it.

```tcl
puts "[expr 23 % 5]"
```

---

### 3. Find the square of `x` using the exponentiation operator.

```tcl
puts "[expr $x ** 2]"
```

---

### 4. Assign the value `45` to variable `num1` and increment it by `10`.

```tcl
set num1 45
puts "[expr $num1 + 10]"
```

---

### 5. Assign a floating-point number to a variable and multiply it by `2`.

```tcl
set flt 2.3
puts "[expr $flt * 2]"
```

---

### 6. Evaluate this expression and store the result: `(4 + 6) * 3`

```tcl
set res [expr (4 + 6) * 3]
puts "$res"
```

---

### 7. Calculate and print the average of three values: `12`, `18`, and `30`.

```tcl
puts "[expr (12 + 18 + 30) / 3]"
```

---

### 8. Assign a string `"VLSI"` to variable `tech` and print its length.

```tcl
set tech VLSI
puts "[string length $tech]"
```

---

### 9. Concatenate `"System"` and `"Verilog"` with a space in between.

```tcl
set s SYSTEM
set v VERILOG
puts "$s $v"
```

---

### 10. Compare the strings `"TCL"` and `"tcl"` using `string compare`.

```tcl
puts "[string compare TCL tcl]"
```

---

### 11. Convert `"HELLO TCL"` to lowercase and print it.

```tcl
puts "[string tolower "HELLO TCL"]"
```

---

### 12. Check if `"script"` contains `"rip"` using `string first`.

```tcl
puts "[string first rip script]"
```

---

### 13. Replace `"123"` with `"XYZ"` in `"abc123"` using `string replace`.

```tcl
puts "[string replace "abc123" 3 5 "XYZ"]"
```

---

### 14. Extract the first 4 characters from `"ScriptingLanguage"`.

```tcl
puts "[string range "ScriptingLanguage" 0 3]"
```

---

### 15. Print `"even"` if a number is divisible by `2`, else print `"odd"`.

```tcl
if {[expr $x % 2] == 0} {
    puts "even"
} else {
    puts "odd"
}
```
