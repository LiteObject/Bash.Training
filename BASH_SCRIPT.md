# Getting Started with Shell Scripting for Bash

## How to write a simple script

## How to execute your script
    chmod +x your_script_name.sh

## What is Shebang or Hashbang

## How to debug script (with -x and more)

## Shell variables (with or without EXPORT)

## Arguments vs Options

## End of options

## `=` with or without space around

## Conditions with `if`, `then`, `else`, `fi`

## Single `[  ]` vs Double `[[  ]]` Square Brackets

In Bash scripting, you can use both `[ ]` (single square brackets) and `[[ ]]` (double square brackets) to construct conditional statements within the `if` statement. However, there are some differences between them.

- Single Square Brackets `[ ]`:
  - Single square brackets are the traditional way of constructing conditions in Bash.
  - Use single square brackets for basic string or numeric comparisons.
  - Requires proper spacing inside the brackets.

- Double Square Brackets `[[ ]]`:
  - Double square brackets provide extended functionality and are generally preferred for more complex conditions.
  - They allow additional features, such as pattern matching and regular expressions.
  - Generally, `[[ ]]` is more versatile and safer for conditional statements.

Choose the square bracket notation based on the complexity of your conditions. For basic comparisons, `[ ]` is sufficient, but if you need extended features, prefer `[[ ]]`.

## Comparison Operators

Both `[ ]` and `[[ ]]` support various comparison operators, such as `-eq`, `-ne`, `-lt`, `-le`, `-gt`, `-ge` for numeric comparisons, and `==`, `!=` for string comparisons.

