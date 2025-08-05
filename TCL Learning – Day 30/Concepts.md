# 📘 TCL Learning – Day 30
Topic: Working with Lists and Files Together in TCL

Date: July 30, 2025

In practical EDA scripting, we often store data from files into lists for easier processing. Today we explore how to:

Read file lines into a list

Iterate over that list

Modify and write the updated list back to a file

This is useful for scripts that preprocess configuration files, manage test case lists, or log reports.

# 🔹 Combining Lists and Files
Common operations:

Store file lines into a list using a loop

Apply lappend, lindex, lsearch, linsert, lreplace on file data

Write list contents back to a file

# 🛠️ Useful Combinations
| Task                      | Useful Combination                        |
|---------------------------|-------------------------------------------|
| Collect all lines into a list | `gets` + `lappend`                      |
| Update specific lines     | `lreplace` or `linsert`                   |
| Filter based on pattern   | `string match` inside a loop              |
| Dump list to file         | `foreach` + `puts`                        |
| Extract subset of lines   | `lrange` or `lsearch`                     |
