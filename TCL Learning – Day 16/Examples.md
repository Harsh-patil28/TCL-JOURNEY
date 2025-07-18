## Example 1: Writing to a File
```tcl
set fileId [open "notes.txt" "w"]
puts $fileId "This is line one"
puts $fileId "This is line two"
close $fileId
```

## Example 2: Reading a File Line-by-Line
```tcl
set fileId [open "notes.txt" "r"]
while {![eof $fileId]} {
    gets $fileId line
    puts "Read: $line"
}
close $fileId
```

## Example 3: Appending to a File
```tcl
set fileId [open "notes.txt" "a"]
puts $fileId "Appended line"
close $fileId
```

## Example 4: Reading Full File at Once
```tcl
set fileId [open "notes.txt" "r"]
set content [read $fileId]
puts "Full File:\n$content"
close $fileId
```

## Example 5: File I/O with Error Handling
```tcl
if {[catch {open "missing.txt" "r"} fileId]} {
    puts "Error opening file: $fileId"
} else {
    puts [read $fileId]
    close $fileId
}
```
