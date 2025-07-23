# 📘 TCL Learning – Day 23

Topic: Working with Associative Arrays (Dictionaries) in TCL

Date: July 23, 2025

In TCL, associative arrays (also called dictionaries) are key-value data structures used for fast lookups. Each key maps to a corresponding value. TCL supports two main forms of dictionaries:

`array `(TCL's original associative array)

`dict` (introduced in TCL 8.5, more modern and script-friendly)

# 🔹 Why Use dict?
Maintains clear structure for key-value storage.

Supports nested dictionaries.

Good readability and easier parsing in scripts.

# 🛠️ Dictionary Commands
| Command      | Description                          |
|--------------|--------------------------------------|
| `dict set`   | Add or update a key-value pair       |
| `dict get`   | Retrieve the value of a key          |
| `dict exists`| Check if a key exists                |
| `dict unset` | Remove a key-value pair              |
| `dict keys`  | Get all keys                         |
| `dict values`| Get all values                       |
| `dict size`  | Get number of pairs                  |
| `dict for`   | Iterate over key-value pairs         |
