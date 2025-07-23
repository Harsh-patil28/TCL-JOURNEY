# 💻 TCL Programming Exercises

### 1. Create a dictionary book with keys: title, author, year, price.
```tcl
dict set book title Abcd
dict set book author Myname
dict set book year 2025
dict set book price 200
```

### 2. Retrieve and print the value of each key.
```tcl
dict for {key value} $book {
    puts "$key: $value"
}
```

### 3. Add a key publisher and assign a value.
```tcl
dict set book publisher Github
dict for {key value} $book {
    puts "$key: $value"
}
```

### 4. Remove the price entry.
```tcl
dict unset book price
dict for {key value} $book {
    puts "$key: $value"
}
```

### 5. Check if the key year exists.
```tcl
if {[dict exists $book year]} {
  puts "Year exists"
}
```

### 6. Create a nested dictionary employee with keys: name, salary, and address(city, pincode).
```tcl
dict set employee name Myname
dict set employee salary 15k
dict set employee address(city) Mycity
dict set employee address(pincode) 580010
```

### 7. Access and print the employee's pincode.
```tcl
puts "[dict get $employee address(pincode)]"
```

### 8. Count the total number of fields in book and employee.
```tcl
puts "Total fields in book: [dict size $book]"
puts "Total fields in employee: [dict size $employee]"
```
