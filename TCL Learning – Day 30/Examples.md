## Example 1: Read Lines into a List
Title: Store file contents as a list
```tcl
set fileData [list]
set fid [open "data.txt" "r"]
while {[gets $fid line] >= 0} {
    lappend fileData $line
}
close $fid

puts "List from file: $fileData"
```

## Example 2: Modify List and Write to File
Title: Add a new line and write back to file
```tcl
lappend fileData "New line added"
set fid [open "data.txt" "w"]
foreach line $fileData {
    puts $fid $line
}
close $fid
```

## Example 3: Filter and Store Selected Lines
Title: Write only lines containing 'error'
```tcl
set fid_in [open "log.txt" "r"]
set errorLines [list]

while {[gets $fid_in line] >= 0} {
    if {[string match "*error*" $line]} {
        lappend errorLines $line
    }
}
close $fid_in

set fid_out [open "error_report.txt" "w"]
foreach err $errorLines {
    puts $fid_out $err
}
close $fid_out
```

##  Example 4: Count Occurrences
Title: Count how many times a specific word appears in a file
```tcl
set count 0
set fid [open "data.txt" "r"]
while {[gets $fid line] >= 0} {
    if {[string match "*line*" $line]} {
        incr count
    }
}
close $fid

puts "Occurrences of 'line': $count"
```
