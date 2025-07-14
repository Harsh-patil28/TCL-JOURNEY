## Example 1: Current Timestamp
```tcl
set now [clock seconds]
puts "Timestamp: $now"
```

## Example 2: Human-Readable Format
```tcl
puts [clock format [clock seconds] -format "%Y-%m-%d %H:%M:%S"]
```

## Example 3: Scan a Date to Timestamp
```tcl
set t [clock scan "1 Jan 2025"]
puts "Timestamp: $t"
```

## Example 4: Add 7 Days to Current Time
```tcl
set nextWeek [clock add [clock seconds] 7 days]
puts [clock format $nextWeek]
```

## Example 5: High-Resolution Time
```tcl
set ms [clock clicks -milliseconds]
puts "Time in ms: $ms"
```

