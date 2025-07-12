# 💻 TCL Programming Exercises

### 1. Create an array `marks` with keys as names and values as scores.
```tcl
array set marks { abc 24 abcd 45 efgh 98 fap 71 John 56}
```

### 2. Print all students in sorted order of names.
```tcl
foreach i [lsort [array names marks]] {
  puts "$i - $marks($i)"
}
```

### 3. Print only students whose names start with "A" using array keys.
```tcl
foreach i [array names marks a*] {
  puts "$i"
}
```

### 4. Print only students who scored more than 70.
```tcl
foreach i [array names marks] {
  if { $marks($i) > 70 } {
    puts "$i"
  }
}
```

### 5. Check if the key "John" exists and print the score.
```tcl
if { [info exist marks(John)] } {
  puts "$marks(John)"
}
```

### 6. Create an array `cities` and print cities starting with "N".
```tcl
array set cities {
    NewYork "USA"
    Nairobi "Kenya"
    Tokyo "Japan"
    Delhi "India"
    Naples "Italy"
    Berlin "Germany"
}
foreach i [array names cities] {
    if {[string match N* $i]} {
        puts $i
    }
}
```

### 7. Print sorted list of all keys from array `contacts`.
```tcl
array set contacts {
    Alice 12345
    John 67890
    Bob 11223
    Diana 99887
}
foreach i [lsort [array names contacts]] { 
puts "$i"
}
```

### 8. Using regexp, find and print keys in array `logData` that end in a digit.
```tcl
array set logData {
    entry1 "Login"
    sessionA "Active"
    data3 "Saved"
    user "Admin"
    temp5 "Expired"
}

foreach i [array names logData] {
  if {[regexp {\d$} $i]} {
    puts "$i"
  }
}
```
