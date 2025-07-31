# 📘 TCL Learning – Day 26

Topic: String Handling and Pattern Matching in TCL

Date: July 26, 2025

TCL provides powerful commands for string manipulation, including slicing, case conversion, searching, and matching. Pattern matching uses string match, regexp, and regsub for simple glob or complex regex operations. This is very useful in parsing logs, validating input, and EDA script automation.

# 🔹 Common String Operations
| Operation              | Command                                  | Example                                     |
|------------------------|------------------------------------------|---------------------------------------------|
| String length          | `string length $str`                     | `string length "TCL"` → `3`                 |
| Convert to upper/lower | `string toupper / tolower`              | `string tolower "HELLO"` → `"hello"`        |
| Extract substring      | `string range $str start end`           | `string range "hello" 1 3` → `"ell"`        |
| Find index of char     | `string first $substr $str`             | `string first "e" "hello"` → `1`            |
| Compare strings        | `string compare $a $b`                  | `string compare "abc" "ABC"`                |
| Replace using regex    | `regsub pattern input replacement`      | —                                           |
| Match using glob       | `string match pattern string`           | `string match "H*"` `"Hello"` → `1`         |

# 🎯 Pattern Matching Types
| Type     | Command        | Pattern Syntax                        |
|----------|----------------|----------------------------------------|
| Glob     | `string match` | `*`, `?`, `[abc]`, `[!abc]`            |
| Regex    | `regexp`       | Full regular expressions              |
| Replace  | `regsub`       | Replaces pattern match with string    |
