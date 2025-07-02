# 💻 TCL Programming Exercises

### 1. Assign the value `25` to a variable named `x`.

```tcl
set x 25
```

---

### 2. Assign 75 to variable `y` and print it.

```tcl
set y 75
puts "$y"
```

---

### 3. Add `x` and `y`, store the result in `z`, and print `z`.

```tcl
set z [expr $x + $y]
puts "$z"
```

---

### 4. Subtract 20 from `z`, update `z`, and print it.

```tcl
set z [expr $z - 20]
puts "$z"
```

---

### 5. Multiply `x` and `y`.

```tcl
puts "[expr $x * $y]"
```

---

### 6. Divide `y` by `x`.

```tcl
puts "[expr $y / $x]"
```

---

### 7. Print a line that says: The result is $result

```tcl
puts "The result is $result"
```

> Note: This will only print a value if `result` is defined earlier.

---

### 8. Try using multiple `set` commands in one line using `;`.

```tcl
set a 10; set b 20;
puts "$a $b"
```

---

### 9. What happens when you do: `set a [expr 3 + 5]`?

```tcl
set a [expr 3 + 5]
puts "$a"
```

> This sets variable `a` to the result of the expression, which is `8`.

---

### 10. Use `#` to add a comment explaining what a line of code does.

```tcl
# This sets variable a to the result of 3 + 5
set a [expr 3 + 5]
```

---

### 11. Assign a string to a variable and print it.

```tcl
set str abcd
puts "$str"
```

---

### 12. Concatenate two strings using `set`.

```tcl
set str1 efg
puts "$str$str1"
```

---

### 13. Try printing variables without using `puts`. Does it work?

```tcl
set x 100
x
```

> ❌ This won't print anything in a script.
> ✅ In `tclsh` (interactive mode), it returns the value.
> In scripts, always use `puts`.

---

### 14. What’s the output of: `puts "Value: [expr 5 * 2]"`?

```tcl
puts "Value: [expr 5 * 2]"
```

> ✅ Output: `Value: 10`

---

### 15. Predict and test the output of this:

```tcl
set a 4
set b 2
set result [expr ($a + $b) * 3]
puts $result
```

> 🔍 Predicted output: `18`  
> ✅ Actual output: `18`

---


