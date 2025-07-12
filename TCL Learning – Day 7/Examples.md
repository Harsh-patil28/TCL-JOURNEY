## Example 1: Writing to a File
```tcl
set fh [open "output.txt" "w"]
puts $fh "This is a TCL file write example."
close $fh
```

## Example 2: Reading a File Line by Line
```tcl
set fh [open "output.txt" "r"]
while {![eof $fh]} {
    gets $fh line
    puts "Read: $line"
}
close $fh
```

## Example 3: Appending Content to a File
```tcl
set fh [open "output.txt" "a"]
puts $fh "Appending new line."
close $fh
```

## Example 4: Reading Entire File at Once
```tcl
set fh [open "output.txt" "r"]
set content [read $fh]
puts "Full content:\n$content"
close $fh
```

##  Example 5: Check If File Exists
```tcl
if {[file exists "output.txt"]} {
    puts "File exists."
} else {
    puts "File not found."
}
```
