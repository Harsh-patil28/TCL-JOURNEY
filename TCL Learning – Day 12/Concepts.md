# 📘 TCL Learning – Day 12

Topic: Namespaces and Variable Scoping in TCL

Date: July 12, 2025

# 🔹 What is a Namespace?
A namespace is a container for:

Variables

Procedures

Other namespaces

It helps avoid naming conflicts between multiple libraries or modules.

# 🔹 Why Use Namespaces?
| **Benefit**  | **Description**                        |
|--------------|----------------------------------------|
| Isolation    | Prevent name clashes                   |
| Modularity   | Organize code into logical sections    |
| Reusability  | Package up reusable procedures/variables |

# 🔹 Variable Scope in TCL
| **Scope Type** | **Description**                              |
|----------------|----------------------------------------------|
| Global         | Exists throughout the program                |
| Local          | Exists within procedures or blocks           |
| Namespace      | Confined to a specific namespace             |

**Use:**
- `global` to access a global variable inside a `proc`
- `variable` to access namespace-scoped variables inside a namespace

# 📘 Key Commands
| **Command**                    | **Description**                                      |
|--------------------------------|------------------------------------------------------|
| `namespace eval <ns> {}`       | Define and run code inside a namespace               |
| `namespace current`            | Returns current namespace                            |
| `namespace which`              | Tells where a variable/procedure is located          |
| `variable`                     | Declares/uses namespace variable                     |
| `global`                       | Accesses global variable inside procedures           |
