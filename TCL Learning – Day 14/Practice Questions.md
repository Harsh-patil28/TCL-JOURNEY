# 💻 TCL Programming Exercises

### 1. Get the current UNIX timestamp.
```tcl
set clk [clock seconds]
puts "$clk"
```

### 2. Print the current date in DD-MM-YYYY format.
```tcl
set dt [clock format [clock seconds] -format "%d-%m-%y"]
puts "$dt" 
```

### 3. Format the current time as HH:MM:SS.
```tcl
set clk [clock format [clock seconds] -format "%H:%M:%S"]
puts "$clk" 
```

### 4. Get today’s day name (e.g., Monday).
```tcl
set day [clock format [clock seconds] -format "%A"]
puts "$day"
```

### 5. Convert "25 Dec 2024" into a timestamp.
```tcl
set t [clock scan "25 Dec 2024"]
puts "$t"
```

### 6. Add 30 days to the current time and print it.
```tcl
set futureTime [clock add [clock seconds] 30 days]
set formattedDate [clock format $futureTime -format "%d-%m-%Y"]
puts "Date after 30 days: $formattedDate"
```

### 7. Subtract 10 days from the current date and print the result.
```tcl
set pastTime [clock add [clock seconds] -10 days]
set formattedDate [clock format $pastTime -format "%d-%m-%Y"]
puts "Date before 10 days: $formattedDate"
````

### 8. Write a function `daysFromNow {n}` that adds n days and returns the date.
```tcl
proc daysFromNow {n} {
    set now [clock seconds]
    set futureTime [clock add $now $n days]
    return [clock format $futureTime -format "%d-%m-%Y"]
}
puts "[daysFromNow 5]"
```

### 9. Write a function that accepts a date string and prints its weekday.
```tcl
proc thatday { datestr } { 
 set then [clock scan $datestr -format "%d-%m-%Y"]
 set day [clock format $then -format %A]
 return $day
}
puts "[thatday 15-08-1947]"
```

### 10. Print the current date and time in ISO 8601 format (YYYY-MM-DDTHH:MM:SS).
```tcl
puts "[clock format [clock seconds] -format "%d-%m-%y %H:%M:%S"]"
```

### 11. Print current milliseconds using `clock clicks -milliseconds`.
```tcl
puts "[clock clicks -milliseconds]"
```

### 12. Generate a timestamp for "01 Jan 2026 08:30" and format it to display weekday and month.
```tcl

set timestamp [clock scan "01 Jan 2026 08:30" -format "%d %b %Y %H:%M"]
set formatted [clock format $timestamp -format "%A, %B"]
puts $formatted
```


