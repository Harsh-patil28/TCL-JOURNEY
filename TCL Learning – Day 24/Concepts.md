# 📘 TCL Learning – Day 24
Topic: Traditional Arrays in TCL – Declaration, Indexing, and Iteration

Date: July 24, 2025

In addition to dict, TCL provides another form of associative data structure called an array. TCL arrays are indexed by strings and allow efficient key-value mapping, but they use a different command interface (array instead of dict). These are more traditional and useful in procedural-style scripts.

#🔹 Key Differences: dict vs array
| Feature      | `dict`                                 | `array`                              |
|--------------|-----------------------------------------|---------------------------------------|
| **Storage**   | Single variable with key-value pairs    | One variable with indexed elements    |
| **Access**    | `dict get var key`                     | `$var(key)`                           |
| **Persistence** | Stored as a string (serializable)     | Native memory structure               |
| **Use-case**  | Structured config/data passing          | Runtime data storage and lookup       |


# 🛠️ TCL Array Syntax
| Operation            | Syntax                                      |
|----------------------|----------------------------------------------|
| Declare/Assign       | `set arrayName(key) value`                  |
| Read                 | `puts $arrayName(key)`                      |
| Get all keys         | `array names arrayName`                     |
| Get all values       | Loop using `foreach` on keys               |
| Delete an element    | `unset arrayName(key)`                      |
| Delete entire array  | `unset arrayName`                           |
| Iterate all elements | `foreach key [array names arrayName]`       |
