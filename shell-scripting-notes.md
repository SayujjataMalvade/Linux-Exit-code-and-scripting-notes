# Shell Scripting Notes

## Arguments
- $1, $2 ... are positional arguments
- Arguments are just text
- Can pass numbers, strings, paths, flags, commands

## Variables
- Global variables: accessible everywhere
- Local variables: defined inside functions using `local`

Best practice:
- Use arguments ($1) inside functions
- Convert arguments into local variables

## Arithmetic
Bash treats everything as text by default.
Arithmetic operations must use:

$(( expression ))

Example:
$(( a + b ))
