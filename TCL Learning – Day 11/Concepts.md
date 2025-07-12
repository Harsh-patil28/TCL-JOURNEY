# 📘 TCL Learning – Day 11

Topic: Advanced TCL Arrays – Sorted Keys, Pattern Matching, and Filtering

Date: July 11, 2025

TCL arrays are associative arrays, meaning they store data as key-value pairs. Today, we'll explore advanced operations on arrays including:

Iterating keys in sorted order

Matching array keys using patterns

Filtering array content using conditions

These techniques are especially useful when processing dynamic datasets, configurations, or look-up tables.

# 🔹 Key Concepts and Commands

| Command                  | Description                                 |
|--------------------------|---------------------------------------------|
| `array names arr`        | Returns a list of keys in the array         |
| `lsort`                  | Sorts a list (used for sorting keys)        |
| `string match pattern key` | Matches key to a pattern (wildcards allowed) |
| `regexp`                 | Filters keys/values using regex patterns    |
| `info exists arr(key)`   | Checks if a key exists in the array         |
