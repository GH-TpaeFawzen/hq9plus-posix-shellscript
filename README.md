# hq9plus-posix-shellscript
HQ9+ interpreter in POSIX-compliant shellscript

# Requirements
Following POSIX-copliant utilities:
* `sh`
* `cat`
* `printf`
* `od`
* `tr`
* `sed`
* `grep`
* `awk`

# Files
`hq9plus` is the HQ9+ interpreter written in shellscript.

# Installation and Uninstallation
Just place `hq9plus` to the directory described in environment variable `PATH`.

# Synonym
```
hq9plus FILE
```

## Note on synonym
If `FILE` begins with a hyphen character (`-`), 
the interpreter may not work because the interpreter actually passes 
the arguments to the POSIX utility `cat`.

# Grammar of HQ9+ program
This interpreter is case-sensitive. `H`, `Q`, `9`, and `+` are valid command characters.
Your program may contain other characters but they are ignored.

This interpreter translates your code into hexadecimal once and read byte-by-byte.
If your program is written in non-ASCII-compatible encoding, your HQ9+ program may not work properly.

# License
Distributed under CC0. See 'LICENSE' for more details.
