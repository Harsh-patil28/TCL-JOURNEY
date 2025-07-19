# 📘 TCL Learning – Day 18

Topic: Lists in TCL – Searching, Modifying, and Utility Commands

Date: July 18, 2025


# 🔹 Tcl List Commands Overview

## 📋 Commonly Used List Commands

| Command   | Purpose                                  | Common Syntax / Example                          |
|-----------|-------------------------------------------|--------------------------------------------------|
| `lindex`  | Access an element by index               | `lindex $list 2` → gets the 3rd element          |
| `llength` | Get the length of a list                 | `llength $list`                                  |
| `lrange`  | Extract a sublist                        | `lrange $list 1 3` → elements from index 1 to 3  |
| `linsert` | Insert an item at a specified index      | `linsert $list 2 "new"`                          |
| `lreplace`| Replace elements in a range              | `lreplace $list 1 2 "new1" "new2"`               |
| `lsearch` | Search for a value, return index         | See `lsearch` options below                      |
| `lset`    | Modify an element at an index            | `lset listVar 1 "updated"`                       |
| `lsort`   | Sort a list                              | See `lsort` options below                        |
| `lappend` | Append one or more items to a list var   | `lappend myList "item1" "item2"`                 |
| `lmap`    | Transform items in a list (Tcl 8.6+)     | `lmap x $list {string toupper $x}`               |

---

## ⚙️ `lsort` Options

| Option         | Description                           | Example                             |
|----------------|---------------------------------------|-------------------------------------|
| `-ascii`       | Sort using ASCII string comparison    | `lsort -ascii $list`                |
| `-integer`     | Sort as integers                      | `lsort -integer $list`              |
| `-real`        | Sort as floating-point numbers        | `lsort -real $list`                 |
| `-increasing`  | Ascending order (default)             | `lsort -increasing $list`           |
| `-decreasing`  | Descending order                      | `lsort -decreasing $list`           |
| `-unique`      | Remove duplicates during sort         | `lsort -unique -ascii $list`        |

---

## 🔎 `lsearch` Options

| Option         | Description                                      | Example                                      |
|----------------|--------------------------------------------------|----------------------------------------------|
| `-exact`       | Match exact string                               | `lsearch -exact $list "yes"`                 |
| `-glob`        | Glob-style wildcard pattern                      | `lsearch -glob $list "y*"`                   |
| `-regexp`      | Regular expression matching                      | `lsearch -regexp $list {^A}`                 |
| `-all`         | Return all matching indices                      | `lsearch -all -exact $list "yes"`            |
| `-inline`      | Return matching values (not indices)             | `lsearch -inline -all -regexp $list {^A}`    |
| `-not`         | Return elements that **do not** match (Tcl 8.7+) | `lsearch -not -inline -all $list "no"`       |

---

## ✅ Tips

- Use `llength` to check if the list is empty before division or indexing.
- Use `lmap` for transformations (Tcl 8.6+).
- `string match`, `regexp`, and `lsearch` are often interchangeable for filtering.
