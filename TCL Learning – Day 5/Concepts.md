# 📘 TCL Learning – Day 4

Topic: Lists and List Manipulation Commands in TCL

Date: July 5, 2025

# 🔹 Creating a List
TCL lists are immutable strings under the hood but treated as list structures via special commands.
```tcl
set fruits {apple banana mango}
```

# 🛠️ Common List Commands

| Command     | Description                                     |
|-------------|-------------------------------------------------|
| `list`      | Creates a list                                  |
| `llength`   | Returns number of elements in the list          |
| `lindex`    | Access element at a given index                 |
| `lrange`    | Extract a sublist from start to end index       |
| `lappend`   | Append element(s) to the end of a list          |
| `linsert`   | Insert element(s) at a specific index           |
| `lreplace`  | Replace elements between given indices          |
| `lsearch`   | Search for an element and return its index      |
| `lsort`     | Sort the list                                   |
| `split`     | Split a string into a list                      |
| `join`      | Join list elements into a string                |
| `foreach`   | Iterate over each element in a list             |
| `concat`    | Merge multiple lists into one flat list         |
| `lset`      | Set value of an element at a specific index     |
| `lrange $list end end` | Get the last element of the list    |
