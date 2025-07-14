# 📘 TCL Learning – Day 14

Topic: Working with Time, Date, and Clocks in TCL

Date: July 14, 2025

TCL provides the clock command for handling date and time operations. This is useful in scheduling, logging, timestamps, or time-based calculations.

# 🔹 The `clock` Command

| **Subcommand**        | **Description**                                             |
|-----------------------|-------------------------------------------------------------|
| `clock seconds`       | Returns the current UNIX timestamp (seconds since 1970)     |
| `clock format`        | Formats a timestamp into a human-readable string            |
| `clock scan`          | Converts a date/time string into a timestamp                |
| `clock add`           | Adds/subtracts time units to/from a timestamp               |
| `clock clicks`        | Returns high-resolution time (milliseconds)                 |
| `clock milliseconds`  | Returns current time in milliseconds                        |


# 📐 Common Formatting Options

| **Format String** | **Description**              |
|-------------------|------------------------------|
| `%Y`              | Year (e.g., 2025)            |
| `%m`              | Month (01–12)                |
| `%d`              | Day of month (01–31)         |
| `%H`              | Hour (00–23)                 |
| `%M`              | Minute (00–59)               |
| `%S`              | Seconds (00–59)              |
| `%A`              | Full weekday name            |
| `%b`              | Abbreviated month            |


