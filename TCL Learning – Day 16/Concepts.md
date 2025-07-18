# 📘 TCL Learning – Day 16

Topic: File I/O – Reading, Writing, and Appending Files in TCL

Date: July 16, 2025

TCL enables file operations using channels. You can open a file in various modes for reading, writing, or appending. File handling is essential for logging, data processing, and scripting automation.

# 🔹 File Modes in TCL
| Mode | Purpose                               |
|------|----------------------------------------|
| r    | Read-only                              |
| w    | Write (overwrites existing file)       |
| a    | Append (adds to end of file)           |
| r+   | Read and write                         |
| w+   | Read and write (overwrites file)       |
| a+   | Read and append                        |

# 🔹 Key File I/O Commands
| Command               | Description                             |
|-----------------------|-----------------------------------------|
| open <file> <mode>    | Opens a file and returns a channel ID   |
| puts <channel> <text> | Writes text to a file                   |
| gets <channel>        | Reads a line from a file                |
| read <channel>        | Reads full contents of file             |
| close <channel>       | Closes the open file channel            |
| eof <channel>         | Checks for end-of-file                  |
| seek, tell            | Used for moving file pointers           |
