##  Example 1: Creating a Namespace
```tcl
namespace eval MathOps {
    proc add {a b} {
        return [expr {$a + $b}]
    }
}

puts [MathOps::add 5 6]  ;# Output: 11
```

## Example 2: Namespace Variables
```tcl
namespace eval Config {
    variable version 1.0
    proc showVersion {} {
        variable version
        puts "Version: $version"
    }
}

Config::showVersion
```

## Example 3: Global Variables
```tcl
set count 10

proc printCount {} {
    global count
    puts "Count is $count"
}
printCount
```

## Example 4: Scope Isolation
```tcl
namespace eval Env1 {
    variable name "TCL"
}

namespace eval Env2 {
    variable name "VLSI"
}

puts "Env1: $Env1::name"
puts "Env2: $Env2::name"
```

