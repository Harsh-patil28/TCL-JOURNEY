## Example 1: Creating a Dictionary
Title: Define a simple dictionary using dict set
```tcl
dict set student name "Harsh"
dict set student age 22
dict set student branch "ECE"
```

## Example 2: Getting a Value
Title: Access a value by key
```tcl
puts "Student Name: [dict get $student name]"
```

## Example 3: Checking Key Existence
Title: Check if a key is present
```tcl
if {[dict exists $student age]} {
    puts "Age exists."
}
```

## Example 4: Removing a Key
Title: Remove a key-value pair
```tcl
dict unset student age
```

## Example 5: Iterating Over Dictionary
Title: Print all keys and values
```tcl
dict for {key value} $student {
    puts "$key -> $value"
}
```

## Example 6: Nested Dictionary
Title: Store nested info (e.g., marks per subject)
```tcl
dict set student marks(math) 90
dict set student marks(science) 85
puts "Math marks: [dict get $student marks(math)]"
```

##  Example 7: Counting Key-Value Pairs
Title: Size of dictionary
```tcl
puts "Total fields: [dict size $student]"
```


