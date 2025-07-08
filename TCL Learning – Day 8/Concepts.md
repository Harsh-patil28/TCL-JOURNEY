# 📘 TCL Learning – Day 8

Topic: Lists vs Arrays in TCL – Differences and Use Cases

Date: July 8, 2025

TCL provides two important data structures to store collections of data: lists and arrays. While both hold multiple values, they differ significantly in structure, syntax, and access mechanisms.

# 🔹 What is a List?
A list in TCL is an ordered collection of space-separated elements treated as a single string internally.
```tcl
set mylist {apple banana mango}
```
Index-based access (lindex)

Best for sequences, ordered collections


# 🔹 What is an Array?
An array in TCL is a collection of key-value pairs (associative array). Keys are strings or numbers, and each key maps to a value.
```tcl
array set fruitColor {apple red banana yellow}
```
Accessed using key-based syntax ($array(key))

Ideal for mapping, lookup tables, or dictionaries

# 🔄 Key Differences: Lists vs Arrays

| Feature         | List                            | Array                             |
|----------------|----------------------------------|-----------------------------------|
| **Structure**   | Ordered, index-based            | Unordered, key-based (associative)|
| **Access Method** | `lindex`, `lrange`, etc.       | `$array(key)`                     |
| **Mutability**  | Treated as a single string      | Each element stored independently |
| **Use Case**    | Sequences, iterations           | Key-value mapping                 |
| **Size Retrieval** | `llength`                    | `array size`                      |

