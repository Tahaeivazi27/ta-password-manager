## Development Conventions

### General

- Follow the official Python PEP 8 style guide.
- Keep the code clean, readable, and maintainable.
- Prefer simplicity over unnecessary complexity.

### Naming Conventions

- Use `snake_case` for variables, functions, and file names.
- Use `PascalCase` for class names.
- Use `UPPER_SNAKE_CASE` for constants.
- Choose meaningful and descriptive names.

### Type Hints

- Use type hints for all public functions and methods whenever possible.

### Documentation

- Write docstrings for public classes, methods, and functions.
- Keep comments concise and explain *why*, not *what*.

### File Organization

- Prefer one public class per file.
- Keep files focused on a single responsibility.

### Imports

- Group imports according to PEP 8:
  1. Standard Library
  2. Third-party packages
  3. Local project modules

### Code Quality

Before every commit:

- All tests must pass.
- Ruff must report no errors.
- The project should remain free of unnecessary warnings.

### Git

- Write clear and meaningful commit messages.
- Commit small, logical changes instead of large batches.