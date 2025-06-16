# Development Guidelines

This document provides technical guidelines to help you contribute code in a consistent and maintainable way.

## Code Style

## General rules

- Follow the Boy Scout rule: *Leave the code better than you found it.*
- Follow the existing style conventions of the repository.
- For C/C++ code, use [clang-format](https://clang.llvm.org/docs/ClangFormat.html) with the provided `.clang-format` config (if any).
- For Go code, run `go fmt` before submitting.
- For Lua, Ruby, and other languages, follow community standards and existing project style.

### Names

Use combination of **CamelCase**, **snake_case**, and **SCREAMING_CASE**:

- **CamelCase** (Capitalize the first letter, including all letters in an acronym) in a class, struct, or namespace name.
- **snake_case** (all lowercase, with underscores separating words) for variable and function names.
- **SCREAMING_CASE** for constants (both global and static member variables).
- **kebab-case** (all lowercase, with dashes separating words) when writing in Lisp-like language (e.g. elisp, fennel).

## Tools and Environment

- Use the provided build scripts or Makefiles (if any) to build and test the code.
- Use your preferred IDE or editor, but ensure the code passes any automated checks before submitting.

## Testing

- Write tests for new features or bug fixes whenever possible.
- Follow the existing testing framework and style.
- Run all tests locally before submitting a PR.
- Make sure new code does not break existing tests.

## Submitting Changes

- Make sure your branch is up to date with the main branch before creating a PR.
- Keep your commits focused and descriptive.
- Include documentation updates if your changes affect usage or APIs.