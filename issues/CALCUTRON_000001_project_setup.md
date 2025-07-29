# Project Setup and Foundation

## Goal
Set up a basic Rust project with the required dependencies and project structure.

## Requirements
- Create Cargo.toml with dependencies: chumsky, rustyline, clap
- Set up basic project structure with main.rs
- Add basic CLI argument parsing structure
- Ensure project compiles and runs with --help

## Technical Details
- Use clap for command line argument parsing
- Set up project to support both single expression mode and REPL mode
- Add proper error handling infrastructure
- Configure cargo to build a binary named "calcutron"

## Acceptance Criteria
- [ ] `cargo build` succeeds
- [ ] `cargo run -- --help` shows usage information
- [ ] Project structure is ready for expression parsing
- [ ] Dependencies are properly configured

## Dependencies
- chumsky (parser combinator library)
- rustyline (readline implementation for Rust)
- clap (command line argument parser)

## Notes
This is the foundation step that all other features will build upon.