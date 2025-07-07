# 📘 TCL Learning – Day 7

Topic: File Handling in TCL

Date: July 7, 2025

# 🔹 What is File Handling?
File handling in TCL allows you to:

Create files

Read from files

Write or append content to files

Close files properly

File operations are done using file channels, which are like pointers to open files.

# 🔑 TCL File Handling Commands

| Command       | Description                         |
|---------------|-------------------------------------|
| `open`        | Opens a file and returns a file handle |
| `puts`        | Writes a string to a file           |
| `gets`        | Reads a line from a file            |
| `read`        | Reads entire content of a file      |
| `close`       | Closes the file handle              |
| `eof`         | Checks for End Of File              |
| `file exists` | Checks if a file exists             |


# 🔹 Opening Modes

| Mode | Description                  |
|------|------------------------------|
| `r`  | Read-only                    |
| `w`  | Write (overwrites if exists) |
| `a`  | Append to file               |
| `r+` | Read and write               |
| `w+` | Write and read               |

