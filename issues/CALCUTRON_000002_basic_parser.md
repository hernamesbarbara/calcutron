# Basic Expression Parser with Chumsky

## Goal
Implement a basic arithmetic expression parser using chumsky that can handle C-style expressions.

## Requirements
- Create an expression parser that handles:
  - Basic arithmetic operators: +, -, *, /
  - Parentheses for grouping
  - Integer and floating-point numbers
  - Proper operator precedence (PEMDAS/BODMAS)
- Create an evaluator that computes the result
- Add comprehensive error handling for parsing failures

## Technical Details
- Use chumsky's parser combinators to build the expression grammar
- Support both integer and floating-point arithmetic
- Handle operator precedence correctly (* and / before + and -)
- Return meaningful error messages for invalid expressions

## Acceptance Criteria
- [ ] Can parse simple expressions: "2 + 3", "10 - 5"
- [ ] Can parse complex expressions: "2 + 3 * 4", "(2 + 3) * 4"
- [ ] Can handle floating-point numbers: "3.14 + 2.5"
- [ ] Respects operator precedence
- [ ] Returns clear error messages for invalid syntax
- [ ] All parsing logic is tested

## Test Cases
- "2 + 3" → 5
- "10 - 4 * 2" → 2
- "(10 - 4) * 2" → 12
- "3.14 + 2.86" → 6.0
- "invalid expression" → meaningful error

## Dependencies
Builds on: CALCUTRON_000001_project_setup