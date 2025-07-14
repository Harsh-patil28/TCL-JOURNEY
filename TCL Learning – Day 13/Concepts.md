# 📘 TCL Learning – Day 13

Topic: Creating and Using Packages in TCL

Date: July 13, 2025

# 🔹 Why Use Packages?

| **Feature**       | **Purpose**                                      |
|-------------------|--------------------------------------------------|
| Code Reuse        | Use logic across multiple scripts                |
| Modular Design    | Organize large codebases into manageable components |
| Maintainability   | Update one package and reuse it everywhere       |

# 📦 Key Terms

| **Term**           | **Description**                                               |
|--------------------|---------------------------------------------------------------|
| `package provide`  | Declares the version of the package being created             |
| `package require`  | Loads the package in another script                           |
| `package ifneeded` | Registers a package with the interpreter                      |
| `auto_path`        | List of directories TCL uses to search for packages           |
| `.tcl` File        | Package files are stored with `.tcl` extension                |

# 🔄 Creating a Package – Structure

# 📁 Directory Layout Example

```bash
project/
│
├── mymath.tcl         # Your package file
├── test_script.tcl    # Your main script that uses the package
