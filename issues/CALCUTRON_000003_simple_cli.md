# Simple CLI Calculator Mode

## Goal
Implement the single-expression calculator mode where users can pass a math expression as a command line argument.

## Requirements
- Accept a single expression as a command line argument
- Parse and evaluate the expression using the parser from step 2
- Print the result to stdout
- Handle and display parsing/evaluation errors gracefully
- Support the usage: `calcutron "2 + 3 * 4"`

## Technical Details
- Use clap to define command line interface
- Integrate with the expression parser created in CALCUTRON_000002
- Provide clear error messages when expressions are invalid
- Exit with appropriate exit codes (0 for success, 1 for errors)

## Acceptance Criteria
- [ ] `calcutron "2 + 3"` outputs "5"
- [ ] `calcutron "10 - 4 * 2"` outputs "2"  
- [ ] `calcutron "(10 - 4) * 2"` outputs "12"
- [ ] `calcutron "3.14 + 2.86"` outputs "6"
- [ ] `calcutron "invalid"` shows helpful error message
- [ ] `calcutron --help` shows usage information
- [ ] Exit codes are correct (0 for success, 1 for error)

## Usage Examples
```bash
calcutron "2 + 3"           # outputs: 5
calcutron "10 - 4 * 2"      # outputs: 2
calcutron "(1 + 2) * 3"     # outputs: 9
calcutron "bad syntax"      # outputs error message
```

## Dependencies
Builds on: CALCUTRON_000002_basic_parser