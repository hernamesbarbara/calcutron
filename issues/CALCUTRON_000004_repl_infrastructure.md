# REPL Infrastructure with Rustyline

## Goal
Implement the basic REPL (Read-Eval-Print Loop) mode using rustyline for interactive calculator sessions.

## Requirements
- Create an interactive REPL mode that activates when no arguments are provided
- Use rustyline for line editing capabilities
- Integrate with the expression parser to evaluate user input
- Provide a clean REPL interface with prompt
- Allow users to exit gracefully (Ctrl+C, Ctrl+D, or "exit" command)

## Technical Details
- Use rustyline::Editor for the REPL interface
- Display a clear prompt (e.g., "calc> ")
- Evaluate each line of input using the existing parser
- Display results or error messages appropriately
- Handle EOF (Ctrl+D) and interrupt signals (Ctrl+C) gracefully
- Support "exit" or "quit" commands to terminate

## Acceptance Criteria
- [ ] Running `calcutron` without arguments starts REPL mode
- [ ] Shows a clear prompt for user input
- [ ] Evaluates expressions and displays results
- [ ] Handles invalid expressions with clear error messages
- [ ] Can exit via Ctrl+D, Ctrl+C, or "exit" command
- [ ] Maintains clean interface without cluttered output

## REPL Flow
```
$ calcutron
calc> 2 + 3
5
calc> 10 - 4 * 2  
2
calc> invalid syntax
Error: Invalid expression: unexpected token
calc> exit
$
```

## Dependencies
Builds on: CALCUTRON_000003_simple_cli